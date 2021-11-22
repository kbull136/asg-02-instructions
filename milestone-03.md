# Assignment 02 - Milestone 03

# not complete yet!

**Due December 8 (W) @ 9 PM**

**Worth 15% of your final grade**

*Holy cow - I think we're gonna make it!*

## Your Mark

I have separated requirements into the following sections (the ⚠ denotes either a new requirement or a requirement that has changed since milestone 2):

1. [Non-Perkable Requirements](#non-perkable-requirements) ⚠
2. [Visual Design Requirements](#visual-design-requirements) ⚠ 
3. [Validation Requirements](#validation-requirements)
4. [Header Requirements](#header-requirements) ⚠
5. [Home Requirements](#) ⚠
6. [Country Page Requirements](#the-country-page-requirements)
7. [City Page Requirements](#the-city-page-requirements)
8. [Photo Page Requirements](#the-photo-page-requirements)
9.  [Favorites Page Requirements](#) ⚠
10. [Registration/Signup Page Requirements](#the-registrationsignup-page-requirements) ⚠
11. [Browse/Search Page Requirements](#) ⚠
12. [Login Page Requirements](#) ⚠
13. [Countries API Requirements](#the-countries-api-requirements)

For a section to be considered "completed", **ALL** requirements in that section must be completed.

| completed requirement sections                                 | mark |
| -------------------------------------------------------------- | ---- |
| Non-Perkable + Header + Validation + API                       | F+   |
| F+ req's + Country, City, and Photo Pages                      | D+   |
| D+ req's + Home + Login                                        | C    |
| C req's + Visual Design + Registration                         | B    |
| B req's + Best Practices + **one** of Favorites, Browse/Search | A    |
| All req's                                                      | A+   |



## Non-Perkable Requirements

These requirements **cannot** be postponed through the use of Perks:

- [ ] The site is hosted through Heroku and connected to your GitHub Classroom Assignment.

- [ ] **All** image files are hosted on Cloudinary.

- [ ] The `README.txt` file contains the names of all team members and the Heroku URL of the site you wish me to mark.

- [ ] The URL provided in the README goes to the Home page.

- [ ] You only cache country data - and you pull it in from your own API.

- [ ] You only populate the Country List and Country Details using JS; all other data that **can** be pulled in from the database **is** pulled in from the database and presented via PHP.

- [ ] All DB access is via PDO. No mysqli is used.


## Perkable Requirements

These requirements **can** be postponed through use of Perks.

The cost for getting extensions  depends on the the number of extensions being requested and the number of group members:

| # extensions | 3-member cost | 4-member cost |
| ------------ | ------------- | ------------- |
| 1            | 1             | 1             |
| 2            | 2             | 3             |
| 3            | 4             | 6             |
| 4            | 7             | 10            |
| 5            | 11            | 15            |
| 6            | 16            | 21            |
| 7            | 22            | 28            |

If you ask for extensions, I will now need to know **who** is paying **how many** Perks!

> _Say you're in a group with 3 members._
>
> _Member A has 2 Perks, Member B has 4, and Member C has 4. They have 2 + 4 + 4 = 10 Perks to spend on extensions._
>
> _If they decide they need 4 extensions, they'd have to pay 7 Perks and let me know who is paying what. (Like, "A will pay 1 and B and C will pay 3 each.")_

---

## Visual Design Requirements

- [ ] The visual design looks presentable enough to become a portfolio piece.

> _I get that people are uber-busy on the back-end, coding up the codez. But you really **do** have to expend at least a *bit* of effort making things look presentable._
>  
> _So if you want to use a framework of some kind to help with this, that's fine. I'm not asking for too much...but it shouldn't look like no effort was applied._
> 
> _I know this is super-vague, but how the heck can I quantify the requirements here at all?_

---

### Validation Requirements

_Since I don't want to check **every** page for valid HTML and CSS, I will instead use the Goddess of Fate to decide: I will randomly choose ONE page to check for HTML violations and ONE page to check for CSS violations_

- [ ] all CSS on a randomly chosen page in the site is declared valid by the [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/)

- [ ] all HTML on a randomly chosen page in the site on the site is declared valid by the [W3C Markup Validation Service](https://validator.w3.org/)

---

### Header Requirements

- [ ] the Header has a logo appropriate for the site

- [ ] the Header has a navigation menu

- [ ] the navigation menu is a "hamburger" menu at mobile L size (see notes about this in the pdf)

- [ ] the navigation menu is a "standard" menu at Laptop L size

- [ ] the navigation menu contains working links to the following pages:
  
    - Home
    - About
    - Browse/Search
    - Countries
    - Cities
    - ~~Profile~~ (removed)
    - Favorites
    - Login/Logout
    - Registration/Sign Up


### The Home Page Requirements

---

### The About Page Requirements

I will assume you haven't busted anything from milestone 1, so will only be looking for these additional requirements:

- [ ] all group members are listed here, as are their GitHub profile links

---

### The Browse/Search Page Requirements

---

### The Country Page Requirements

_An overview of the Country Page can be found on page 5 of the [assignment pdf](comp-3512-asg-2-fall-2021-version-2.pdf)._

- [ ] the file for this page is named **single-country.php**

- [ ] if the query string parameter for this page is invalid in any way, the user is redirected to a generic error page. A non-existent query string is **not** invalid!

- [ ] this page has a Header, as detailed in the [Header section](#the-header)

- [ ] when viewed in Chrome's devtools at Mobile L size (425px) and Laptop L size (1440px), this page has a reasonable layout

- [ ] a well-presented, alphabetically-sorted list of all countries from your [countries API](#the-countries-api) is visible on the page. This list is populated via JS (see assignment 1), not PHP.

- [ ] each country in the country list hyperlinks back to this page with a query string parameter indicating the country to display

  > _for example the link to Canada would need to go to `single-country.php?iso=ca`_

- [ ] caching of the list of countries occurs to local storage occurs, just like it did in assignment 1

- [ ] all filtering behaviour from assignment 1 is present and is done solely through JS

- [ ] filters are well-presented

  > _this is my way of saying "improve the presentation of the filters as compared to assignment 1_

- [ ] clicking on a country will cause this page to reload this page for that country

- [ ] all country details, as outlined in the assignment pdf, are present for the current country. Since you've cached the country details, you can present them via JS if you wish.

  > _if the query string parameter is non-existent, the country details section should show no data_

- [ ] a list of cities for the current country are present, each city hyperlinking to the `single-city.php` page with an appropriate query string parameter

  > _if the query string parameter is non-existent, the city list section should show no data_

- [ ] if photos are available for the current country, they are displayed in a well-presented fashion.

  > _The sizes can be changed from the restrictions presented in assignment 1, but all images **must** be hosted on Cloudinary and **must** be resized so that the user isn't pulling down unnecessarily large image files!_

- [ ] if photos are **not** available for the current country, that fact is indicated in a clear and well-presented way

  > _if the query string parameter is non-existent, the photos section should show no data_

- [ ] each photo present hyperlinks to the `single-photo.php` page with an appropriate query string parameter

---

### The City Page Requirements

_An overview of the City Page can be found on page 6 of the [assignment pdf](comp-3512-asg-2-fall-2021-version-2.pdf)._

- [ ] the file for this page is named **single-city.php**

- [ ] if the query string parameter for this page is invalid in any way, the user is redirected to a generic error page. A non-existent query string is **not** invalid!

- [ ] this page has a Header, as detailed in the [Header section](#the-header)

- [ ] when viewed in Chrome's devtools at Mobile L size (425px) and Laptop L size (1440px), this page has a reasonable layout

- [ ] a well-presented, alphabetically-sorted list of all countries from your country API is visible on the page. This list is populated via JS (see assignment 1), not PHP.

- [ ] each country in the country list hyperlinks back to this page with a query string parameter indicating the country to display

  > _for example the link to Canada would need to go to `single-country.php?iso=ca`_

- [ ] caching of the list of countries occurs to local storage occurs, just like it did in assignment 1

- [ ] all filtering behaviour from assignment 1 is present and is done solely through JS

- [ ] filters are well-presented

  > _this is my way of saying "improve the presentation of the filters as compared to assignment 1_

- [ ] clicking on a country will cause this page to load the `single-country.php` page for that country

- [ ] all city details, as outlined in the [assignment pdf](comp-3512-asg-2-fall-2021-version-2.pdf), are present for the current city. All details are generated via PHP. 

  > _if the query string parameter is non-existent, the city details section should show no data_

- [ ] the static country map described in the assignment pdf is present for the current city

  > _Yes - a map using the [Google Maps Static API](https://developers.google.com/maps/documentation/maps-static/overview). You've got plenty of time to get your credits in order now and read up on this API._

  > _if the query string parameter is non-existent, the city map section should show no data_

- [ ] if photos are available for the current city, they are displayed in a well-presented fashion.

  > _The sizes can be changed from the restrictions presented in assignment 1, but all images **must** be hosted on Cloudinary and **must** be resized so that the user isn't pulling down unnecessarily large image files!_

- [ ] if photos are **not** available for the current city, that fact is indicated in a clear and well-presented way

  > _if the query string parameter is non-existent, the photos section should show no data_

- [ ] each photo hyperlinks to the `single-photo.php` page with an appropriate query string parameter

---

### The Photo Page Requirements

_An overview of the Photo Page can be found on page 7 of the [assignment pdf](comp-3512-asg-2-fall-2021-version-2.pdf)._

- [ ] the file for this page is named **single-photo.php**

- [ ] if the query string parameter for this page is invalid in any way, the user is redirected to a generic error page. Unlike the Country and City cases, a non-existent query string **is** an error.

- [ ] this page has a Header, as detailed in the [Header section](#the-header)

- [ ] when viewed in Chrome's devtools at Mobile L size (425px) and Laptop L size (1440px), this page has a reasonable layout

- [ ] A larger version of the thumbnail that caused this view to appear is displayed. You can choose a size that works for your layout.

  > _A Cloudinary transformation must be used to achieve this - you cannot just use CSS to shoehorn an improperly-sized image onto the page._

- [ ] In addition to the photo itself, the title, user name (not optional this time!), city, and country are also displayed. All details are generated via PHP.

  > _**comment from JP**: there **is** a user field in the image objects you get back from the API. It is not optional this go-round because it actually does represent a user of our website!._

- [ ] the city name shown on the page hyperlinks to the `single-city.php` page with an appropriate query string parameter

- [ ] the country name shown on the page hyperlinks to the `single-country.php` page with an appropriate query string parameter

- [ ] there should be an obvious way to access the Description, Details, and Map sections in Single Photo View. Although tabs are shown in the provided layout sketch, you could use some kind of obvious show/hide mechanism as well.

- [ ] when the Description information is accessed, it should show the information in the photo's description field.

- [ ] when the Map information is accessed, it should show a static Google map with the photo’s lat+long location indicated via a marker.

  > _Yes - a map using the [Google Maps Static API](https://developers.google.com/maps/documentation/maps-static/overview). You've got plenty of time to get your credits in order now and read up on this API._

- [ ] when the Details information is accessed, it should show the exif information (model, exposure, aperture, focal length, iso), credit information, and color information.

- [ ] when a user mouses into the image, display in a box (that has a little bit of transparency), the credit info, the exif info (model, exposure, aperture, focal length, iso), and color information. When the mouse is moved outside the image, this box should disappear.

- [ ] each time color information is displayed (in either the Details section or when the Single Photo View image is hovered over), this information should be displayed as color boxes with the corresponding hex values clearly visible as well.

---

### The Favorites Page Requirements

---

### The Registration/Signup Page Requirements

_An overview of the Registration Page can be found on page 11 of the [assignment pdf](comp-3512-asg-2-fall-2021-version-2.pdf)._

- [ ] a registration form containing the fields in the sketch on page 11 is displayed

- [ ] the form is well-presented. Many resources abound on the web about this. [This one is quite nice](https://gerireid.com/forms.html), for example.

- [ ] the page uses JS to perform client-side validation:

  - [ ] first name, last name, city and country cannot be blank

  - [ ] email is in a proper format (using a regex you find online and attribute in your About page)

  - [ ] password and confirmation are 8+ characters long and match

- [ ] if client-side validation of the form detects any issues, these issues are conveyed to the user in a reasonable and nice-looking way

- [ ] the form action is a POST (but while you're developing the form requirements, you will find it useful to use GET - just remember to change it back to POST before submission!)

- [ ] when the form is submitted, 


---

### The Countries API Requirements

- [ ] if you go to `api-countries.php` in the browser, you are provided with JSON representing all countries available in the array provided in `countries-data.php`

- [ ] if you go to `api-countries.php?iso=xx` in the browser, you are provided with JSON representing the country with iso=xx

- [ ] data from both endpoints is valid JSON (you can find online validators to help you be sure)

