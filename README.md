
<p align="center">
  <img width="560" height="120" src="https://camo.githubusercontent.com/ed508e9c66d718f76333215a139af24f8bb8fa8d/68747470733a2f2f6d75736573636f72652e6f72672f73697465732f6d75736573636f72652e6f72672f66696c65732f4361707475726525323064253237652543432538316372616e253230323031362d30332d303125323030392e34382e31315f302e706e67">
</p>

## Google Summer of Code 2018 Work Report 

| Field | Details |
| --- | --- |
| **Student** | **Saurav Tiwary** |
| **Github** | [@srv-twry](http://github.com/srv-twry)  |
| **Organisation**  | [FOSSASIA](http://fossasia.org)  |
| **Project** | [Open Event](https://summerofcode.withgoogle.com/projects/#5905844613414912) |  
| **Technology** | Flask, Ember JS and Android |

## Project Description
![Open Event](https://camo.githubusercontent.com/6386234d12db1b6710ddaadc83cafd94b7a16299/68747470733a2f2f73746f726167652e676f6f676c65617069732e636f6d2f6576656e747961792e636f6d2f6173736574732f6272616e64696e672f626173655f6272616e64696e672e706e67)

The  **[Open Event](https://github.com/fossasia/open-event)**  Project offers event managers a platform to organize all kinds of events including concerts, conferences, summits and regular meetups. The various components support organizers in all stages from event planning to publishing, marketing and ticket sales. Automated web and mobile apps help attendees to get information easily.

There were two major divisions of this project:
1. Implementation of numerous features on the **Open Event Server** in order to make it feature complete. Some of the features that we aimed for were the integration of *payment system*, *tickets*, *taxes*, *promo codes* etc. 

2. Integration of missing endpoints and related features on the **Open Event Frontend** and **Open Event Orga** app. Some of the features that we aimed for in the *frontend* were the implementation of *promo codes*, *notifications* while *tracks* and *speakers* endpoints were targeted for the orga app.

## Results

Considering that we were able to achieve the project goals as well as implement additional features as our stretch goals, the project was a **success**.

### Community Bonding Period
We kicked off the summer with the bonding period. Most of the time in the period was utilised in understanding the organization's community. Additionally we started the implementation of few of the missing endpoints in the orga app. We were able to successfully integrate the *tracks* and parts of the *speakers* api in the orga app.

| [Tracks](https://github.com/fossasia/open-event-orga-app/issues/870) | [List of Speakers](https://github.com/fossasia/open-event-orga-app/pull/926) 
| --- | --- |
| <img src="https://i.imgur.com/HgVob1U.png"/> | <img src="https://user-images.githubusercontent.com/21277837/39904192-5513fb18-54f4-11e8-8606-0fe04ad742eb.png" /> 

### Coding Phase I

A lot of crucial features were implemented in this period. The highlight of this coding phase was the success implementation of the custom **Date** and **Time** pickers in the *Orga app* which allowed us to remove the use of observable fields in the models. The other important ones are as follows:
1. Server side integration of *Stripe Express checkout* for the event wizard.
2. Addition of a schema defaulting decorator in order to fix the schema validation in the server.
3. Addition of unit tests for the *speakers* module in the *Orga* app.
4. Refactor of the Settings endpoint into Public, Non-Admin and Admin schemas.
A lot of minor bugs such as *Internal server error* were solved along side the above mentioned features.

| [Custom date and time picker](https://github.com/fossasia/open-event-orga-app/pull/932) |  
| --- |
| <img src="https://i.imgur.com/cMGcCed.png"/> |

### Coding Phase II

We started to gather momentum by the start of the coding phase II and hence this phase was the most productive coding phase of the project. We started out with the aim of completing the most important features of the project in this phase so that we can have ample time to test the features before they are pushed to production. The highlight of this coding phase was the successful implementation of the *Orders* endpoint in the *Open Event Server*. We were able to integrate payments via both **Stripe** and **Paypal**. Another major achievement of this period was the integration of *Soft Deletion* support in the server. This meant that the admin of the platform could easily restore all the user and event related information with a single click!
Other important features implemented in this period are as follows:
1. Server side implementation of the Tax endpoint.
2. Implementation of endpoints for accessibility of *Access & Discount codes* via it's *code*.
3. The API integration of *Access code* creation in the *Tickets tab* in the *Open Event Frontend*.
4. Refactor of the *Main Presenter* in the *Open Event orga app* which led to improved architecture and code readability.
5. Addition of a *Rate Limiter* in the *Abstract observables* in the *Open Event Orga app* which fixed multiple instances of infinite loops present in the project.
As always numerous bugs were fixed in this period as well.

| Payment via Stripe | Payment via Paypal | 
| --- | --- |
| <img src=""/> | <img src="" />

### Coding Phase III
The third coding phase involved implementation of the remaining targets of the project. Most of the work on the server side was done and hence more emphasis was given on the *Frontend* side. We started off with the implementation of the *My Tickets* tab in the *Frontend*. We then moved  on to the implementation of user input validation throughout the project. Lastly we were able to implement automatic *Order expiry* in the *Server*.
By this time, we were able to successfully achieve all the targets of the program. Since we had a good part of 2 weeks left in the coding phase we decided to go ahead with our stretch goals. The first stretch goal accomplished was the implementation of the *Attendee form builder* both on the server and frontend side. Now the event organizer could specify what information to collect from the ticket buyers which was a highly demanded feature. With a week still left in the coding period, we decided to integrate action buttons in the *Notification panel*. We started off with the server side support and quickly moved on to it's frontend integration.
Apart from the above mentioned features, we spent a lot of time on fixing minor bugs and addition of unit tests whenever possible.

| [Notification Panel](https://github.com/fossasia/open-event-frontend/issues/1112) | 
| --- | 
| <img src="https://i.imgur.com/9Lmyk7N.png"/> 
## Link to commits

[Open Event Server](https://github.com/fossasia/open-event-server/commits?author=srv-twry)

<p align="left">
  <img width="458" height="193" src="https://i.imgur.com/hxbObJZ.png">
</p>

[Open Event Frontend](https://github.com/fossasia/open-event-frontend/commits?author=srv-twry)

<p align="left">
  <img width="458" height="193" src="https://i.imgur.com/pMowm3Z.png">
</p>


[Open Event Orga app](https://github.com/fossasia/open-event-orga-app/commits?author=srv-twry)

<p align="left">
  <img width="458" height="193" src="https://i.imgur.com/UfR86Zx.png">
</p>

## Blog Posts

All of my blog posts related to my work can be found in the FOSSASIA Blog [http://blog.fossasia.org/author/srv-twry/](http://blog.fossasia.org/author/srv-twry/)

## Scrums

My Scrum Reports which includes daily work report can be found [here](https://groups.google.com/forum/#!searchin/open-event/Saurav$20Tiwary%7Csort:relevance).

## Social
* [Facebook posts about the Project](https://www.facebook.com/search/str/fossasia/keywords_blended_posts?filters_rp_author=%7B%22name%22%3A%22author_me%22%2C%22args%22%3A%22%22%7D)
* [Tweets about the Project](https://twitter.com/search?l=en&q=from%3Asrv_twry%20%40fossasia&src=typd&lang=en-gb) 
* [Youtube Screencast about my Project]()
* [Presentation about my Project]()
