# LeO
LeO — *Legible, extendable, Open Source* — is a [Progressive Web App](https://developers.google.com/web/progressive-web-apps/), built with, or inspired by, sane concepts and awesome Open Source projects. 

Under the hood a "platform-agnostic CMS meta-framework", LeO is suited for quick and elegant production, cloud publishing and cloud distribution of:

 - online magazines and brochures
 - slides presentations 
 - any mini-website that can't afford to be "static only"
<br>

## 1. LeO's White Book
###Technical goals
Aim at maximum front-end modularity: LeO should accept any .js library you throw at it.

###App distribution goals
 Platform ubiquitous and offline-first. It should produce custom builds for:
	 - Progressive Web App (by default)
	 - iOS, Android, Windows Phone (through Ionic CLI)
	 - Windows, OS X, Linux (through Electron API)

###Front-End goals
 - free designers and developers without bleeding edge knowledge from other massively popular CMS systems
 - use the Optimistic UI approach for all end user interactions
 -  give a restricted set of the best UI frameworks out there

###Back-end goals
Back-end data should use JSON format to be agnostic, and the crucial data (or the whole data) must be encapsulated in the app itself, for the best offline experience possible.

<br>
#2. Technologies

##Back-end
### Firebase
**What for:** JSON storage and https hosting. 
I had faith in Firebase since their beta, and they haven't lost their fire by becoming part of Google. The Firebase dashboard is arguably one of the best Angular Material dashboards out there.
**TODO:** Leverage other Firebase capabilities, such as real-time chat, i.e. for slides presentations requiring audience interactions.


##Middle-end
###gulp
**What for:** Custom build generation of LeO as a Progressive Web App. 
Gulp is still one of the best Node task manager out there.
TODO: keep an active survey on other tools, and see who emerges. Adoption of Ionic 2 (and therefore Angular 2) may require to switch the building 

###Web Starter Kit
**What for:** out-of-the-box speed and offline-first capabilities. 
Learn more about the importance of offline-first and Service Workers with Jake Archibald.
**TODO:** have a service worker generator able to handle as many as useful caching strategies possible. 



 
###Lock.js
**What for:** auth0 capabilities. 
Lock provides an out-of-the-box customizable user registration.login modal, and covers entreprise-grade login solutions, such as Salesforce, Microsoft LDAP, and more.

###Reveal.js 
for its speed, its shell layout and its simple router

###Ionic 1
for AngularJS awesomeness* and App Stores capabilities**
 
 

Make atomic CSS for each page, when required

Make atomic translation files for each page (store common interface messages in a common_strings.json)

##3. Core Concepts

###DRY
Don't Repeat Yourself.

###KISS
Keep It Simple, Stoopid.

###Vanilla
As much as we can, because who doesn't like Vanilla?
