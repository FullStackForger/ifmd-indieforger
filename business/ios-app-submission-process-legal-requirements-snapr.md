# IOS App submission - legal requirements, SNAPR

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

If you using any sort of encryption, including connecting via HTTPS (SSL encryption) you should answer export compliance questions as follows:

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

Allow up to five business days to process your SNAP-R registration.
Once it's done you will get email with activation link. Go ahead, click it and register. Now you can log in.

[bis]: http://www.bis.doc.gov/
[snap]: http://www.bis.doc.gov/index.php/licensing/simplified-network-application-process-redesign-snap-r

### SNAP-R account - work items

Log in to SNAP-R administration panel with [snapr.bis.doc.gov/snapr](https://snapr.bis.doc.gov/snapr/). You might want to
bookmark that link.

Once you have successfully logged in, you can now create work item.

#### Work item type

Select the appropriate Work Item type from the drop-down box.
You may choose from the following: Export License Application, Re-Export License, Agriculture License Exception Notice, Commodity Classification, and Encryption Registration.

<!--
todo: classification for following:
- Keychain - for saving username and password on the device
- server-side app store receipt verification
- "Security by obscurity" which includes hashing, to prevent unauthorized access to the server API
-->

If you are using **SSL** to, for example, call API over **HTTPS** use ***Encryption Registration***.

If have implemented your **own encryption mechanism** use ***Commodity Classification Request*** and take a look at [Mass Market Encryption CCATS Commodity Classification for iPhone Applications in 8 Easy Steps](https://www.zetetic.net/blog/2009/8/3/mass-market-encryption-ccats-commodity-classification-for-ip.html) - it is really good guide that will take you through the process.

#### Reference number

Reference number is an arbitrary unique number in the format `AAA1111` you make up to identify your application.
You could use first three letters of the your company name combining it with current year and month (`YYMM`) or just a ordinary number, eg: `0001`.
Anything that follows required format is acceptable.

Go ahead, create work item and edit the form.

Form is partially filled for you so firstly just make sure contact details are in order, and scroll down to **Additional information** section.

#### Additional information

Registration requires *Supplement no. 5 to part 742 - Encryption Registration* so use **Additional information** to refer to it. Type something like:

> Please see Supplement no. 5 to part 742 - Encryption Registration to complete the Encryption Registration.



#### Documents attached to application

You will need is to create PDF document based on [Supplement no. 5 to part 742 - Encryption Registration template](http://www.ecfr.gov/cgi-bin/retrieveECFR?gp=1&SID=4150cfbf028e9a85574385383a581f47&h=L&mc=true&n=pt15.2.742&r=PART&ty=HTML#ap15.2.742_119.4) you can find on either [www.bis.doc.gov/index.php/policy-guidance/encryption](https://www.bis.doc.gov/index.php/policy-guidance/encryption) or by copying page 60 from [document  742](https://www.bis.doc.gov/index.php/forms-documents/doc_download/1208-742). In either case just fill it with your data and export it as PDF.
Here is an example of the document.

>Supplement No. 5 to Part 742
Encryption Registration
>  
> **(1) Point of Contact**  
> (a) John Smith  
> (b) +44 1111222333  
> (d) your@email.com  
> (e) YOUR COMPANY LTD  
> 10 Some Street  
> WC1A 10Q, London  
> UNITED KINGDOM  
>
> **(2) Company**  
YOUR COMPANY Ltd is small London based company providing consultancy services and producing software application and games.

>  **(3) Categories of technology/families of product**  
  (b) Mobile applications  
  (j) Software   
    (ii) Applications  
    (m) Gaming  
>
> **(4) Cryptographic functionality**  
At YOUR COMPAMY LTD we make software using standard encryption mechanisms such as HTTPS (SSL) and strive to use those in accordance with market standards defined by documentation and commonly accepted best practices. We don’t develop or intend to develop any proprietary encryption mechanisms.
>
> **(5) Exporting source code**  
> We do not export and are not planning to export source code of our application.
>
> (6) Encryption components  
> We develop our mobile applications and games for Apple, Android and Windows devices in accordance to those companies recommended standards and following regulated by them software submission process. While we do not implement encryption components directly, we utilize platform specific functionalities relying on their security and standards for communication over HTTPS, data caching and payment transactions.
>  
> **(7) Manufacturing**  
> N/A, YOUR COMPANY Ltd is not a manufacture company.

Feel free to copy cat it updating your contact details and you will be ready to go.

#### Submitting the form

Submitting SNAP-R application is now straightforward. Verify everything and hit
`submit` button located at the very bottom of the form. Fill required information
and proceed. It shouldn't take long before approval.

Once your application will get status *Accepted** you can then preview it and you should see something like this:

> Acknowledgement Details  
>
> Title	Encryption Registration GAM1606 Accepted with ERN R111111  
> Type	Acknowledgement  
> Date of Message	05/31/2016  
> Reference Number	GAM0000  
>
> Content  
> Thank you for submitting the information in Supplement 5 to Part 742.  
> Your ERN is R111699.  
> Based on this submission you are authorized to export or reexport encryption
> products described in Section 740.17(b)(1) of the EAR and mass market encryption
> products described in Section 742.15(b)(1) of the EAR.  You are required to submit
> an annual self-classification report (Supplement 8 to Part 742) for these products
> pursuant to the requirements in Section 742.15(c) of the EAR.

Take a screen grab. That is what you need to submit to Apple when registering it
via iTunes Connect while answering **Export Compliance** questions.

![img](https://carouselapps-wpengine.netdna-ssl.com/wp-content/uploads/2015/11/Mac-App-Store-questions-and-answers-about-encryption.png)

### Additional resources

#### Community guides to filling SNAP-R forms

<!-- todo: link to self -->
* [How to legally submit application to Apple's App Store when it uses encryption (or how to obtain ERN)](https://pupeno.com/2015/12/15/legally-submit-app-apples-app-store-uses-encryption-obtain-ern/) - good article
* [Apple iTunes export restrictions on apps](http://tigelane.blogspot.co.uk/2011/01/apple-itunes-export-restrictions-on.html) - good article - *high contrast*
* [Mass Market Encryption CCATS Commodity Classification for iPhone Applications in 8 Easy Steps](https://www.zetetic.net/blog/2009/8/3/mass-market-encryption-ccats-commodity-classification-for-ip.html)

#### Additional resources that might help

* [EAR Controls for Items That Use Encryption](https://www.bis.doc.gov/index.php/policy-guidance/encryption) - official from bis.doc.gov
* [iPhone - Export compliance when outside the U.S](http://stackoverflow.com/questions/5633957/iphone-export-compliance-when-outside-the-u-s) - stackoverflow
* [CCATS on iOS AppStore and encryption](http://stackoverflow.com/questions/15770215/ccats-on-ios-appstore-and-encryption)
* [Most Mac and iOS applications are breaking the rules and could be removed, is yours?](https://carouselapps.com/2015/12/09/mac-ios-applications-breaking-rules-removed/)
