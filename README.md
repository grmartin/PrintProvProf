# PrintProvProfCerts

This is a simple project in the form of a [PHP](http://php.net) Script that allows the user to simply print out the security information in an Apple iOS [Provisioning Profile](https://developer.apple.com/library/mac/documentation/IDEs/Conceptual/AppStoreDistributionTutorial/CreatingYourTeamProvisioningProfile/CreatingYourTeamProvisioningProfile.html#//apple_ref/doc/uid/TP40013839-CH33-SW1). Allowing a user to know what certificates were used in the creation of it.

This project hasn't needed any real work since its creation and thus I am simply providing the files here for general use by everyone.

This project is licensed under the 3-clause BSD License found in the ```./LICENSE``` file.

This script is meant to be used locally on your Mac by a trusted user, it does make a couple of shell level execution calls.

It is also [available](https://github.com/grmartin/PrintProvProf/releases) in self-executable [PHAR](http://php.net/manual/en/book.phar.php) form. Which I will make available along side this repository.

## Execution
Execution is rather simple, the script takes on argument, the path to a Provisioning Profile.

	cfkane:myproject grmartin$ ~/Scripts/PrintProvProfCerts /Users/grmartin/Desktop/profile.mobileprovision 
		Verification successful
		Certificate:
		    Data:
		        Version: 3 (0x2)
		        Serial Number:
		            70:47:a7:09:68:XX:XX:XX
		        Signature Algorithm: sha1WithRSAEncryption
		        Issuer: C=US, O=Apple Inc., OU=Apple Worldwide Developer Relations, 	CN=Apple Worldwide Developer Relations Certification Authority
		        Validity
		            Not Before: Aug 20 03:05:11 2014 GMT
		            Not After : Aug 20 03:05:11 2015 GMT
		        Subject: UID=9V6XXXXBPL, CN=iPhone Distribution: Some Company, Inc. (9V6XXXXBPL), OU=9V6XXXXBPL, O=Some Company, Inc., C=US
		        Subject Public Key Info:
		            Public Key Algorithm: rsaEncryption
		            RSA Public Key: (2048 bit)
		                Modulus (2048 bit):
		                    00:d1:xx:d0:c6:4a:b7:18:ba:a9:d4:63:74:2a:e4:
		                    xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:
		                    xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:
		                    xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:
		                    xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:
		                    xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:
		                    xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:
		                    xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:xx:

		... <truncated for brevity> ...
