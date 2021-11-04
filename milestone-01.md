# Assignment 01 - Milestone 01

**Due November 10 (W) @ 9 PM**

**Worth 5% of your final grade**

**starting GitHub assignment link**: https://classroom.github.com/a/iXeR-vEp  
**Make sure you move the resulting directory into your XAMPP htdocs directory!**

## Heroku

While you can work locally on a lab machine or your own computer via XAMPP, this milestone requires you to have that work up and ready for viewing on Heroku. 

This is a more complex process that you experienced with Netlify. I'll provide some guidance, because you'll be working from a GitHub repository that you don't have admin access to. (If you **did** have access, I'd be all like "RTFM, yo"...but here we are.)

There **is** some stuff I expect you to do on your own first: 

1. create an account on [Heroku](https://www.heroku.com/)
2. install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli)

After that's done, you can follow along with [this screencast (29:37)](https://youtu.be/r_Ft9TnUTkQ) I made about how to get work from your local repo to Heroku.


## Your Mark

Straightforward stuffs:

- if you meet **all** the requirements below, your mark is 100%
- if you are missing **one** of the requirements below, your mark is 50%
- if you are missing **two or more** of the requirements below, your mark is 0%

## Non-Perkable Requirements

These requirements **cannot** be postponed through the use of Perks:

- [ ] the site is hosted through Heroku

- [ ] the code for your site is in the GitHub Classroom repo you accept

- [ ] the `README.txt` file contains your name and a working link to the Heroku URL you wish me to mark. This link must go to the Home page (see that section below).

## Perkable Requirements

These requirements **can** be postponed through use of Perks.

By spending one Perk, you can extend your submission deadline **for a single requirement** by 48 hours after you've been given your requirement feedback from JP.

> _Yes, you can spend multiple Perks to extend deadlines for multiple requirements._  
> _No, you cannot spend multiple Perks to extend a single deadline longer than 48 hours._  


- [ ] all CSS on the site is declared valid by the [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/)

- [ ] all HTML on the site is declared valid by the [W3C Markup Validation Service](https://validator.w3.org/)

### The Home Page (not logged in state)

- [ ] this page has a Header, as detailed in the [Header section](#the-header) below
  
- [ ] this page has a Hero Image, as detailed in the main assignment writeup
  
- [ ] this page has an obvious way to log in (but this functionality is not yet working)

- [ ] this page has an obvious way to join (but this functionality is not yet working)

- [ ] this page has an obvious way to search for photos (but this functionality is not yet working)

- [ ] when viewed in Chrome's devtools at Mobile L size (425px) and Laptop L size (1440px), this page has a reasonable layout


### The About Page

- [ ] this page has a Header, as detailed in the [Header section](#the-header) below
  
- [ ] this page contains your name, this course's name, semester (including year), and technologies used

- [ ] this page contains a link to your GitHub profile page

- [ ] this page contains a link to this assignment's repo on GitHub

- [ ] this page displays the current date and time. PHP must be used to accomplish this.

- [ ] this page displays how many days, hours, and minutes are left until milestone 3 is due (assume it's due December 8 @ 9:00 PM). This is not a countdown timer - just how much time is left at the time this page is output by the server. PHP must be used to accomplish this.

- [ ] when viewed in Chrome's devtools at Mobile L size (425px) and Laptop L size (1440px), this page has a reasonable layout

### The Header

- [ ] the Header has a logo
  
- [ ] the Header has a navigation menu

- [ ] the navigation menu is a "hamburger" menu at mobile L size (see notes about this in the pdf)

- [ ] the navigation menu is a "standard" menu at Laptop L size

- [ ] the navigation menu contains working links to the Home and About pages


## Submission Process

Please have your final work ready on `main` - this way, I can use GitHub's code revision tools easily. You might find it useful to create branches for features you add and then merge them back on to `main` when they're complete - that way, `main` will always be the version ready to be submitted.

**Don't forget that you need to push to BOTH github AND heroku! The first is so I can see your code; the second is so I can see your web page!**

Please use a commit message that will indicate to me that that commit is your submission. We're both reasonable adults - as long as it's clear, I don't care what it says exactly. If you need to do another submit before the deadline, just make that clear from your message. I'll take the last submission before the deadline as your "official submit".

You know from the work you've done on the first assignment that handling your work on GitHub with even just one teammate can be challenging. I urge you to become familiar with standard Git team practices both to reduce the issues you have on _this_ assignment and to help you gain experience that will be useful in your future career.

Using the [GitHub flow](https://guides.github.com/introduction/flow/) is likely the easiest such practice. Here's the [first tutorial video (13:50)](https://www.youtube.com/watch?v=GgjIvUrOpmg) that popped up when I searched for "github flow tutorial". It seems pretty nice.
