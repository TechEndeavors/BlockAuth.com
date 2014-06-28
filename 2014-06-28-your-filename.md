## User Verification procedures
When a user signs up at a BlockAuth Identity Registrar, they can enter a lot of information about themselves and choose what depth they want the Identity Registrar to verify. The results of those verifications are available to websites that understand how to implement the OpenID Connect OAUTH requests. 

### Email
Email verification is normally a plain and simple procedure, but we're adding a few additional steps in order to defeat automated bots. When a user initiates email verification, they are shown a word on their screen. The email that they receive has a link to the confirmation page, where they have to click the image matching that word. 

For instance, if they initiate an email verification they might be shown the word "Horse". When they click the link in their email, they'll be taken to a confirmation page where there will be several pictures, including one of a horse, and they'll be instructed to click on the picture that matched their word. 

An alternative method that is friendly to the blind needs to be developed.

Email addresses also have to be checked against a list of known single-use email providers such as mailinator. 


### Phone
When a user wishes to verify their SMS-capable mobile phone number, they will be shown a word on their screen. When they receive the SMS message, they will need to reply to the SMS with the word that was on their screen. 

Verification through landlines will be similar, but the user will be given a numeric number to punch in after an automated voice system calls them. 

Phone numbers should be run through a series of API’s to determine what carrier they use. Phone numbers that are from VoIP providers like Twilio or Plivo or Google Voice might get a lower score than ones that go directly to a cellphone or landline. 

###ID
The user is given three options for ID submission. 

Submission through a photo with their camera phone, a regular camera, and a flatbed scanner. 

For camera phones, the user is asked to take a picture of their ID at that moment and email it from their phone to a special email address created just for the process. For regular cameras, they are asked to take a photo and upload it without modification. Same with the flatbed scanner.

The images are checked for modification by looking at the EXIF headers, modification dates, and other metadata. Also, a database of JPG specifics will be generated for a range of cameras and phones to detect if an image might have the right EXIF tags, but has a different color profile or JPG compression level. 

The image will then be run through an Error Level Analysis (ELA) algorithm that evaluates the error level potential of a JPEG image. JPEG is a lossy image format; every resave degrades the picture. The amount of degradation varies based on the number of saves. 

When a picture is modified, the changed parts have a higher error level potential than the rest of the image. ELA works by saving the picture at a known quality level (like a JPEG at 95%), and then determines how much changed. Edits and splices appear as regions with more change. 

An employee that has gone through the online course about how to interpret ELA results will be tasked to look for signs of digital alteration. That human will also occasionally get images that are known to be fake to test their attentiveness and skills. 

If the image appears to be valid, then the data in the image is entered into the users profile as unverified and sent to a queue for other checks. 

That data is then run through the Interpol Stolen and Lost Travel Documents (SLTD) database (available to us through the name I-Checkit) to make sure the documents aren’t stolen. 

At this point, we can be somewhat sure that the images aren’t altered and the documents aren’t stolen, but it doesn’t exclude the possibility that the documents are simple forgeries. 

If there is access to databases to directly verify the documents, that check must be done. Otherwise, the confirmation of the document will have to be through a mixture of verifications of the individual and other information on their identity document. 

###Address
Users are allowed to enter multiple addresses and specify which are their residence, vacation address, work address, etc. 
Primary corroboration occurs when the address is seen on legitimate identification documents or other documents like  utility bills. 

In order for the address to be completly confirmed, verification that the user can receive mail at that address must occur. The easiest, but substantially expensive, way to accomplish this is to send them a postcard with a unique code that they have to enter into a web form once they receive it. 

Additional ways to increase the verification score of addresses is by simply googling the address to look for obvious commercial post office facilities, business addresses, hotels, and other things of that nature. That won’t necessarily invalidate the address, but it needs to be flagged with that data. Additionally, checks of online property ownership databases can help determine if an address is zoned for residential or commercial use and who the registered owner is.


