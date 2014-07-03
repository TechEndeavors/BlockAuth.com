BlockAuth - A network of OpenID Connect providers that verify user authentication AND authenticity
================================================================




The Need
--------------------
There are a multitide of groups that need the ability to not just provide a secure user authentication system but also need to be assured of the authenticity of every user. Authenticity isn't just verification that a user is who they claim they are, it's verification of the facts that they choose to assert about themselves. 

If a user claims that they are a certain gender, age, ethnic group, financial class, or citizen of a certain country, we want to be able to vouch for those assertations on behalf of that user. 

Some sites and services have common needs, like the desire to only allow real people on their platform or to restrict their platform to people who are not minors or who are located in certain jurisdictions with legal entanglements. Other services might have more esoteric requirements, like wanting to restrict their site to people with degrees from a certain university or certain genders or specific locales. 

Right now, those sites and services have to do all of the verification work themselves. This is difficult, expensive, and the work that those sites do isn't shared with competing or non-competing services. By centralizing the verification tasks to a third-party authority, the services can have the verification costs and burdens eased. The users can also avoid having to repeat the same verification tasks with different services. 

The Competition
-----------------
There are several agencies that offer verification services, but they tend to just allow sites and services to lower their verification costs. By not placing the ownership of the results in the users ownership, those services  charge different sites and services the same costs for repeated verifications. Additionally, they don't provide authentication outsourcing. 
*That's what makes BlockAuth different from the existing services. The user has the ownership of the results of their verification tasks and can use that verification with any site that will accept it. *

Open Source Throughout
-----------------------
BlockAuth believes strongly in the pricipals of the open source and the free software movement. In fact, most of the technologies that will power our work are existing open source projects that we're using to enable our services. 

Any use of open source projects will be clearly be advertised and we'll regularly engage the developers. Any projects that require modification will be forked and we'll work with the developers to have the changes merged back into the project. If a developer is hesistant of the changes that we've made, we'll try to find a compromise so the original open source project can continue to be the main focus of development. Only in very extreme cases will a forked project try to find a life of it's own. 

Additionally, BlockAuth will use it's financial resources to help developers of open source projects by paying grants or bounties. Financial incentives will be focused on the existing developers who have shown that they have a passion in their own project, but occasionally might be used to hire subject-specific experts to help the existing developers with certain specialities. An example would be hiring an expert on cryptography to help the developer of a login provider improve their hashing algorithms or hiring an expert on best-practices in API development add a modern standards-compliant API to an existing project. 


Decentralization
-----------------
BlockAuth recognizes that many projects and services start out with the intentions of helping a community, but get mired in problems with politics, internal beucracy, or the self-interests of people involved. In order for this to be prevented, all employees will be held to a code of conduct. In addition, the organization will be run in a democratic fashion with all groups having a stake in the overall operations. 

There isn't currently a platform operational for a true decentralized management infrastructure of an organization like this, but BlockAuth will attempt to build one to the best of it's abilities. 

All franchise partners will be issued powers to vote on issues regarding BlockAuth. Some types of decisions will accept votes based on their holding of BlockAuth tokens, and some will be based on the principals of one-franchise, one-vote. For instance, a vote on an expensive marketing campaign to benefit all of the franchise partners is one that's related to money, so it would be based on the holdings of the franchise partners BlockAuth tokens. This allows the franchise partners with the most investment in the ecosystem to have a louder voice in it's financial operations. Votes regarding policy changes will often be based on one-franchise, one-vote. 

We need to make some more clear rules to determine when the different voting methods will be employed to make sure there isn't confusion. 

BlockAuth Tokens
-----------------
After much thought, it's been determined that using an App Token, refered to as a BlockAuth Token, is in the best interests of this community. By purchasing tokens, it allows partners to channel funds to the BlockAuth organization early in order to help kick-start development of all of the technologies. In receiving the tokens, the partners maintain a stake in the operations and direction of the BlockAuth organization. The more tokens they hold, the more more powerful their voice is. 

