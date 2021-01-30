# Demo_Ayananta
This is for learning GitHub

## OneApp
### Background
When a person visits a store, the storekeeper often—at the time of payment—suggests downloading their application (app) for availing benefits, like earning reward points on every spend, receiving early notifications for discounts and promotional offers, getting gift vouchers, availing valet parking, and similar such offers. How many of those customers do actually download and install the app to avail the benefits? The answer is not very encouraging for stores and brands who have their own apps. Very few actually install their app. People do not feel strong enough urge to drive them in taking the effort to download and install a new app on their phone, as the reward for doing so is nominal. 

### Description of prior attempts/systems and the reasons they did not succeed
--
## 10000 feet view
**OneApp** works as a multipurpose app. It converts into the app of the location where the user is in. Say, if the user is in a Starbucks café, the app works as the Starbucks app. When the user steps out and visits a departmental store, say Walmart, the app converts into the Walmart app. When the user enters a Marriott property, it transforms into the Marriott App. The benefit is that users need not download and install multiple standalone apps. Instead this single app works as a one size fits all.
Use cases
_How it works for Users_
1.  A user downloads OneApp from the Play Store or App store. Go to [google] (https://www.google.com/)
2.  The user carries out the registration and creates a profile on the App with verified user credentials and user details.
3.  For first time users, there are two possibilities:
a.	User is at a particular place / physical store (PoI)
i.	In this case, OneApp transforms into that store’s / brand’s App and the user will be able to see all the content curated by the store / brand, along with all in-store features and functionalities offered by the store / brand
ii.	Detailing out this use case:
1.	If the user is at Starbucks, the user will be able to see the Starbucks menu, offers, store timing, etc.
2.	The user will also be able to access her Starbucks profile, including the loyalty program, available rewards, etc. which are seamlessly synced (if a persistent user identity is created)
3.	The user will also be able to use the App to place an in-store order and pay using the App (if the functionality is enabled by Starbucks and supported by the store)
b.	User is not at a PoI
i.	In this case, OneApp acts as a hyperlocal discovery engine of PoIs around the user
ii.	The user can now browse and discover PoIs by use cases (Eat / Drink / Shop / Stay), by PoI categories (Hotel / Mall / Theatre / Café / Restaurant / Shoe Store / Pharmacy), by distance (Closest or search in a particular area or within a distance), by user reviews & ratings, etc. or a combination of the above
iii.	A user can click on a particular PoI / brand to launch the brand App, even without physically being at a store and access all the information curated by the brand, as well as other functionalities offered by the brand
iv.	Detailing out this use case:
1.	The user can search for cafes in a 2 km radius and populate a list of cafes
2.	The user can further filter this list by “Cafes that support table reservations”
3.	The user can now select a particular outlet of Starbucks to launch the Starbucks App
4.	The user can now look at the menu, the real-time food availability (if the functionality is enabled by Starbucks and supported by the store), table availability (if the functionality is enabled by Starbucks and supported by the store), etc. and process a reservation for 2 at 3 pm
How it works for the PoI/Brand
1.	A brand has the following options to onboard itself to OneApp
a.	The PoI / Brand can enable its website / Progressive web app (PWA) to work with OneApp out of the box
b.	If the PoI / Brand has an existing mobile App, then the same App can be ported to OneApp
c.	The brand can choose to use the OneApp Builder to create an App from scratch with the easy to use, fully modular and customizable App Builder framework that OneApp offers
2.	Once a Brand App is created on OneApp, the brand gets full access to the user data on OneApp (filtered to each PoI / Brand) and the OneApp also offers APIs to integrate it with the brand / PoIs existing User Management system
3.	Once a Brand App is created on OneApp, the brand gets full control on all features, functionalities and content that is showcased about the PoI / Brand on OneApp, including APIs to integrate it with the Brand / PoIs existing Content Management system
4.	The PoI / Brand gets access to an automated dashboard that provides them detailed insights with respect to customers, analytics, performance, etc. which can also be customized based on category and PoI / Brand needs
5.	The PoI / Brand also gets hierarchical access control to enable multiple stakeholders to view / edit Brand data and to add / edit / delete features and functionalities
6.	The PoI / Brand can also choose to install hyperlocal attribution technology, a few options of which being QR codes / NFC / BLE beacons / Wi-Fi, that can enable OneApp to switch to the Brand App more accurately, based on user proximity
How it works at a platform level
1.	Platform Functionality
a.	OneApp is a Platform as a Service which can be used by Brands / PoIs to render Brand Apps, which are then exposed to end users via different consumer interfaces including Mobile Apps, Progressive web Apps & websites
b.	A microservice based modular backend framework is built which consists of “Widgets”
c.	The framework is built based on PoI categories and functionality / features that are relevant to that category of PoIs
d.	Each Widget represents a functionality / feature that is relevant to that category of PoI (some widgets may even overlap between multiple categories) and can be reused on demand by any Brand / PoI with operations in that category (i.e. “Menu” is a Widget which can be used by a chain of restaurants, as well as a standalone café in the F&B category)
e.	Each Widget can be further customized in terms of UI / UX, template, structure, size, categorization, sections, etc. using a modular framework, albeit the underlying functionality remains constant
f.	A Brand can even request a custom Widget to be developed, which then appears on their dashboard once the same is built by the OneApp team
g.	A Brand App on OneApp is a combination of such widgets, which a Brand / PoI can select using a dashboard made available to them, with a filter on the set of widgets that need to be rendered when a user is at a PoI and the set of widgets that need to be rendered when a user is not at a PoI (Both lists can be the same or may just be arranged in a different order of priority)
h.	Once selected, the Brand / PoI needs to add a critical mass of information / configuration for each PoI so that the same can be rendered to fulfil its intended functionality on OneApp and then exposed on to the consumer interfaces
i.	The Brand / PoI can further define the order in which these widgets appear using the dashboard and this order can either be pre-decided by the Brand or can be intelligently populated based on consumer preference led / personalization led rule sets or AI / ML algorithms
j.	In addition to the same, the Brand can also define the UI / UX, logo, templates, colours, structures, themes, animations, etc. of the consumer interfaces to customize the same to their look and feel, making each Brand App unique to the Brand / PoI identity
2.	Consumer Interfaces
a.	The consumer interfaces (Apps / PWA / Website) interact with the OneApp platform using APIs
b.	Once a new user creates an account / user identity or an existing user logs in to the account, the consumer interface detects the user context (User context is a combination of location and user proximity to a PoI)
c.	Based on the device capabilities (GPS / Bluetooth / NFC / QR scanner / Wi-Fi) and hyperlocal attribution technology deployment (QR codes / BLE Beacons / Wi-Fi / NFC), the consumer interface detects with varying degree of accuracy, whether a user is at a PoI or not
d.	If the user is at a PoI, the consumer interface requests the Brand App of that PoI to be populated from the OneApp platform
e.	If the user is not at any particular PoI, the consumer interface populates a list of PoI closest to the user based on distance / user proximity as the default mode. The user can then sort / filter this list or even alter the logic via the consumer interface settings
f.	If the user device doesn’t support location / user proximity, the user is provided a search prompt to either select a location on the map or a PoI to commence the user journey
g.	The user has overriding control to shift modes – either from being inside a PoI to discovery mode or from one Brand App to another
h.	The functionality available to a user on a Brand App is based on the Widgets enabled by that Brand / PoI on the OneApp platform and on whether the user is at the PoI (In-premise mode) or is accessing the Brand App in Discovery mode. The information available to the user is based on the information listed by the Brand / PoI on the platform
Core Claims
1.	An App / Progressive Web App / Website that changes into an App / Progressive Web App / Website of a Brand based on user location and / or user proximity and / or user context
1000 feet view
OneApp transforms into millions of apps based on a user’s context (presence at a particular place/physical store) or user’s input (user driven search, preference, etc.). Once one of the defined conditions is met, OneApp converts itself into the app of that brand / store (For e.g. When a user enters a Starbucks, it becomes the Starbucks App. When a user enters a Marriott property, it acts as the Marriott App. When a user searches for Malls, OneApp provides a list of all Malls in the vicinity and on selecting a particular mall, it acts as that Mall’s App)

