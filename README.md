ise-bootstrap
=============

A responsive portal theme for Cisco ISE, powered by bootstrap

# Installation

* Download the files :)
* On Cisco ISE, create a custom portal
 * Administration -> Web Portal Management -> Settings -> Guest -> Multi-Portal Configuration
 * Call it "myportal"
 * Select "Custom Default Portal (_upload files_)"
* upload the files to the portal
* map the files
 * Login file -> login.html
 * AUP file -> aup.html
 * Change Password file -> cpass.html	 
 * Self Registration file -> selfreg.html
 * Self Registration Results file -> selfsuc.html
 * Device Registration file -> _fixme_
 * Guest Success file -> sucess.html
 * Error Page file 	-> err.html
* Set your authentication to the correct sequence
* create an authorization result to the new portal
* update your authorization rule to point to new result!

# Notes for Customisation

To test changes locally on your harddisk without uploading to ISE, included is `dev.bootstrap.min.css`; in the file you are testing...

Replace

```
<link href="portals/myportal/bootstrap.min.css" rel="stylesheet" type="text/css" />
<!--  <link href="dev.bootstrap.min.css" rel="stylesheet" type="text/css" /> -->
```

With

```
<!-- <link href="portals/myportal/bootstrap.min.css" rel="stylesheet" type="text/css" /> -->
<link href="dev.bootstrap.min.css" rel="stylesheet" type="text/css" />
```

This will allow you to view the page properly in your browser on your machine

# To change the portal name from "myportal" to "foobar"

* Goto http://twitter.github.io/bootstrap/customize.html
* Change @iconSpritePath to 'portals/foobar/glyphicons-halflings.png'
* Change @iconWhiteSpritePath to 'portals/foobar/glyphicons-halflings-white.png'
* change any links in your html

# MISC

HTML Src: http://www.cisco.com/en/US/docs/security/ise/1.1.1/user_guide/ise_guest_pol.html
