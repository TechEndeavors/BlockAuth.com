BlockAuth - OAUTH provider that performs Know Your Customer verifications
================================================================




The Legal Requirements
--------------------
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
