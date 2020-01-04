# LeO

LeO — *Legible, extendable, Open Source* — is a [Progressive Web App](https://developers.google.com/web/progressive-web-apps/), built with, or inspired by, sane concepts and awesome Open Source projects. 

Under the hood a "platform-agnostic CMS meta-framework", LeO is suited for quick and elegant production, cloud publishing and cloud distribution of:

 - online B2B brochures
 - slides presentations 
<br>
<br>

## 1. LeO's White Book

### Core goals

**Maximum front-end modularity:** LeO should accept any front-end .js library you throw at it.<br>
**Maximum back-end modularity:** LeO should not care about the server, the [REST](https://www.wikiwand.com/en/Representational_state_transfer) [API](https://www.wikiwand.com/en/Web_API) or the [CMS](https://www.wikiwand.com/en/Content_management_system) you are currently using. The only hard dependency is for the app's content and preferences to be exportable in [JSON format](https://www.wikiwand.com/en/JSON).



### App distribution goals

 **Platform ubiquitous** and **offline-first**. <br>
 LeO should produce custom builds for:
	 
- Progressive Web App (by default)
- iOS, Android, Windows Phone (through [Ionic CLI](http://ionicframework.com/))
- Windows, OS X, Linux (through Electron API)


### Internationalization goals

 **LeO should speak any language**. Its content data is made of strings, whether they contain text, HTML, and/or code to be executed. <br>
These strings can be stored anywhere (REST API, Firebase, Local or Cache Storage), as long as they are returned under JSON format and can be encapsulated, for complete offline usage. 


### Front-End goals

LeO is an alternative to other massively popular Content Management Systems, such as Wordpress, but it can use the output of these CMS for its data, so the clients can keep on using a familiar interface.

LeO allows designers and developers without bleeding edge knowledge to make their first step into the modern front-end development approach. 

LeO should:
  
  -  propose a restricted choice of the best UI frameworks out there:
	  - [MDL](https://getmdl.io/) (by default, included in [WSK](https://github.com/google/web-starter-kit))
	  - [Ionic 1](https://ionicframework.com/docs/) ([Ionic 2](https://ionicframework.com/docs/v2/) in 2017 roadmap, once it's stable and ironed out)
	  - [Bootstrap](http://getbootstrap.com/)


**Why such a restricted choice?** We don't want to maintain to much matrix/bridges responsible for establishing the correspondence between LeO's classes and the frameworks ones.

[Ionic](https://ionicframework.com/docs/) seems to have the proper strategy here: one CSS class serves three mobile devices/OS: iOS, Android and Windows Phone. 

Ultimately, LeO should leave the responsibility of the UI choice to the designer or the developer, just keep in mind the templates built are going to be strongly dependent of the UI framework. But this is true for any UI framework.

Whichever the UI Framework, LeO's templates should be built with the latest good practices, such as [Optimistic UI](https://www.smashingmagazine.com/2016/11/true-lies-of-optimistic-user-interfaces/) for all end user interactions, since it relies on [Service Workers](https://www.youtube.com/watch?v=cmGr0RszHc8&t=1640s), and use of [HTML 5 semantics](https://codepen.io/mi-lee/post/an-overview-of-html5-semantics), for proper semantic parsing by the search engines Bots.



### Back-end goals

Back-end data should use JSON format to be agnostic, and the crucial data (or the whole data) must be encapsulated in the app itself, for the best offline experience possible.

<br>
<br>


## 2. Technologies


## Back-end
### Firebase or any
**What for:** JSON storage and https hosting. <br>
I had faith in Firebase since their beta, and they haven't lost their fire by becoming part of Google. The Firebase dashboard is arguably one of the best Angular Material dashboards out there.
**TODO:** Leverage other Firebase capabilities, such as real-time chat, i.e. for slides presentations requiring audience interactions.


## Middle-end
### gulp or any
**What for:** Custom build generation of LeO as a Progressive Web App. <br>
Gulp is still one of the best Node task manager out there.<br>
**TODO**: keep an active survey on other tools, and see who emerges. Adoption of Ionic 2 (and therefore Angular 2) may require to switch the building 



 
### Lock.js
**What for:** auth0 capabilities. <br>
Lock provides an out-of-the-box customizable user registration.login modal, and covers entreprise-grade login solutions, such as Salesforce, Microsoft LDAP, and more.

### Reveal.js 
for its speed, its shell layout and its simple router

### Ionic 1
for AngularJS awesomeness* and App Stores capabilities**
 
 

Make atomic CSS for each page, when required

Make atomic translation files for each page (store common interface messages in a common_strings.json)

## 3. Core Concepts

### DRY
Don't Repeat Yourself.

### KISS
Keep It Simple, Stoopid.

### Vanilla
As much as we can, because who doesn't like Vanilla?
