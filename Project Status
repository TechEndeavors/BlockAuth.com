OpenID Connect Infrastructure
------------------------------
BlockAuth has identified the core software to power the OpenID Connect login provider networks. 
https://bitbucket.org/PEOFIAMP/phpoidc

We have installed it on several test servers and verified that it works well and also that the different identity registrars will be able to use it in a manner where users can log in at ANY BlockAuth Identity Provider and the results of their verifications will be able to be passed. 

There are some changes that we want to make to the software. 

We want to make sure that it runs on cloud application platforms, like Google AppEngine or Elastic Beanstalk, in order to make it so our franchise partners can operate it with less of a need to hire system administrators to handle the difficulties of growth and server resources. 

We also want to make the software work with a NoSQL database backend rather than the relational database backends that it currently supports. Because our users can assert any number of facts about themselves and request that they be authorized, it makes sense to use NoSQL databases to store user profiles rather than creating unweildy database tables. During the beta period, we'll limp along with a relational database structure until this work can be completed. 

User Interface Software Package
------------------------------------
The OpenID Connect Server package does not have a friendly user interface. Very few of the open source ones do. One is being built in Laravel, but it isn't ready for primetime and needs the expertise of a seasoned Laravel developer. 

This is the interface that the end user sees when they decide to create a BlockAuth compatible account. It needs to be easily themed so our franchise partners can give their system it's own "flavor" and branding. Whenever a user signs into a site, they'll be redirected to either a page or a popup dialog asking them to log in (if they aren't already) and if it's a new site to them, it'll ask them for the information the site is requesting for their approval or modification. That interface is also powered by this. 

This software package also lets users log in and enter their information, choose what they want verified, manage their account, and use additional features such as the micropayment system and privacy enhancement options that the Identity Provider wishes to operate. 

This software also be built to run on a cloud platform. It will talk to the API of the User Data Management System, as well as other API's to things like the email system to provide private email addresses or the wallet system to provide micropayment services. 


User Dossier Storage System
---------------------------
This software package operates as the API that several different components use to access user data. 
