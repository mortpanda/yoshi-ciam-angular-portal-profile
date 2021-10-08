# ciam-angular-portal-profile
Japanese CIAM Demo Portal Site

<img src="/Capture.PNG" alt="drawing" width="600"/>
<img src="/Capture2.PNG" alt="drawing" width="600"/>
<img src="/Capture3.PNG" alt="drawing" width="600"/>


**Not formally supported by Okta**
This is merely a personal projct, and Okta's support do not offer support for this tool.
Also, the website is currently in Japanese ONLY, and there are no plans for translation into English.

## What does this tool do?
This website is a simple demo site, which will display some bery basic user information retrieved from Okta.

## Development Environment
```
Angular CLI: 11.2.14
Node: 14.15.0
OS: linux x64

Angular: 11.2.14
... animations, cli, common, compiler, compiler-cli, core, forms
... platform-browser, platform-browser-dynamic, router
Ivy Workspace: Yes

Package                         Version
---------------------------------------------------------
@angular-devkit/architect       0.1102.14
@angular-devkit/build-angular   0.1102.14
@angular-devkit/core            11.2.14
@angular-devkit/schematics      11.2.14
@angular/cdk                    11.2.13
@angular/flex-layout            12.0.0-beta.34
@angular/material               11.2.13
@schematics/angular             11.2.14
@schematics/update              0.1102.14
rxjs                            6.6.7
typescript                      4.1.6

```

## How to run this tool
- In a directory of your choice,

- Clone the repo,

- Enter the directory,

- Install pakackages

`npm install`
- Run the tool

`ng serve`
- Open the tool

`http://localhost:4200`

- The below file is used to hold the Okta condfigurations for the application.
`src/app/shared/okta-config.ts`

- The below sample has been included, which you can edit and rename to "okta-config.ts" prior to running your own instance of this application.
`src/app/shared/sample-okta-config.ts`

- Inside the files, the below section will need to be updated with your setting.

```
 strBaseURI = '{{Base URI}}';  
 strRedirectURL = '{{Redirect URI}}';
 strClientID = '{{Client ID}}';
 strIssuer = '{{Issuer URI}}';
 strPostLogoutURL = '{{Redirect URI}}';
 strScope = ['openid', 'email', 'profile','address'];
 strResponseType = ['token','id_token'];
 strResponseMode = 'fragment';
 strPrompt = ['consent','login'];
 strPkce = false;
 strLang = '{{Language code}}';
 strBrand =  '{{Colour}}';
 strLogo = '{{Logo URL}}';
 strMFAClientID = '{{}}';
 strPortalAddress = '{{Portal address}}';

```




