# Your Plex server is like a restaurant 

A. `Kitchen = Plex server`: It needs to take high quality ingredients (the original video) and prepare them in large aluminum trays that still looks fancy. This is complicated and labor intensive

B. `Delivery service = internet`: Even if you hire a high end catering restaurant and have a mansion to serve it in, you need a large vehicle to transport all of the food at once. 

  - If your delivery service has a massive truck, you can typically everything you need right away. This is analogous to the server's **upload speed**

  - However, even if the large quantity of food comes by a large truck, you'll need an efficient way of getting the food off the truck and into your dining room. This is analogous to **download speed**. 


C. `Your home = your client (ex: PC, phone, Firestick, Apple TV)`: You need to be able to take large quantities of food delivered to you in aluminum trays and serve them to all of your guests at the party. Some foods are easy to serve (think finger food appetizers) while others are complicated (well plated dinners). This is analogous to **decoding the video**. 

----


# **Are you dining in? This is like watching stuff "in house" or where the server is physically located --> LAN playback**

Here you get all of the best service. The restaurant can almost always keep up with your needs

* **Speed is fast** because the waiter needs to travel a very short distance to go from the kitchen to your table  
* **Quality is great** because the food is plated perfectly from the kitchen. No need to package it in smaller to-go containers (uncompressed Direct Play)

---- 

# **Are you ordering delivery/catering?**

Here things get tricky depending on:
   
* Restaurant's kitchen capabilities  
* Delivery service capabilities  
* Your home's capabilities  

Let's go over some of the possibilities:

**~Catering a feast**  
You want the high end food, a large quantity all at once, and you want it delivered. So you'll need a kitchen that can prepare a lot of high-end food, a large truck to deliver it, and enough plates at your house to serve the food on. 

- Good server
- Fast server upload speed
- Fast client download speed
- A great client that can play back basically anything (Shield, ATV, Firestick 4K, iPhone X and new, etc)


What happens when you want a feast catered, but you don't have a truck?  

`4k HEVC--> 4k playback on ethernet in the same house`

* If your delivery service is a motorcycle, expect to get a tiny amount of food...wait...some more food...wait...some more food... wait. This is analogous to **buffering due to the server not having enough upload bandwidth**
* If your get a large truck to deliver stuff to your house, but you've got cars blocking the driveway and you send your uninterested children to help carry stuff into the kitchen, this is analogous to **buffering due to the client not having enough bandwidth**


**~Delivery meal to your home for one when you're really starving**

`1080p HEVC --> 1080p HEVC on WiFi in another house`

You've ordered the most common dish and the restaurant already has it ready to go. A large SUV is ready to take the order to you (great internet speeds from both uploader and downloader). Most importantly, you're so hungry, you'll eat it right out of the box. No need to take it out and plate it properly. You're not picky and you'll take anything. (Great client that can play back any codec).
 

**~Delivery meal to your home for one when you're a little hungry**

`1080p HEVC --> 480p x264 on WiFi in another house`

The restaurant has a lot of raw ingredients, but you ask for a single meal. So it tries to quickly takes one of each ingredient and whips up something in seconds. It sends it by motorcycle, which can navigate through traffic easily and come right to your door (good upload and download bandwidth). You're ready to open the container and plop the food on a plate (good client). You got the small sized food you wanted and you got it fast. 


However, the kitchen needs to be able to take a huge refrigerator of raw ingredients, cook each in small quantities, and package it nicely. There's only so many orders like this it can take at once before the kitchen gets overwhelmed. But with small orders, it can typically keep up

**~Delivery meal to your home for a family of 4**

`1080p --> 720p on WiFi in another house`

Similar to delivering to your home for one, but scaled up. The kitchen needs to prepare more meals, put them into to-go containers, all ready to go at once. You'll also need a larger vehicle like a car to carry the order (better upload and download speeds). And you'll need someone in the family who can serve the food fast enough for those hungry mouths (good client). 

This becomes more work for the kitchen and more work for the delivery service. You've probably got someone at home who's good at serving the food for just 4 people, so no issues there. 


**~Delivering a small meal to the back of your minivan cruising down the highway**

`1080p --> 320p playback on a cell phone`

As you can imagine, ordering something from a restaurant, and expecting a delivery service to hand off the food to you while zooming down the highway is a difficult delivery request. But your restaurant is understanding that you're a busy family and always on the move, so it tries to accommodate.

The kitchen will make bite sized food that's small enough to put in tiny containers which fit in a backpack. It will race them to you on a motorcycle which can race off to find you, and hand it off to you through the window. The kitchen can whip up these tiny meals relatively easily, but getting them to you is the hard part. People are typically great at eating bite sized finger foods though (good clients).

**~Carrying out a gormet meal to eat on a plane**
`1080p --> 1080p Plex Pass sync`
You're the kind of person who likes to dine in style even when you're on the go, so you plan ahead. You place an order a day early to the restaurant for some good food. Delivery times are irrelevant because you offer to pick it up yourself when you get off work. And you'll be able to eat this flying at 35,000 feet, where there are no restaurants around to order from. This is analogous to *sync/download* (a Plex Pass feature). 

Here you can have the kitchen prepare you high quality stuff and you take the responsibility of the transfer and remote plating. Sync/Downloads is wonderful because you can have high quality videos, even without internet, if you're okay with not having it "on-demand". You need to request the download, have the Plex server prepare it, and download the file. This means you have to plan head of time and have a Plex server that is capable of offering this service to you (this is a paid Plex Pass feature).


# Plex is an amazing service because the server (like a restaurant's kitchen) will analyze the entire process and try to make the best decision for good delivery. It predicts where the choke points will be and plans accordingly. 

Sometimes, though, Plex takes an order that's more than it can handle. This is like 

**~Delivering a meal to your home for an extended family of 15**

`1080p HEVC 10Mbps to 1080p x264 20Mbps`

The kitchen is unable to package so many meals in to-go boxes. On top of that, the Uber eats delivery guy doesn't have enough space in his tiny car to fit the food. There are multiple problems here. The kitchen won't be able to serve anyone else food while it works on your order. The restaurant's delivery guy is overwhelmed and late on the other orders. This is when the transcoding is too much for the server's hardware, and the file size is too much for the internet bandwidth available. 

**~Delivering food in smaller containers because it thinks there's too much traffic on the road for an SUV**
`1080p 10Mbps to 720p x264 2Mbps`

Here we have the unfortunate most common issue with Plex. It assumes that somewhere along the delivery chain, something will get backed up. So let's play it safe and give you decent quality food, but we'll cut some corners on the meal sizes so that we can get it to you on a motorcycle. The default settings on Plex are made to assume this. If you let Plex automatically adjust qualilty, it will play it even safer and often make the quality lower, in it's effort to get you what you want ASAP. However, all of this means a lot more work for the kitchen (Plex server).

# Being a responsible patron of the restaurant / Plex

1. Talk to the owner and ask them what settings you should use
2. Only order as much as you can eat and don't clean the restaurant out 
3. Don't be a picky client.  Use a client that can consume whatever the server gives it in whatever format.
