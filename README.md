
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

| Tracks | List of Speakers 
| --- | --- |
| <img src=""/> | <img src="" /> 

### Coding Phase I

A lot of crucial features were implemented in this period. The highlight of this coding phase was the success implementation of the custom date and time pickers in the Orga app which allowed us to remove the use of observable fields in the models. The other important ones are as follows:
1. Server side integration of *Stripe Express checkout* for the event wizard.
2. Addition of a schema defaulting decorator in order to fix the schema validation in the server.
3. Addition of unit tests for the speakers module in the orga app.
4. Refactor of the Settings endpoint into Public, Non-Admin and Admin schemas.

| Custom date and time picker | Stripe Express checkout 
| --- | --- |
| <img src=""/> | <img src="" />

### Coding Phase II









