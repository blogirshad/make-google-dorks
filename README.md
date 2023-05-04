### Broad domain search w/ negative search

> site:example.com -www -shop -share -ir -mfa

### PHP extension w/ parameters

> site:example.com ext:php inurl:?

### Disclosed XSS and Open Redirects

> site:openbugbounty.org inurl:reports intext:"example.com"

### Juicy Extensions

> site:"example[.]com" ext:log | ext:txt | ext:conf | ext:cnf | ext:ini | ext:env | ext:sh | ext:bak | ext:backup | ext:swp | ext:old | ext:~ | ext:git | ext:svn | ext:htpasswd | ext:htaccess

### Code Leaks

> site:pastebin.com "example.com"

> site:jsfiddle.net "example.com"

> site:codebeautify.org "example.com"

> site:codepen.io "example.com"

### Cloud Storage

> site:s3.amazonaws.com "example.com"

> site:blob.core.windows.net "example.com"

> site:googleapis.com "example.com"

> site:drive.google.com "example.com"

> site:dev.azure.com "example[.]com"

> site:onedrive.live.com "example[.]com"

> site:digitaloceanspaces.com "example[.]com"

> site:sharepoint.com "example[.]com"

> site:s3-external-1.amazonaws.com "example[.]com"

> site:s3.dualstack.us-east-1.amazonaws.com "example[.]com"

> site:dropbox.com/s "example[.]com"

> site:box.com/s "example[.]com"

> site:docs.google.com inurl:"/d/" "example[.]com"

### XSS prone parameters

> inurl:q= | inurl:s= | inurl:search= | inurl:query= inurl:& site:example.com

### Open Redirect prone parameters

> inurl:url= | inurl:return= | inurl:next= | inurl:redir= inurl:http site:example.com

### SQLi Prone Parameters

> inurl:id= | inurl:pid= | inurl:category= | inurl:cat= | inurl:action= | inurl:sid= | inurl:dir= inurl:& site:example.com

### SSRF Prone Parameters

> inurl:http | inurl:url= | inurl:path= | inurl:dest= | inurl:html= | inurl:data= | inurl:domain=  | inurl:page= inurl:& site:example.com

### LFI Prone Parameters

> inurl:include | inurl:dir | inurl:detail= | inurl:file= | inurl:folder= | inurl:inc= | inurl:locate= | inurl:doc= | inurl:conf= inurl:& site:example.com

### RCE Prone Parameters

> inurl:cmd | inurl:exec= | inurl:query= | inurl:code= | inurl:do= | inurl:run= | inurl:read=  | inurl:ping= inurl:& site:example.com

### High % inurl keywords

> inurl:config | inurl:env | inurl:setting | inurl:backup | inurl:admin | inurl:php site:example[.]com

### Sensitive Parameters

> inurl:email= | inurl:phone= | inurl:password= | inurl:secret= inurl:& site:example[.]com

### JFrog Artifactory

> site:jfrog.io "example[.]com"

### Firebase

> site:firebaseio.com "example[.]com"

### API Docs

> inurl:apidocs | inurl:api-docs | inurl:swagger | inurl:api-explorer site:"example[.]com"

### File upload endpoints

> site:example.com ”choose file”

## Dorks that work better w/o domain

### Bug Bounty programs and Vulnerability Disclosure Programs

> "submit vulnerability report" | "powered by bugcrowd" | "powered by hackerone"

> site:*/security.txt "bounty"

### Apache Server Status Exposed

> site:*/server-status apache

### WordPress

> inurl:/wp-admin/admin-ajax.php

> site:example.com intitle:index of /wp-admin

### Drupal

> intext:"Powered by" & intext:Drupal & inurl:user

### Joomla

> site:*/joomla/login

### Using special search string to find vulnerable websites:
 
> site:example.com inurl:php?=id1

> site:example.com inurl:index.php?id=

> site:example.com inurl:trainers.php?id=

> site:example.com inurl:buy.php?category=

> site:example.com inurl:article.php?ID=

> site:example.com inurl:play_old.php?id=

> site:example.com inurl:declaration_more.php?decl_id=

> site:example.com inurl:pageid=

> site:example.com inurl:games.php?id=

> site:example.com inurl:page.php?file=

> site:example.com inurl:newsDetail.php?id=

> site:example.com inurl:gallery.php?id=

> site:example.com inurl:article.php?id=

> site:example.com inurl:show.php?id=

> site:example.com inurl:staff_id=

> site:example.com inurl:newsitem.php?num= andinurl:index.php?id=

> site:example.com inurl:trainers.php?id=

> site:example.com inurl:buy.php?category=

> site:example.com inurl:article.php?ID=

> site:example.com inurl:play_old.php?id=

> site:example.com inurl:declaration_more.php?decl_id=

> site:example.com inurl:pageid=

> site:example.com inurl:games.php?id=

> site:example.com inurl:page.php?file=

> site:example.com inurl:newsDetail.php?id=

> site:example.com inurl:gallery.php?id=

> site:example.com inurl:article.php?id=

> site:example.com inurl:show.php?id=

> site:example.com inurl:staff_id=

> site:example.com inurl:newsitem.php?num=

> site:example.com inurl: 1051/viewer/live/index.html?lang=en

> site:example.com inurl: inurl:"view.shtml" ext:shtml

> site:example.com inurl:"/?q=user/password/"

> site:example.com inurl:"/cgi-bin/guestimage.html" "Menu"

> site:example.com inurl:"/php/info.php" "PHP Version"

> site:example.com inurl:"/phpmyadmin/user_password.php

> site:example.com inurl:"servicedesk/customer/user/login"

> site:example.com inurl:"view.shtml" "Network"

> site:example.com inurl:"view.shtml" "camera"

> site:example.com inurl:"woocommerce-exporter"

> site:example.com inurl:/?op=register

> site:example.com inurl:/Jview.htm + "View Video - Java Mode"

> site:example.com inurl:/Jview.htm + intext:"Zoom :"

> site:example.com inurl:/adfs/ls/?SAMLRequest

> site:example.com inurl:/adfs/ls/idpinitiatedsignon

> site:example.com inurl:/adfs/oauth2/authorize

> site:example.com inurl:/cgi-bin/manlist?section

> site:example.com inurl:/eftclient/account/login.htm

> site:example.com inurl:/homej.html?

> site:example.com inurl:/index.html?size=2&mode=4

> site:example.com inurl:/pro_users/login

> site:example.com inurl:/wp-content/themes/altair/

> site:example.com inurl:/xprober ext:php

> site:example.com inurl:RichWidgets/Popup_Upload.aspx

> site:example.com inurl:Sitefinity/Authenticate/SWT

> site:example.com inurl:adfs inurl:wctx inurl:wtrealm -microsoft.com

> site:example.com inurl:authorization.ping

> site:example.com inurl:https://trello.com AND intext:@gmail.com AND intext:password

> site:example.com inurl:idp/Authn/UserPassword

> site:example.com inurl:idp/prp.wsf

> site:example.com inurl:login.seam

> site:example.com inurl:nidp/idff/sso

> site:example.com inurl:oidc/authorize

> site:example.com inurl:opac_css

> site:example.com inurl:weblogin intitle:("USG20-VPN"|"USG20W-VPN"|USG40|USG40W|USG60|
