# ![kukulhan](/resources/images/iknelia.png?raw=false)
Mexico has had a tragic experience when it comes to earthquakes. Proof of this have been the earthquakes of September 19, 1985 and 2017. In which the importance of timely and efficient aid was noted. The project of 'Iknelia' we give a strategic solution so that people can help others who unfortunately were affected by this natural disaster.

‘Iknelia’ was born as a strategic solution to improve the way that people send their help to others who unfortunately has been affected by natural disasters as earthquakes.  ‘Iknelia’ is based on a web/ device mobile browser through people can design and accomplish campaigns whose objective is to send efficient aid to vulnerable groups. Iknelia is able to link potential helpers with the most affected, avoiding a saturation of unnecessary supports in the same affected groups. To achieve this, our solution analyzes the data found on Twitter such as retweets, publications, mentions, hashtags, etc. After analyzing the data, Iknelia sends a direct message to Twitter to boost aid.

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

[![](https://img.youtube.com/vi/fGjvKrDrlg4/0.jpg)](https://www.youtube.com/watch?v=fGjvKrDrlg4)

Demo project

[![](https://img.youtube.com/vi/2WI9CHF4hOg/0.jpg)](https://www.youtube.com/watch?v=2WI9CHF4hOg)

## Setting up the solution
See [SETUP.md](SETUP.md)

## How does our solution work?

### Ask for help
Our application is able to send efficient help to the victims by earthquakes throught campaigns designed on our platform. We have 4 categories..

* Debris
* Supplies
* Health
* Donation

# ![kukulhan](/resources/images/5.png?raw=true)

Those categories we analyze the Mexico City data happened in the earthquake on September 19, 2017, which made international news and was affected many Mexican families.

For instance, in the rubble category we detected that people on Twitter were retweeting and responding that a certain location needed tools and volunteers to remove the buildings that were destroyed by the earthquake.

The next step is that the user who has created your help campaign, can put all the information that it considers relevant, such as the address where they need help, the description of the need for the town and the duration of their campaign can be between 24 hrs. at 72 hrs.

# ![kukulhan](/resources/images/13.png?raw=true)

### Community on Twitter
**Twitter** has become the main means of citizen expression. Therefore, the analysis is important to observe the degree of citizen participation on news content on Twitter, based on the quantification of their interactions and interests of people. Through our platform we help these people to call new volunteers to support, and that Twitter searches for potential volunteers and sends them an invitation so they can contribute to the support. Twitter has also allowed activist groups to raise awareness and mobilize even those not affected by the cause of the activists. This search for the behavior of people on Twitter according to an analysis of key words interest and realized that the person uses in their social network. Businesses, organizations and even governments have used social networks to reach a broader and influence public behavior.

Therefore, we offer a solution to effectively target aid to all affected community. Providing the opportunity for people to create post-disaster social aid communities, with activist volunteers with a Twitter account without the need to create an account on this social network. Then, the user is asked to put hashtags that they considered relevant in the search. If the user has no idea how to put these hashtags, **IBM Watson assistant** will help in the process.

# ![kukulhan](/resources/images/watson.png?raw=true)

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

Then we added three hashtags in the user campaign that we consider most relevant in relation to our analysis. These hashtags will later serve us to search for potential activists on Twitter.

# ![kukulhan](/resources/images/mongo_campaign.png?raw=true)

Finally, the user is informed that they have successfully created their campaign. And our platform through algorithms will analyze and search for people on Twitter who are interested in offering their help and can segment and group these activists. Where us through the **Twitter API**, once identified these people, we send them an invitation by a direct message to their profile.

# ![kukulhan](/resources/images/api_twiter.png?raw=true)

Our application saves the users that have been selected by our analysis. Users are grouped depending on the type of help and it is related to the message sent.

# ![kukulhan](/resources/images/mongo_message.png?raw=true)

At last, the users can see all campaign from other people. And these people can be sympathizers with the aid. We provide them with contact information for the person who created the aid campaign.

# ![kukulhan](/resources/images/23.png?raw=true)

### Data science: Natural Language Processing (NLP)

The topic we choose, our tone, our selection of words, everything adds some type of information that can be interpreted and value extracted from it. In theory, we can understand and even predict human behaviour using that information. But there is a problem: one person may generate hundreds or thousands of words in a declaration, each sentence with its corresponding complexity. Nevertheless, thanks to the advances in disciplines like machine learning a big revolution is going on regarding this topic.

Natural Language Processing or NLP is a field of **Artificial Intelligence** that gives the machines the ability to read, understand and derive meaning from human languages. It is a discipline that focuses on the interaction between data science and human language, and is scaling to lots of industries.

We cleaned the data, and it was possible to identify the relevant words. With this we discovered that it is the most requested as aid related to an earthquake and we also segment hashtags related to these requests. Furthermore, We also identify who the interested people are to help, and how the support roles interact. We finally identify the categories of help and that this helped us to implement it in our project.

* Rubble collection
* Transport
* Nonperishable food
* First aid kits
* Construction tools
* Psychological help

Our development at Jupyter, see [earthq_data.ipynb](/data/earthq_data_analyst.ipynb)

## Which are the next steps?

### In the future, we are aiming to do:

- [ ] Monitor the behavior of people on Twitter in real time, with the implementation of **IBM Watson Studio** using our analytical model of data in the cloud.
- [ ] Explore other natural disasters that our platform can help (hurricane or wildfire)
- [ ] Deploy the project in the cloud with **IBM Cloud Kubernetes Service**, because our project is already compiled with **Dockers** in our local environment.

### Longer term goals are:

- [ ] Improve search and data analysis algorithms.
- [ ] We will do volume and request tests on services already deployed in the IBM cloud.

# ![kukulhan](/resources/images/presentation_3.png?raw=true)

## Technologies used

* Polymer (Front-End): The polymer is JavaScript libraries created to support a component-oriented approach to front-end web development. A polymer is an open-source JavaScript library use for developing web-based applications using web components. Created by Google developers and contributors on GitHub, Polymer JavaScript library is built using JavaScript and HTML.

* NodeJS (Back-End): Node.js is an open-source server side runtime environment built on Chrome's V8 JavaScript engine. Also, can be used to build different types of applications such as command line application, web application, real-time chat application, REST API server etc. For this reason it is easy to create our own APIs to be consumed by the Front-end.

* Bcrypt (Security): The bcrypt hashing function allows us to build a password security platform that scales with computation power. We use it for security when the user enters our platform.

* API Twitter (API): It is an API to be able to consult more explicit information about what happens on Twitter.

* **IBM Watson assistant** (Cloud Service): Watson Assistant is a conversation AI platform that helps you provide customers fast, straightforward and accurate answers to their questions, across any application, device or channel. For our project we use this wizard to resolve the doubts that arise on our platform. What we are looking for with Watson is to answer questions about an aid campaign, hashtags, the information we are looking for, ask about emergency numbers and the nearest hospitals. But the most important use is to reference the strategic points of the collection centers that are located in Mexico City, this in order to complement more points of support for our users.

# ![kukulhan](/resources/images/watson_acopio.png?raw=true)

* MongoDB (Database No-SQL): Is a document-oriented No-SQL database used for high volume data storage. Instead of using tables and rows as in the traditional relational databases, MongoDB makes use of collections and documents.

* Jupyter Notebook (Data science): With data analysis/science making the news these days, we have ipython based jupyter notebooks that are being used by beginners and experts alike. The kernel provides the multiple language support to Jupyter notebooks(R, Python, Julia, Java, etc)

* Docker (Containers): A Docker container image is a lightweight, standalone, executable package of software that includes everything needed to run an application: code, runtime, system tools, system libraries and settings. We have already set up both Front-End and Back-End in Dockers and later can be deployed on **IBM Cloud Service Kubernetes**.

## Authors
* Hebert Velázquez
* Joatham Baez
* Saúl Rodríguez

## Acknowledgments
* We are grateful to IBM for allowing us to participate in this challenge where we learned about IBM Technologies throughout development. And we hope that regardless of our performance, we hope to contribute something to the community :)

* I'm grateful to Cynthia Maldonado, a great friend and for helping me in correcting the text. -Saul.
