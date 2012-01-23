![](http://bendodson.com/_images/projects/phpmyopenid-thumb.jpg)

phpMyOpenID is a simple to use install routine for the popular [phpMyID](http://siege.org/phpmyid.php) library which allows you to host an [OpenID](http://www.openid.net/) server on your own hosting package! OpenID was designed to be a decentralised framework which means that you can keep your ID on any server - no single company will own it. However, most people tend to sign up with a site such as [myopenid.com](http://www.myopenid.com/) therefore putting all of the power into one single organisation (reminiscent of [Microsoft Passport](http://en.wikipedia.org/wiki/Windows_Live_ID)). Therefore, I looked for a way to run an OpenID server on my own machine so that I could be sure all of my details were being kept by someone I trusted; me!

After searching for a while, I came across phpMyID which I quickly set up and have been using ever since. However, there is no actual installation routine for phpMyID and I thought that the process of setting up would be incredibly daunting for some people (e.g. generating your own MD5 hashes, etc). I therefore created phpMyOpenID in order to be an easy to use way of getting the power and functionality of phpMyID, but with the ease of setting up an OpenID on a third party system.

After releasing version 1, I had a lot of feedback asking for me to edit the phpMyID script to enable multi-user support. I've now done this with version 2 which you can download below. The phpMyID script is relatively unaffected and therefore I can update phpMyOpenID very easily when new versions of phpMyID are released.

Installation
------------

This version of phpMyOpenID incorporates phpMyID version 0.9

To get it up and running, simply upload the phpmyopenid folder into the root of your website. You will probably need to set the permissions to write for the entire folder (though this will be changed back at the end of the installation). Then go to http://www.YOURDOMAIN.com/phpmyopenid/ - this should automatically redirect to the installation routine. Simply follow the instructions and you should be good to go.

To test it out, go to any OpenID enabled website such as LiveJournal or mag.nolia and login with your domain name.

Please note that the multi-user settings are for a single domain (e.g. multiple people can login to the account for one domain) - this script will not automatically generate subdomains or user folders although it could be easily modified to perform such tasks.

Disclaimer
----------

I'm not actively developing phpMyOpenID at the moment as I feel OpenID has been superseded to a certain degree by endeavours such as [Facebook Connect](http://developers.facebook.com/connect.php) which has been widely integrated into many websites and applications. However, should OpenID remain a dominant force in single-point logins, then I may well return to update this script. The code in this project is not good (very procedural) as I'd been planning on tidying it up and making it object orientated when I got to a v1.0 release (rather than this version 0.9). However, I still use this project personally to connect to a number of websites and felt that it might be useful to somebody.

License
-------

This work is licensed under a [Creative Commons Attribution 3.0 Unported License](http://creativecommons.org/licenses/by/3.0/).

