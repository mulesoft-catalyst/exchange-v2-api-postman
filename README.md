# Exchange v2 API Postman Collection

## Introduction
Exchange v2 APIs are a major improvement over earlier version. Exchange v2 APIs provide the following benefits - 
- Improved discoverability
- Manage asset docs and metadata through Exchange v2 APIs 
- Publish all types of assets supported by Exchange 
- Improved error feedback and publication support
- Improved documentation and examples for Exchange APIs

Official Documentation - https://anypoint.mulesoft.com/exchange/portals/anypoint-platform/f1e97bc6-315a-4490-82a7-23abe036327a.anypoint-platform/exchange-experience-api/

This GitHub project provides a Postman collection for users to interact with Anypoint Exchange v2 APIs.

## How to use the Postman Collection
1. Under postman folder there are two files - Environment-template.postman_environment.json and Exchange APIs - v2.postman_collection.json. Import both the files into your postman by clicking on import -> file option
2. Update the MuleSoft environment with appropiate values needed to run collection - **username**, **password**, **orgId**. Some other values will be populated as and when a particular test is run.
3. The Postman collection uses user login to create Bearer token which will be used for calling any Exchange v2 API 
![image](https://user-images.githubusercontent.com/44620039/112908633-d9123580-90bd-11eb-8455-860cb3a14d6e.png)

The API call will automatically store the access token into **access_token** variable.

4. All subsequent calls requires **access_token** to be passed in the header.
5. The **supporting-artifacts** folder contains files needed to test the Postman collection. 
6. While exporting postman collection it would normally not recognize the file path so if does not show the file correctly. Check for the file name and click on x. It would then show option to Select Files. Browse to **supporting-artifacts** folder and choose right file.
![image](https://user-images.githubusercontent.com/44620039/112910259-01e7fa00-90c1-11eb-9ad5-9aeab3c72e77.png)
![image](https://user-images.githubusercontent.com/44620039/112910276-0b716200-90c1-11eb-86ea-b95ae6786ab8.png)
7. Make changes to parameters, version and API body as needed to test.

## Version
Postman - 8.0.6

## Disclaimer
The Postman collection provides users with a medium to interact with Exchange v2 APIs. Users should make changes to Postman collection as per their needs before invoking the APIs. The API list in Postman collection is derived from examples shared in Exchange v2 API documentation.
