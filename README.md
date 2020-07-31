# ![kukulhan](/resources/images/iknelia.png?raw=false)
The history of Mexico in natural disasters has been catastrophic if we talk about earthquakes.The project of 'Iknelia' we give a strategic solution so that people can help others who unfortunately were affected by this natural disaster.

Our solution is through a web or device mobile browser people can create campaigns help you through the analysis and understanding of the kind of people on Twitter (including retweets, publications, mentions and other responses) send a direct message to through this social network to invite you to be part of the campaigns that were created through Iknelia.

## Iknelia team proposes

Iknelia uses 6 different components:
1. [Front End: Polymer](SETUP.md#the-front)
2. [Back End: NodeJS](SETUP.md#the-back)
3. [No-SQL: MongoDB](SETUP.md#the-mongodb)
4. [API Twitter](SETUP.md#the-api-twitter)
5. [IBM Watson Assistant](SETUP.md#ibm-watson-assistant)
6. [IBM Cloud Kubernetes Service](SETUP.md#ibm-cloud-kubernetes-service)

And for future development we will develop ...
7. [IBM Watson Studio](SETUP.md#ibm-watson-studio)

## Diagram
# ![kukulhan](/resources/images/presentation.png?raw=true)

## Get started

* [Know us](#know-us)
* [Setting up the solution](#setting-up-the-solution)
* [How does our solution work?](#how-does-our-solution-work)
* [Which are the next steps?](#which-are-the-next-steps)
* [Technologies used](#technologies-used)
* [Authors](#authors)
* [Acknowledgments](#acknowledgments)


## Know us
Watch the video below to understand our solution:

## Setting up the solution
See [SETUP.md](SETUP.md)

## How does our solution work?

### Ask for help
Our application has the ability to create help through campaigns with people who want to help their community on our platform, in four categories:

* Debris
* Supplies
* Health
* Donation

# ![kukulhan](/resources/images/5.png?raw=true)

In these categories we analyze the data from Mexico City happened in the earthquake on September 19, 2017, which made international news and was affected many Mexican families.

For example, in the rubble category we detected that people on Twitter were retweeting and responding that a certain location needed tools and volunteers to remove the buildings that were destroyed by the earthquake.

The next step is that the user who has created your help campaign, can put all the information that it considers relevant, such as the address where they need help, the description of the need for the town and the duration of their campaign can be between 24 hrs. at 72 hrs.

# ![kukulhan](/resources/images/13.png?raw=true)

### Community on Twitter
**Twitter** has become the main means of citizen expression. Therefore, the analysis is important to observe the degree of citizen participation on news content on Twitter, based on the quantification of their interactions and interests of people. Through our platform we help these people to call new volunteers to support, and that Twitter searches for potential volunteers and sends them an invitation so they can contribute to the support. Twitter has also allowed activist groups to raise awareness and mobilize even those not affected by the cause of the activists. This search for the behavior of people on Twitter according to an analysis of key words interest and realized that the person uses in their social network. Businesses, organizations and even governments have used social networks to reach a broader and influence public behavior.

Therefore, we offer a solution to effectively target aid to all affected community. Providing the opportunity for people to create post-disaster social aid communities, with activist volunteers with a Twitter account without the need to create an account on this social network. Then, the user is asked to put hashtags that they considered relevant in the search. If the user has no idea how to put these hashtags, **IBM Watson assistant** will help in the process.

**This in order to help people who have never used a social network such as Twitter.**

Also, we took information and data regarding the earthquake of September 19 in Mexico City, which was one of the most affected areas. And according to our analysis, the most relevant hashtags:

**Relevant Hastags**

* #Sismo
* #19s
* #Ayuda
* #sismo19s
* #19septiembre
* #FuerzaMexico
* #AyudaSismo

And we detect the things that were most requested.

* Rubble collection
* Transport
* Nonperishable food
* First aid kits
* Construction tools
* Psychological help

Then we added three hashtags in the user campaign that we consider most relevant in relation to our analysis. These hashtags will later serve us to search for potential activists on Twitter.

# ![kukulhan](/resources/images/mongo_campaign.png?raw=true)

Finally, the user is informed that they have successfully created their campaign. And our platform will now be in charge of analyzing and searching for people on Twitter who are interested in offering their help and can segment and group these activists. Where us through the Twitter API, once identified these people, we send them an invitation by a direct message to their profile.

# ![kukulhan](/resources/images/api_twiter.png?raw=true)

## Which are the next steps?

## Technologies used

## Authors
* Hebert Velázquez
* Joatham Baez
* Saúl Rodríguez

## Acknowledgments
* We are grateful to IBM for allowing us to participate in this challenge where we learned throughout development. And we hope that regardless of our performance, we hope to contribute something to the community :)
