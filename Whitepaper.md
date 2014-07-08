#BlockAuth#
Powering a franchised network of OpenID Connect providers that verify user authentication AND authenticity




The Need
--------------------
There are many services that need a secure user authentication system who also need to be assured of the authenticity of every user. Authenticity isn't just verification that a user is who they claim they are, it's verification of the facts that the user chooses to assert about themselves. 

A user can make any claim about themselves from their gender, age, financial class, visa status, or citizenship. The verification providers in the BlockAuth network will verify any information possible to vouch for those assertations on behalf of that user. 

Some sites and services have common needs. Most likely they want to make sure the users on their platform are real people . Perhaps they want to restrict their platform to people who are not minors or are located in certain jurisdictions without specific legal entanglements. Other services might have more esoteric requirements like wanting to restrict their site to people with degrees from a certain university or certain genders or specific locales. 

Right now those sites and services have to do all of the verification work themselves. This is difficult, expensive, and the work that those sites do isn't shared with other services. By centralizing the verification tasks to third-party authorities, the services can have the verification costs and burdens eased. The users can also avoid having to repeat the same verification tasks with different services. 

The Competition
-----------------
There are several companies that offer verification services but they tend to just facilitate specific verification techniques. By not placing the ownership of the results in the users ownership, those services charge different sites and services the same costs for repeated verifications. 
**This is why BlockAuth is different from the existing services. The user has the ownership of the results of their authenticity verifications and can use that verification with any site that asks for it.**


Industry Impact
-----------------
The services that the BlockAuth providers will provide have tangible benefits from an extensive variety of industries from cryptocurrency exchanges to message boards to dating sites. For more, please see  https://github.com/BlockAuth/Planning/blob/master/Industry%20Opportunities.md


Open Source Throughout
-----------------------
BlockAuth believes strongly in the pricipals of the open source and the free software movement. In fact, most of the technologies that will power our work are existing open source projects that we're using to enable our services. 

Any use of open source projects will be clearly be advertised and we'll regularly engage the developers. Any projects that require modification will be forked and we'll work with the developers to have the changes merged back into the project. If a developer is hesistant of the changes that we've made, we'll try to find a compromise so the original open source project can continue to be the main focus of development. Only in very extreme cases will a forked project try to find a life of it's own. 

Additionally, BlockAuth will use it's financial resources to help developers of open source projects by paying grants or bounties. Financial incentives will be focused on the existing developers who have shown that they have a passion in their own project, but occasionally might be used to hire subject-specific experts to help the existing developers with certain specialities. An example would be hiring an expert on cryptography to help the developer of a login provider improve their hashing algorithms or hiring an expert on best-practices in API development add a modern standards-compliant API to an existing project. 

You can read more at https://github.com/BlockAuth/Planning/blob/master/Founding%20Ideals%20and%20Goals.md and see a list of proposed projects at https://github.com/BlockAuth/Planning/blob/master/Open%20Source%20Projects%20to%20Contribute%20to.md

Decentralization
-----------------
BlockAuth recognizes that many projects and services start out with the intentions of helping a community, but get mired in problems with politics, internal beucracy, or the self-interests of people involved. In order for this to be prevented, all employees will be held to a code of conduct. In addition, the organization will be run in a democratic fashion with all groups having a stake in the overall operations. 

There isn't currently a platform operational for a true decentralized management infrastructure of an organization like this, but BlockAuth will attempt to build one to the best of it's abilities. 

All franchise partners will be issued powers to vote on issues regarding BlockAuth. Some types of decisions will accept votes based on their holding of BlockAuth tokens, and some will be based on the principals of one-franchise, one-vote. For instance, a vote on an expensive marketing campaign to benefit all of the franchise partners is one that's related to money, so it would be based on the holdings of the franchise partners BlockAuth tokens. This allows the franchise partners with the most investment in the ecosystem to have a louder voice in it's financial operations. Votes regarding policy changes will often be based on one-franchise, one-vote. 

We need to make some more clear rules to determine when the different voting methods will be employed to make sure there isn't confusion. 

You can read more about our founding principals at https://github.com/BlockAuth/Planning/blob/master/Founding%20Ideals%20and%20Goals.md

BlockAuth Tokens
-----------------
After much thought, it's been determined that using an App Token, refered to as a BlockAuth Token, is in the best interests of this community. By purchasing tokens, it allows partners to channel funds to the BlockAuth organization early in order to help kick-start development of all of the technologies. In receiving the tokens, the partners maintain a stake in the operations and direction of the BlockAuth organization. The more tokens they hold, the more more powerful their voice is. 

