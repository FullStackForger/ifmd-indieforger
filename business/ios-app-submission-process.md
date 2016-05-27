# IOS App submission

So you have build your first game, designed all the levels, fixed all the bugs and you want to submit it into App store and you landed here. It means you hit the wall in the maze of Apple developer documentation on (even better) Bureau of Industry and Security of U.S. Department of Comerce. In either way you need help. This guide is one of many sites taking a shot at explaining how to do it in human friendly way. 


## Submiting application to app store

### Links to bookmark

* [Apple developer account](https://developer.apple.com/account)
* [iTunes Connect](https://itunesconnect.apple.com)

### Application provisioning and provisioning profile(s)

From [Creating Your Team Provisioning Profile](https://developer.apple.com/library/ios/documentation/IDEs/Conceptual/AppStoreDistributionTutorial/CreatingYourTeamProvisioningProfile/CreatingYourTeamProvisioningProfile.html):

> Provisioning is the process of preparing and configuring an app to launch on devices and to use app services. During development, you choose which devices can run your app and which app services your app can access.


> A provisioning profile is downloaded from your developer account and embedded in the app bundle, and the entire bundle is code-signed. The embedded provisioning profile is installed on the device before the app is launched. If the information in the provisioning profile doesn’t match certain criteria, your app won’t launch. You indirectly configure a development provisioning profile by choosing options in Xcode.

### Good guides

* [App Distribution Quick Start](https://developer.apple.com/library/ios/documentation/IDEs/Conceptual/AppStoreDistributionTutorial/Introduction/Introduction.html) - official
* [Submitting the App to App Review](https://developer.apple.com/library/ios/documentation/LanguagesUtilities/Conceptual/iTunesConnect_Guide/Chapters/SubmittingTheApp.html) - official
* [How to Submit an iOS App to the App Store](http://code.tutsplus.com/tutorials/how-to-submit-an-ios-app-to-the-app-store--mobile-16812)

### Apple Worldwide Developer Relations Intermediate Certificate Update

Last certificate expired on Feb 14, 2016. All developers should download and install the [renewed certificate](https://developer.apple.com/certificationauthority/AppleWWDRCA.cer) on their development systems and servers. All Apple certificates can be found on [Apple PKI](https://www.apple.com/certificateauthority/) page.

From [Apple Worldwide Developer Relations Intermediate Certificate Expiration][app-cert-expiration]:

>The previous Apple Worldwide Developer Relations Certification Intermediate Certificate expired on February 14, 2016 and the renewed certificate must now be used when signing Apple Wallet Passes, push packages for Safari Push Notifications, Safari Extensions, and submissions to the App Store, Mac App Store, and App Store for Apple TV.


>All developers should download and install the renewed certificate on their development systems and servers. All apps will remain available on the App Store for iOS, Mac, and Apple TV.


Check [Maintaining Your Signing Identities and Certificates](maint-signing-ident) for more information on code signing.

[maint-signing-ident]: https://developer.apple.com/library/ios/documentation/IDEs/Conceptual/AppDistributionGuide/MaintainingCertificates/MaintainingCertificates.html
[app-cert-expiration]: https://developer.apple.com/support/certificates/expiration/

## Legal requirements of submitting application to Apple's App Store

### Export Compliance during App Store submission process

If you using any sort of encryption, including SSL, HTTPS you should answer export complianace questions as follows:

![img](https://carouselapps-wpengine.netdna-ssl.com/wp-content/uploads/2015/11/Mac-App-Store-questions-and-answers-about-encryption.png)

That also means you will need to obtain an Encryption Registration (ERN) approval.

>To make your app available on the App Store, you must submit a copy of your U.S. Encryption Registration (ERN) approval from the U.S. Bureau of Industry (BIS).

In order to obtain the approval you have to register with BIS (Bureau of Industry and Security of U.S. Department). You can register using SNAP-R registration form.

### SNAP-R

[SNAP-R][snap] stands for Simplified Network Application Process - Redesign (SNAP-R) and administer by Bureau of Industry and Security of U.S. Department of Comerce ([BIS][bis]).

> You must have a Company Identification Number (CIN) and an active user account to access SNAP-R.

To obtain CIN scroll down to **Obtaining a CIN** section, click 
[registration form] link and follow the instructions.

You will receive confiramtion email with verification link. Processing might take up to 5 days.

> Your email address has been confirmed and we are processing your registration. You will be notified via email when your SNAP-R login information is available. 

Please allow up to five business days to process your SNAP-R registration.
[bis]: http://www.bis.doc.gov/
[snap]: http://www.bis.doc.gov/index.php/licensing/simplified-network-application-process-redesign-snap-r

### Additional resources

#### Community guides

* [How to legally submit application to Apple's App Store when it uses encryption (or how to obtain ERN)](https://pupeno.com/2015/12/15/legally-submit-app-apples-app-store-uses-encryption-obtain-ern/)
* [Most Mac and iOS applications are breaking the rules and could be removed, is yours?](https://carouselapps.com/2015/12/09/mac-ios-applications-breaking-rules-removed/)

