# Turvat service

 
## Idea description:
Turvat is a platform service aimed for people who are walking or cycling in winter conditions. The service is especially targeted for elderly people but can be handy for pedestrians and cyclists of all ages. The system has two key functions for users: 1) alert on hazardous conditions to prevent accidents, and 2) help getting help in case of an accident. Other users of the system are municipalities, who are responsible for maintaining pavements by plowing snow and adding sand on icy conditions. Third user group is insurance companies as they are typically the ones who are on the payer side in case of sick leaves, insurance compensation, and so forth.
 
Turvat uses various open data services: weather data is obtained through Ilmatieteenlaitos web API’s, pavement maintenance data by municipalities, e.g., https://wp.oulunliikenne.fi/avoin-data/pyorailykavely/graphql-rajapinnat/#kunnossapitotiedot, and Google Maps for routing. Also, Turvat has its own database containing information of incidents happened to its users. This anonymized information is shared with users, in case incidents have recently happened on user’s planned route.
 
The service consists of two parts: 1) the Turvat web platform, and 2) Turvat mobile application. In short, the application works in the following way: user enters his/her destination along with the mode of transport: walk or cycle. When user is moving, the application is monitoring phone’s gyroscopic sensors. In case the system detects user trips over, the event is recorded and details (time, location, anonymized user data) are sent to the Turvat platform. In addition, user is being prompted if she/he wants to call pre-defined emergency contact. In case there is no response, and the user hasn’t moved for some time, i.e., the person is still lying on ground, the phone will make an automatic emergency call.

## Ecosystem Map
![Ecosystem map](EcosystemMap.jpg)


## Value proposition:
Given pedestrian and cyclist accidental falls is a significant cost to insurance companies, and given it is the responsibility of municipalities to ensure pavements are in safe condition, this kind of solution would provide important insight into how walking and cycling in our Nordic winter conditions can be made safer. From the user viewpoint, the system provides important information about weather conditions, helping to plan used routes. And in case of an accident, it can possibly even save lives.

## Resources
A link to google doc: https://docs.google.com/document/d/1GiOCGTAPhU8yzVhgFYMaw4idR_nk6DvBGS1skQgEogM/edit?usp=sharing
