##How Users Can Control Their Privacy##

###How we treat security and data protection###
BlockAuth believes in the principals of over-engineering when it comes to data security. We use standards based on analyzing the technology, not necessarilly the popularity of the implementation. 

Data that is meant to be in cold storage is encrypted with multi-part encryption keys with different independant groups holding the keys. 

Data that is meant to be secured, but able to be decrypted for use is encrypted with a method where the users password can decrypt the data, but also an off-server key held by the site can be used in the event of the user needing to reset their password. 

Regular data is kept encrypted with the decryption keys stored in server memory so it can be accessed through software. In the event of server reboot, the datastore is unavailable until the decryption key can be loaded. 

###Helping Users Choose the Right Settings###
The site generates some basic data templates for users with what we consider reasonable requests for information. Users can make their own data templates and assign them to different sites that ask for their information, or they can make a custom data template for specific sites. Those data templates can also be set to allow access from the general public of through a secret URL. 

*Examples*
* _Forums Basic Data Template_: email address, desired nickname, profile image, age, and location at city level
* _Forums Advanced Data Template_: Same as _Forums Basic Data Template_ but also includes links the users social media sites
* _Dating Site Data Template_: email address, desired nickname, age, gender, location at city level, educational achievement, job position
* _Shopping Site_: Name, email address, physcal address

Users can also generate time-limited secret URL's to display data about themselves they want to be able to advertise. These pages can either show the exact information or a redacted hint of the information, and the status of verification about any of those bits of information. 

Users can also have a public profile with the same settings at a friendly URL. They can choose to enable discovery via a search engine or not. 

