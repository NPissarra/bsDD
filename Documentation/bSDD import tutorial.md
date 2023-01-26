# How to import your bSDD model into bSDD?

If you have your model in the bsdd-import-model.json format available, you can upload it into the bSDD database yourself.

*Important* if you upload a file it will replace the whole domain! You cannot upload the classifications in parts, all classifications and properties of one domain must be in one file.

1. If it's the first time you are going to upload, you need to have your e-mail address, the one you used to log in, connected to your organization. To achieve this, send an e-mail with
- your name
- your e-mail address you use to log in the bSDD API
- the name of your organization
- a hyperlink to the website of your organization
- (optional) contact e-mail address in case users have questions about the domain you uploaded

to bsdd_support@buildingsmart.org.
As soon as you've got a reply, you can continue with the next step.

2. Go to [https://manage.bsdd.buildingsmart.org/](bSDD Management App)
or for test environment: [https://manage-test.bsdd.buildingsmart.org](bSDD Management App TEST)

3. Log in

> If you do not have a bSDD buildingSMART account yet, choose "Sign up now", otherwise choose "Sign in"
> 
> <img src="/Documentation/graphics/Screenshot_03_signupsignin.png" alt="Signup/signin" style="width: 400px">

4. If all is well you should see "Upload domain" menu item. Click on it.

5. Select the JSON file you want to upload via button "Select file".
> If you don't know how to create the proper JSON file, read that section: [bSDD JSON import model](/Documentation/bSDD%20JSON%20import%20model.md).

6. Optional: check the "Validate only?" checkbox if you only want to validate the file, not inserting the data

7. Press "Upload selected file"

> If there are any validation errors detected you will see them listed. You will receive a more detailed import report, one that might include warnings, by e-mail once the file has been imported.

# General guidelines

- Manage and publish translations in a seperate files.
- Make specific domains, don't try to put too much data into one domain.
- Link to IFC entities for increased usability.
- Add IFC properties to your content instead of replicating your own properties.
- Make sure you use the correct encoding of characters. 

# Naming conventions and guidelines
Avoid names that conflict with other domains. For example, do not create classifications with an 'Ifc'-prefix. Do not replicate content from other domains, but link to it. 

## Domain name
The domain name needs to be unique. Avoid the use of a name that is generic; choose a domain name that is specific. Global names like 'building products' are not allowed. Add your region or applition (use case application, not software) to the name of the domain to make it specific.

## Domain code
The domain code needs to be unique in the bSDD; choose one that is recognizable with the domain name.
The domain code is used in the URI of all the data, so choose carefully. 

## Organisation name
The organisation name (and URI code) will be assigned by the bSDD team, but suggestions can be made.

## Property set names
Avoid the use of 'Pset_' prefix. This is restricted for IFC only.
Avoid replicating the name of the property or class/classification.
