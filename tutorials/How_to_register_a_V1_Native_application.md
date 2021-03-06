# How to register a V1 Native application

This tutorial introduces how to register the application using Microsoft Azure portal. Once you have registered an application by following this tutorial, you can use it as a "Public client/native (mobile & desktop) app" in Office365APIEditor.

1. Go to https://portal.azure.com/ and sign in using your Office 365 account.
2. Click [Azure Active Directory] in the left panel.
3. Click [App registration].
4. Click [New registration].
5. Enter the name of your application. (e.g. MyPublicApp)
6. It doesn't matter what you select for [Supported account types].
7. Select [Public client/native (mobile & desktop)], and enter the redirect URI of your application in [Redirect URI]. (e.g. https&#58;<span></span>//localhost/MyPublicApp <- Whatever is fine.)
8. Click [Register].
9. Copy the value of [Overview] - [Application (client) ID].
10. Click [API permissions] and add the necessary permissions for your application. If your application has to read the messages in the users' mailbox using Microsoft Graph, you have to add the [Mail.Read] permission under [Delegated permissions] of [Microsoft Graph].
11. Check the following values and use them in Office365APIEditor.

  | Value in Azure portal  | Textbox in Office365APIEditor |  
  |:-----------------------|-------------------------------|  
  |Application (client) ID |Application ID                 |  
  |Redirect URI            |Redirect URI                   |  

  [Tenant name] is your Office 365 tenant name. (e.g. contoso.onmicrosoft.com)