Tokens also allow us to enable a fluid, functional, and secure marketplace for services between franchise partners that have been verified and approved to work with user data. This marketplace will allow partners with specialized verification technologies to outsource those services to the other franchise partners for a fee. In true capitalist fashion, popular but expensive verification processes will encourage partners to offer competing services for lower prices or with higher quality. 

When a franchise partner is used to verify a specific piece of information, that piece of information is digitally signed and placed in the users dossier so all verifications can be traced back to who performed the work. BlockAuth itself will audit the work of verification partners through various means like submitting fake information for verification or having a franchise partner submit information to more than one verification service in order to look for discrepencies.  

Franchise Requirements
----------------------
Franchises must adhere to the operational procedures set forth when they are licensed. Re-licensing is expected to take place every 6 months, and they will have to resign agreements with any changes to operational procedures in order to maintain their license. 

Some of the basic operational requirements involve keeping their software updated to the latest BlockAuth issued releases, meeting our code of conduct, allowing audits, responding to legal or governmental requests in the proper manner, and not having an unacceptable rate of mistakes of the validation process. 

If a verification service has a high rate of incorrect verifications, BlockAuth might commission a spot audit of a percentage of that work in order to determine if the franchise partner should lose their license or be asked to stop verifying the category of information that they are showing a deficiency in. 

If a franchise partner loses their license, their monthly membership fee is kept for the remainder of that month and they are still allowed to participate in the BlockAuth token marketplace, in order to sell their remaining BlockAuth tokens to other franchise holders. Any user account that they have conservatorship of will be seized by the BlockAuth foundation and will be placed on the marketplace for other franchise Identity Providers to purchase. The BlockAuth Tokens earned by the sales of these seized user accounts will be sold and the funds will be returned to the Identity Registrar


Project Status
-------------
BlockAuth has identified the core software to power the OpenID Connect login provider networks. We have installed it on several test servers and verified that it works well and also that the different identity registrars will be able to use it in a manner where users can log in at ANY BlockAuth Identity Provider and the results of their verifications will be able to be passed. 

There are some changes to be made that require expertise. Right now, the software 

Old Whitepaper
Anytime digital currency is exchanged for fiat currency (USD, Euro, etc), regulations in many countries and jurisdictions require that those money exchangers follow several rules. 

The first one, Know Your Customer (KYC), refers to the due diligence financial institutions are required to perform on their customers as an aspect of doing business. In order to comply with federal regulations surrounding financial fraud, money laundering, identity theft, and terror financing, Bitcoin companies that convert digital currencies to some other kind of asset (such as physical cash) are required to verify their customers by instituting policies on customer acceptance and transactions.

The other rule that's important is FinCen's Anti-Money Laundering (AML) compliance. 
AML compliance requires companies to monitor and report any suspicious activity or transactions over $2000 if they are relevant to a possible violation of law or regulation. Companies also have to keep records of the transactions, including the amount, date and time, account information, IP address, etc. Also, similar regulations require reporting any accounts that transact over 10k a day, as well as preventing transactions coming from any countries that the US has sanctions against (Burma, Cuba, Iran, Libya, North Korea, Sudan, and Syria). 

This kind of compliance causes a lot of problems for small startups. First of all, it causes customer friction. Customers don't like to have to input all this information, especially over and over with different sites. It also requires startups to spend a lot of time and resources engineering safe ways to process and store this information. It's also expensive because it often requires them to hire a full-time employee to verify the information. Another danger is that if a startup makes a mistake in how they store this information and the site is breached, it's often the end of that company since they'll lose customer loyalty as well as have to pay for expensive credit monitoring for all of their customers. 

Overview of range of services
-------------------------
The answer is BlockAuth. BlockAuth is a service that to meet the KYC & AML requirements needs of bitcoin sites, as well as a service that protects the privacy of the end users and provides a convenient accounting system for them. It also functions as a way to ensure that users on sites don't have multiple accounts to astroturf or to scam other users. 