Tokens also allow us to enable a fluid, functional, and secure marketplace for services between franchise partners that have been verified and approved to work with user data. This marketplace will allow partners with specialized verification technologies to outsource those services to the other franchise partners for a fee. In true capitalist fashion, popular but expensive verification processes will encourage partners to offer competing services for lower prices or with higher quality. 

You can read more about BlockAuth Tokens at https://github.com/BlockAuth/Planning/blob/master/Token%20Plans%20and%20Pricing.md

Franchise Requirements
----------------------
Franchises must adhere to the operational procedures set forth when they are licensed. Re-licensing is expected to take place every 6 months, and they will have to resign agreements with any changes to operational procedures in order to maintain their license. 

Some of the basic operational requirements involve keeping their software updated to the latest BlockAuth issued releases, meeting our code of conduct, allowing audits, responding to legal or governmental requests in the proper manner, and not having an unacceptable rate of mistakes of the validation process. 

If a verification service has a high rate of incorrect verifications, BlockAuth might commission a spot audit of a percentage of that work in order to determine if the franchise partner should lose their license or be asked to stop verifying the category of information that they are showing a deficiency in. 

If a franchise partner loses their license, their monthly membership fee is kept for the remainder of that month and they are still allowed to participate in the BlockAuth token marketplace, in order to sell their remaining BlockAuth tokens to other franchise holders. Any user account that they have conservatorship of will be seized by the BlockAuth foundation and will be placed on the marketplace for other franchise Identity Providers to purchase. The BlockAuth Tokens earned by the sales of these seized user accounts will be sold and the funds will be returned to the Identity Registrar

You can read more about the franchise program at https://github.com/BlockAuth/Planning/blob/master/Franchise%20Fees%20and%20Operating%20Costs.md

Project Status
-------------
BlockAuth has forked an existing OpenID Connect Provider software package and is making the necessary improvements to extend the metadata written into the standard to include additional data that can be passed along to any services that are configured to listen to them. We are currently in the process of altering the software to work with MongoDB in order to allow for proper storage of user information that fits our extended and flexible schema. 

There needs to be a lot more work done on the user interface side of the services. We've been building it with the API first. 

You can read more about the project status at https://github.com/BlockAuth/Planning/blob/master/Project%20Status.md 

You can read the summary of the technology that'll be integral to our platform at https://github.com/BlockAuth/Planning/blob/master/Technology%20Platform.md

You can also read more about how we intend to encourage other open source developers to take part by reading https://github.com/BlockAuth/Planning/blob/master/Developer%20Incentives.md


Privacy and Security
--------------------
One of the most important aspects of BlockAuth is how seriously we take users privacy and security. 

User privacy is entirely within the control of the users themselves by allowing them to choose what information they wish to make public, and to whom it'll be released.  Those disclosure settings will be able to be set on every page in an informative and easy manner and not hidden away in a hard-to-find "Privacy Settings" portion of their profile. 

Security of user data is also taken very seriously. All user data will be encrypted in various manners, depending on what kind of privacy settings the user lists. Information they wish to keep entirely private is encrypted with multi-part keys that require multiple parties to work in tendem to decrypt. Information the user wishes to share, but only with their approval, is kept encrypted in a form so raw access to the database doesn't result in any disclosures. 

In addition to using encryption, we'll be using best-practices that exceede industry standards. Not only will security be enabled through proper procedures, we'll use additional security-through-obscurity techniques and employ various "canary
profiles" and honey pots. All systems will be routinely checked by third-party auditors and bounties will be issued to the general public who wishes to take part in attempting to breech our systems. 

More about our security plans can be found at https://github.com/BlockAuth/Planning/blob/master/Security%20Practices.md

Flexible User Schemas
---------------------
The initial design will ask for common bits of information such as name, gender, age, social media links, location, etc. The BlockAuth systems are being designed to allow ANY information that users assert about themselves to be checked for authenticity if there is a verification partner willing to perform the checks. This allows for the system to grow to meet the needs of websites such as a forum for Air Conditioner repair only allowing licensed AC repairmen or an investment platform that only allows accredited investors to participate. 

More about our schema can be found at https://github.com/BlockAuth/Planning/blob/master/dossier_schema.json

Summary
--------
BlockAuth is not just building a business to verify user authenticity while also providing an easy-to-integrate authentication system, it's building the framework necessary to build an entire resiliant decentralized ecosystem to perform these tasks. The core technology is finally ready for the internet to take advantage of what's being offered and the industries that can take advantage of the platform are extensive. 


