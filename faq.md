# FAQ

## Milestone 2

**Q. In regards to the client validation requirements, would creating a custom error message with the built-in HTML form validation suffice? Or should we make our own error message from scratch?**

_A. I'd like to see people get some practice using JS, so although the "built-in" validation in HTML5 these days is good, I want to see "built from scratch"._

**Q. Are we able to reuse and adapt code from assignment 1 if it was written by our partner for assignment 1?**

_A. Treat the code like any other that didn't get birthed from your own noggin: attribute it._

## Milestone 1

**Q. Should all images be hosted on Cloudinary? Including logo?**

_A. Yes, please. (I've added it to the milestone requirements now.)_

_Cloudinary is a CDN (flashbacks to the midterm!) and brings tangible benefits to all image access...and it would kinda suck to have image files scattered all over the place anyway._

_Don't forget you can create different "folders" in Cloudinary, so you can keep your travel photos separate from your other stuffs._

**Q. Do the requirements that are mentioned in the pdf and main assignment but not in the milestone 01 page cost a perk if you fail to do them, or are only the requirements on the milestone page applicable.**

_A. The pdf serves as a general overview of the assignment (and I also use it to help me generate the milestones). If there's a conflict, milestone instructions trump things in the pdf._

**Q. Do we need to pull all pages in `.php` files, even if those files only contain html?**

_A. Pages that don't need any PHP currently (like the Home page) will need PHP later, so it'd be easiest to just make everything a PHP file now. See the related question that follows as well._

**Q. Do I need to use PHP to echo things (like the search box, or container divs) in the `index.php` page?**

_A. Only use it when you need to use it, or are explictly directed by milestone instructions. So in milestone 1, the only place you need to use PHP is for the two requirements that say "PHP must be used to accomplish this" on the About page._

**Q. Can we use external libraries?**

_A. That'll depend on what libraries you're talking about. If folks want to use a UI Framework (Bootstrap, ZURB, Material, Tailwind, yadayada), I'm OK with that. (It'd be cool if someone tried out Tailwind - it's pretty neat.)_

_If you want to have some kind of JS library, I'd want to know what you have in mind, because if it's something I feel you should be able to do in vanilla JS with the skills you should have at this point, then the answer would be 'no'. But there are some 'yes' opportunities as well. Talk to me._

_If it's some kind of PHP framework, then the answer will likely be no, because y'all should be buildng some PHP chops at this point. But, again, when in doubt, talk to me._

**Q. When you say Hero Image, does that image need to be uploaded to Cloudinary or can we just use the link from Unsplash?**

_A. Your site images are resources that you should be managing. You don't want some link to break on you and have your beautiful site suddenly look horrid. Put those suckers into Cloudinary._

**Q. When you say "obvious way to login or join", do you mean just a button in the navigation bar? Or like a full out page for it when we click login or join?**

_A. A button or link is fine. The actual login page ain't coming until milestone 3._

**Q. On the milestone 1 instructions it says to validate the html pages. Well I only have PHP pages and when I put the code into the validator it gives me an error message because I cannot use PHP in the html.**

_A. If you have your stuff up on Heroku, the validation will work (as long as choose 'Validate by URI')._

_If you want to validate your local work because you're not ready to push it to Heroku, then you can load your local page in the browser and copy-pasta from the 'View page source' option in your browser._

**Q. What does the "technologies used" mean?**

_A. Consider this project a portfolio piece (it is). If you showed it to a potential employer, consider these technologies things you could say "I know how to 'do' this - and this site is proof of that"._

**Q. What timezone should the time on the About page be showing in?**

_A. I want to be able to look at my computer's clock and see that it shows the same time (within a minute or so) as the time on your site._

**Q. How can I tell if my day/hour/minute calc is correct?**

_A. There are lots of tools out there. I'm checking your work with https://www.timeanddate.com/date/durationresult.html ._