Our primary service offering is that we'll function as an OAUTH provider. All member sites have to do add a little snippet on their website and users can log in with BlockAuth just like how some sites let people login with their Google Account or Facebook Connect. 

At a minimum, the member site will always get a user identifier that will always be unique for the relationship between that user and that site (sites can use this as the user identifier), and the Auth Score the user has. Other information can be requested such as the users phone number, the complete or portions of the mailing address, email address, profile photo, links to social media, etc. The user ultimately has the choice to allow or disallow that information to be passed to the member site. 

In order to build up their Auth Score, end users will go to our site to fill out their information. We perform KYC checks on everything and provide encouragement to the users to verify more and more to increase their Auth Score. 

Some member sites will require a minimum Auth Score to use their services, such as an online merchant might require users to have a verified phone number and postal address. A loan provider might require that the end user have a verified source of income, address, and drivers license scanned. A travel agency might require the end user to have a scanned passport page. BlockAuth will tell the member sites if the end user has those things verified. 

How to decentralize
-----------------
The bitcoin ecosystem desperately needs someone to validate users, but it also needs to not be totally reliant on a central authority. This project intends to use the Mastercoin protocol to store our certification of BlockAuth's verification of a users KYC documentation

One way to accomplish this is by creating a new Mastercoin Smart Property (Transaction type 50). When a smart property is created, it's owned by the address which broadcast the transaction. That address will always be the BlockAuth address. 

Let's say that the address that created this mastercoin is 1KZmDQGzGJWYmPP9X3b7TA9d1234567890

- Property Category = "Authentication\0"
- Property Subcategory = "login.blockauth.com\0" (used to designate what OAUTH server to hit)
- Property Name = "UNASSIGNED-8ab28c77\0"
- Property URL = "UNASSIGNED-8ab28c77.blockauth.com\0"
- Property Data = "pd1,pd2,pd3+,pd4,pd5,ce1+,ce2,cd3,cp1+,cp2,cp5,\0"
- Number Properties = 7941


Once the smart property is created it'll be assigned a property ID (let's say it's 5481) by the mastercoin network, then a second transaction will occur to UPDATE the smart property to this:


- Property Category = "Authentication\0"
- Property Subcategory = "login.blockauth.com\0" (used to designate what OAUTH server to hit)
- Property Name = "5481\0"
- Property URL = "5481.blockauth.com\0"
- Property Data = "pd1,pd2,pd3+,pd4,pd5,ce1+,ce2,cd3,cp1+,cp2,cp5,\0"
- Number Properties = 7941



The configuration of this smart property will tell sites that if they have a "Login with BlockAuth" button that points to the OAUTH provider at login.blockauth.com, a user will be able to login and if the OAUTH provider returns 5481 as the user ID, they have been verified. 

The property data field includes a parsable set of boolean values that can be used to indicate various levels of user compliance and verification and preferences. The property URL indicates the location a website can go to the get the profile data the user wishes to make public. The direct URL will be a HTML webpage, but appendinging /json or /xml to the URL will give the data in other formats. 

The number properties field will be something of a "trustability" score. This will allow some websites to make quick instant decisions about letting users login or sign up. The algorithm to generate this score is not yet known. 

What's great about this system is that if the user is ever unhappy with BlockAuth, they can request their profile to be moved to another provider, like medical charts. The token can be transfered to another provider who replaces the Property Subcategory and Property URL settings. 

BlockAuth will also have a wind-down business plan that guarantees that the private keys that control the address that owns all the tokens is split up among a few trusted members of the community. If the service ever has to disolve, and there is an alternative service available, all of the authentication tokens can be transfered.

Since property subcategories can be sorted by popularity, this will allow sites to write an OAUTH login display that lets users login with the top 3 login providers on the Mastercoin network or manually enter their provider. This will result in the first mover advantage making BlockAuth at the top of the list, but it also lets other players enter the market.  
