# Login Page
User will either sign in using username, password, and ranking (admin, coach, or provider) on file or click "create account" to create a new account. When clicked on "create account" the user is redirected to the account page. Password should be encrypted as it enters database. The admin should gain access to every page in the website. The Coach should be directed to the map page once signed in and should only have access to the map, building, and unit pages. The housing provider should be directed to the provider page once signed in and only have access to provider page and form pages.
---

# Account Page
User will enter their wanted username, email, password, confirm password (background needs to make sure both passwords match), and ranking (admin, coach, or provider). Password should be encrypted as it enters database. When user clicks "create account" data should go to database and be stored in a login table to be referenced for the login page. Redirect user to login page once account data is sent to database (when "create account" button is pressed).
---

# Form Page (provider)
---
# Provider Form
This form is for the Provider to fill out their personal company information. This will be used to be included with the Provider Page, Building Info Page, and the Unit Info Page.

# Building Form
The Provider will fill out this form for all the buildings they own that they want available to be rented out. The form's info will be directed to the database to be able to be retrieved later on the provider, map, building info, unit info, buildings, and units pages. Provider will be able to click "+ Add more Buildings" to add more information to the database without having to create a form every time (so they can add all buildings at once) - if possible.

# Unit Form
The Provider will fill out this form for all the units they own that they want available to be rented out. The form's info will be directed to the database to be able to be retrieved later on the provider, map, building info, unit info, buildings, and units pages. Provider will be able to click on "Add more Units" to be able to add more information to the database all at once (add all units all at once) - if possible.
---

# Provider Page (provider)
The Provider is directed to this page after logging in. Here, they will be able to see a list of all their buildings and associated units. They should be able to edit the information here (via a button with a link to a new form) or be able to delete all the information for that specific unit or building or their own personal information.
---

# Edit Pages (provider)
The provider will be directed to these pages when they need to edit any information they entered. They will do this by clicking on the edit button (sample is given on provider page - I linked the edit buttons to the proper edit pages - but I understand it will need to be done a bit differently because data will need to be collected from the database so each edit page will need to be referenced specifically - in the URL- to each personal provider or building or data) These are just sample pages of what they could look like. You can make all three editing pages (for provider form, building form, and unit form) what you need them to look like to function. Also, the form would need to be prefilled with what they entered, that way the provider only needs to change one thing and not re-enter all fields.

# Map Page (coach)
The coach should be directed to this page automatically after logging in. This page will have a map with pins to all the available buildings. The top will also have a filter where the coach can click on things they want included in buildings, and the filter will only show buildings that are available with those specific items. The coach can then click on the pin and be taken to the buildingInfo.html page via a link.
---

# Building Info Page (coach)
This page (as shown) has the provider info at the top and then the building info underneath. The coach can then click on the name of the building and be directed to the unitInfo.html page.

# Unit Info Page (coach)
This page (as shown) has the provider info at the top, the building info next, and then all the available units with their info. A coach can then click on the "rent" button and rent out the unit for their client. Once the unit is rented, it should not show up as available until it is no longer rented.
---

# Buildings Page (coach)
This page can be accessed by a coach via the navigation bar at the top of the page and will list all available buildings. The Provider's name will be attached (accessed through database) and number of available units for that building. Link will be attached to name of building so they can be directed to unitInfo.html page so they can press the "rent" button.
---

# Units Page (coach)
This page can be accessed by a coach via the navigation bar at the top of the page and will list all available units. The Providers name and building name will be added (accessed through database) and the name of the unit will be linked to unitInfo.html so they can press the "rent" button.
---

# Database
4 tables

1: Login/Account Information - Username, Email, Password, Status (Coach, Provider, Admin)

2: Provider Information - Name, Address, Contact Information

3: Building Information - Key is Provider Name (that way when any information is saved or used for pages, it is connected to the right provider - for instance, when a provider logs in, they can only see their buildings/units; when a coach clicks on the map to see a building, the information for the provider pops up too)

4: Unit Information - Key is Building Information (so when a building is clicked on, the unit information is connected), 
