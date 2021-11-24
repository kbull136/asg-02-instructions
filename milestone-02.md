# Assignment 02 - Milestone 02

**Due November 24 (W) @ 9 PM**

**Worth 5% of your final grade**

**starting GitHub team assignment link**: https://classroom.github.com/a/bEkGuriD

**Make sure you move the resulting directory into your XAMPP htdocs directory!**

## Your Mark

In an attempt to learn from past experience, I am modifying how this milestone is marked.

I have separated requirements into the following sections:

1. [Non-Perkable Requirements](#non-perkable-requirements)
2. [Validation Requirements](#validation-requirements)
3. [Header Requirements](#header-requirements)
4. [Country Page Requirements](#the-country-page-requirements)
5. [City Page Requirements](#the-city-page-requirements)
6. [Photo Page Requirements](#the-photo-page-requirements)
7. [Registration/Signup Page Requirements](#the-registrationsignup-page-requirements)
8. [Countries API Requirements](#the-countries-api-requirements)

For a section to be considered "completed", **ALL** requirements in that section must be completed.

| completed requirement sections                    | mark (%) |
| ------------------------------------------------- | -------- |
| Non-Perkable + Header + Validation + Restrictions | 20       |
| 20% req's + Registration **or** Countries API     | 45       |
| 20% req's + Registration **and** Countries API    | 55       |
| 55% req's + ONE of Country, City, Photo           | 75       |
| 55% req's + TWO of Country, City, Photo           | 90       |
| All req's                                         | 100      |

## About The "Look" of Your Site

The blurb from page 2 of the assignment pdf says it all:

> _...the sketches in this assignment specification are meant to show **functionality**, not design. Here I've shown content as boxes, but you can do them as rectangles, circles, icons, simple links, etc. **Make your pages look nicer than these sketches!**_

I'll stress that _submitting something that looks like the sketches is a bad idea_. I should have made this clear in assignment 1. Here I am, learning from my mistakes!

**Takeaway: While the look of your site can be put on the back burner until milestone 3, that look will play a non-trivial role in your mark of milestone 3. If you want me to provide you with some quick feedback about your visual design, I can.**

## Restrictions (NEW: 2021-11-17)

- [ ] The **only** data you're allowed to cache in this milestone is the country data you pull in from your own API.

- [ ] You are **not** allowed to pull in any data from Randy's API from assignment 1, nor create another API to access other data necessary for this assignment.

  > _The reasoning here is that you've already had experience doing API consumption in assignment 1. It's now time to gain experience from pulling in data from your own back-end sources using PHP._

- [ ] Since you're allowed to cache the country data, you are allowed to populate the Country List (in both the Country and City pages) and the Country Details (in the Country Page) via JS if you wish. All other data population must be done through PHP.

## Non-Perkable Requirements

These requirements **cannot** be postponed through the use of Perks:

- [ ] the site is hosted through Heroku and connected to your GitHub Classroom Assignment

- [ ] all image files are hosted on Cloudinary

- [ ] the `README.txt` file contains the names of all team members and the Heroku URL of the site you wish me to mark

- [ ] the URL provided in the README goes to the Home page (as per milestone 1)

## Perkable Requirements

These requirements **can** be postponed through use of Perks.

I want to tweak the system a bit. In this milestone (and likely the next), all members of the group can pool their Perks together. The cost for getting extensions now depends on the the number of extensions being requested and the number of group members:

| # extensions | 3-member cost | 4-member cost |
| ------------ | ------------- | ------------- |
| 1            | 1             | 1             |
| 2            | 2             | 3             |
| 3            | 4             | 6             |
| 4            | 7             | 10            |
| 5            | 11            | 15            |

If you ask for extensions, I will now need to know **who** is paying **how many** Perks!

> _Say you're in a group with 3 members._
>
> _Member A has 2 Perks, Member B has 4, and Member C has 4. They have 2 + 4 + 4 = 10 Perks to spend on extensions._
>
> _If they decide they need 4 extensions, they'd have to pay 7 Perks and let me know who is paying what. (Like, "A will pay 1 and B and C will pay 3 each.")_

### Validation Requirements

_Since I don't want to check **every** page for valid HTML and CSS, I will instead use the Goddess of Fate to decide: I will randomly choose ONE page to check for HTML violations and ONE page to check for CSS violations_

- [ ] all CSS on a randomly chosen page in the site is declared valid by the [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/)

- [ ] all HTML on a randomly chosen page in the site on the site is declared valid by the [W3C Markup Validation Service](https://validator.w3.org/)

### Header Requirements

- [ ] the Header has a logo

- [ ] the Header has a navigation menu

- [ ] the navigation menu is a "hamburger" menu at mobile L size (see notes about this in the pdf)

- [ ] the navigation menu is a "standard" menu at Laptop L size

- [ ] the navigation menu contains working links to the Home, About, Country, ~~City~~, ~~Photo~~, and Registration pages

  > _**Note from JP (2021-11-22)**: I've turfed City and Photo for this milestone because they don't make sense, given the constraints on when those pages are displayed! If you have them in your current work, you can keep them there or not - I'll be testing those pages by mangling the URL._

### The Country Page Requirements

_An overview of the Country Page can be found on page 5 of the [assignment pdf](comp-3512-asg-2-fall-2021-version-4.pdf)._

_You should read the [warnings at the bottom of this document](#read-this-or-suffer-madness) before reading these requirements._

_I will mangle the URL to reach this page and then begin checking these requirements. So if I wanted to see your page on Canada, I'd need to go to `single-country.php?iso=ca`_

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

- [ ] all country details, as outlined in the assignment pdf, are present for the current country. All details are generated via PHP, not JS.

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

_An overview of the City Page can be found on page 6 of the [assignment pdf](comp-3512-asg-2-fall-2021-version-4.pdf)._

_Make sure you read [the warnings below](#read-this-or-suffer-madness) - they are applicable here._

_I will mangle the URL to reach this page and then begin checking these requirements. So if I wanted to see your page on Calgary, I'd need to go to `single-city.php?id=5913490`_

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

- [ ] all city details, as outlined in the assignment pdf, are present for the current city. All details are generated via PHP.

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

_An overview of the Photo Page can be found on page 7 of the [assignment pdf](comp-3512-asg-2-fall-2021-version-4.pdf)._

_Make sure you read [the warnings below](#read-this-or-suffer-madness) - they are applicable here._

_I will mangle the URL to reach this page and then begin checking these requirements. So if I wanted to see the image for the Lyon Train Station, I'd need to go to `single-photo.php?id=103`_

- [ ] the file for this page is named **single-photo.php**

- [ ] if the query string parameter for this page is invalid in any way, the user is redirected to a generic error page. Unlike the Country and City cases, a non-existent query string **is** an error.

- [ ] this page has a Header, as detailed in the [Header section](#the-header)

- [ ] when viewed in Chrome's devtools at Mobile L size (425px) and Laptop L size (1440px), this page has a reasonable layout

- [ ] A larger version of the thumbnail that caused this view to appear is displayed. You can choose a size that works for your layout.

  > _A Cloudinary transformation must be used to achieve this - you cannot just use CSS to shoehorn an improperly-sized image onto the page._

- [ ] In addition to the photo itself, the title, ~~user name (not optional this time!)~~, city, and country are also displayed. All details are generated via PHP.

  > _**comment from JP**: there **is** a user field in the image objects you get back from the API. It is not optional this go-round because it actually does represent a user of our website!._

  > _**a comment on my previous comment(2021-11-22)**: I did not provide you with a file that has the User data! Face palmed. You can ignore the User display requirement **for this milestone** - it **definitely** will be a requirement in milestone 3!_

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

### The Registration/Signup Page Requirements

_An overview of the Registration Page can be found on page 11 of the [assignment pdf](comp-3512-asg-2-fall-2021-version-4.pdf)._

You should **ignore** (for this milestone) the second and third paragraphs in the Registration/Signup page description. Instead, these are the requirements for this milestone:

- [ ] a registration form containing the fields in the sketch on page 11 is displayed

- [ ] the form is well-presented. Many resources abound on the web about this. [This one is quite nice](https://gerireid.com/forms.html), for example.

- [ ] the page uses JS to perform client-side validation:

  - [ ] first name, last name, city and country cannot be blank

  - [ ] email is in a proper format (using a regex you find online and attribute in your About page)

  - [ ] password and confirmation are 8+ characters long and match

- [ ] if client-side validation of the form detects any issues, these issues are conveyed to the user in a reasonable and nice-looking way

- [ ] the form action is a POST (but while you're developing the form requirements, you will find it useful to use GET - just remember to change it back to POST before submission!)

- [ ] when the form is submitted, it redirects to another page displaying the contents of the fields that were submitted, kind of like was done in tutorial-08. (This will NOT happen in milestone 3 - it's just for this milestone.)

#### if you have the textbook and/or labs

Section 9.5 (Forms in JavaScript) will be pretty useful here, as is ex 9.13 (Working with Forms) in Lab 9.

If you don't have these resources, you will find it fairly straightforward to find resources to help you...there may be _too_ many out there, to be honest!

---

### The Countries API Requirements

- [ ] if you go to `api-countries.php` in the browser, you are provided with JSON representing all countries available in the array provided in `countries-data.php`

- [ ] if you go to `api-countries.php?iso=xx` in the browser, you are provided with JSON representing the country with iso=xx

- [ ] data from both endpoints is valid JSON (you can find online validators to help you be sure)

---

## Read This, Or Suffer Madness

While very much like parts of assignment 1, you can't just copy/paste your code from assignment 1 into the Country, City, and Photo pages and call it a day.

Far from it.

Here are some important differences provided in the [assignment pdf](randy-original-2019-04-asg2-v1.pdf) that you can find if you read carefully, but that I'm providing here as a PSA:

### getting to the country, city, and photo pages

#### Country Page

The only ways you can actually reach the Country Page in milestone 2 are:

- getting there from the Header menu
- getting there from the Photo Page
- getting there by clicking a country name on the Country Page or City Page
- cutting the [Gordian Knot](https://en.wikipedia.org/wiki/Gordian_Knot) by mangling the URL and adding a valid query string to take you to the country you want to view

#### City Page

The only ways you can actually reach the City Page in milestone 2 are:

- ~~getting there from the Header menu~~
- getting there from the Photo Page
- getting there by clicking a city name on the Country Page
- mangling the URL and adding a valid query string to take you to the city you want to view

#### Photo Page

The only ways you can actually reach the Photo Page in milestone 2 are:

- getting there by clicking a photo on the Country Page or City Page
- mangling the URL and adding a valid query string to take you to the photo you want to view

### data for the pages

With the exception of the list of countries, all data that changes in these pages (country details, city list, country photos, etc.) must be generated using PHP from your "faux database" (see the next section).

##### no db yet, so...

Grabbing data from a database will happen in milestone 3, not here. To get around this, much like you were asked to do in milestone 2 of assignment 1, you'll use data from an alternate source for the time-being.

You've been given a number of associative arrays containing some of the data that you will eventually need to obtain yourself via database queries in milestone 3.

You will want to create some functions - in a separate php file - that allow you to pull needed information out of these arrays for use in the Country, City, Photo, and Countries API requirements.
