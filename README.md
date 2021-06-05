# The Guitar Centre

I've chosen to redesign the website for my local guitar shop, **The Guitar Centre, in Sevenoaks, UK**.

The existing website can be viewed [here](https://www.sevenoaksguitarcentre.co.uk/).

The redsigned website can be viewed [here](https://oerbeyer.github.io/MS1/index.html).

I chose this project for the following reasons:
- I am a guitar music enthusiast and I am passionate about playing the guitar myself.
- I love the my local guitar shop.
- This is a real business with a real need for user centric frontend development.
- The business has an existing website, but there is a need to enhance UX and UI design to reflect current standard and best practices.
- All businesses should periodically review and if necessary enchance UX and UI design to maximise value for users.
- The existing website provides a starting point for content and some UX and UI design might be worth retaining or incorporating.
- This allows me to focus on applying UX and UI enhancements that drive value for users.
- This makes it a very good candidate for the user centric frontend design section of this Code Institute Diploma course.
- The existing website is a set of static webpages.
- This makes it a very good candidate for the user centric frontend design section of this Code Institute Diploma course.
- The responsiveness of the UX design is especially in need of enhancement.

![Landing Page](https://github.com/oerbeyer/MS1/blob/master/assets/screenshots/02%20laptop-home-workshop-carousel.jpg)

## UX

This website is aimed at guitar players of various skill levels and anyone thinking of 
taking up playing the guitar.

The summary value drivers for the business and for customers (based on the user stories) are as follows:

### Value drivers for the business

+ The website should support and enhance the business's brand which is passion for and 
expertise in all things guitar.
+ The website should generate email enquiries, facebook enquiries, phone calls and 
in-store visits.
+ The website should encourage repeat visits and contact from customers.
+ The website should render properly and responsively on smart phones, tablets (portrait) and laptops.
+ The website should clearly explain how the business is operating during Covid-19.

### Value drivers for the customer

+ The website should be attractive to and relevant for guitar players of various skill levels.
+ The website should be attractive to and relevant for someone who is thinking of taking up playing the guitar.
+ The website should allow the customer to find the relevant services without navigating away from the landing page.
+ The website should allow the customer to contact the business easily from any webpage in the website.
+ The website should be simple to navigate.
+ The website should have clear calls to action e.g. special offers.


### User stories
Please note that the following is **not** an ordered list of user stories. The **ID** is simply a 4 digit unique identifier. 
An ID starting with a 1 is a business user story. An ID starting with a 2 is a customer user story. 

The focus is on the customer, hence the larger number of customer user stories relative to business user stories in the list. 
However, it should be clear from reading the list that the two sets of user stories are consistent and mutually reinforcing.

An initial list of development items based on these user stories was created. 
Items were initially prioritised based on perceived business and customer value taking into account development dependencies. 
The list of development items is periodically updated, and priorities are reviewed and adjusted as necessary as I learn more 
about the user stories and as my UX knowledge grows during the project.

ID | As a... | I want... | So that...
:-: | --- | --- | --- 
1000 |  Business | to convey our passion for everything guitar | we can capture the customer's attention and get them excited about doing business with us
1010 |  Business | to convey our expertise in all things guitar | we can capture the customer's trust and get them confident about doing business with us
1020 |  Business | to allow a customer to contact us easily from any webpage in the website | we can encourage sales conversion
1030 |  Business | to encourage a customer to visit our website or contact us regularly | we can encourage repeat sales and lifetime customer value
1040 |  Business | to list email, phone, address, facebook as options for contacting  us | customers can contact us using the option most in-line with their preferences
1050 |  Business | to clearly explain how we're operating during the Covid-19 outbreak | we can manage the customer's expectations, capture their trust and get them confident about doing business with us
2000 |  Customer | to know if you are a credible business | I can decide whether or not I can do business with you with confidence
2010 |  Customer | to know if you do in-person guitar lessons | I can know whether or not it makes sense to contact you for lessons
2020 |  Customer | to know if you do on-line guitar lessons | I can know whether or not it makes sense to contact you for lessons
2030 |  Customer | to know the days you do guitar lessons | I can check my schedule before I contact you about lessons
2040 |  Customer | to know how long a guitar lesson lasts | I can check my schedule before I contact you about lessons
2050 |  Customer | to know how much a guitar lesson costs | I can check my budget before I contact you about lessons
2060 |  Customer | to know how to contact you to book guitar lessons | I can contact you about lessons
2070 |  Customer | to know if you can help me pick a guitar | I can know whether or not it makes sense to contact you about a guitar
2080 |  Customer | to know how to contact you about buying a guitar | I can contact you about buying a guitar
2090 |  Customer | to know if you can help me pick accessories | I can contact you about buying accessories
2100 |  Customer | to know how to contact you about buying accessories | I can contact you about buying accessories
2110 |  Customer | to see special offers when I'm on the landing webpage | I can quickly find special offers that are relevant to me
2120 |  Customer | to see a list of all services when I'm on the landing webpage | I can quickly find the services that are relevant to me
2130 |  Customer | to navigate to the landing webpage from any other webpage in the website | I can quickly find the services that are relevant to me
2140 |  Customer | to a single scrollable info webpage per service | it's convenient and easy for me review a service
2150 |  Customer | to navigate to the info webpage for a selected service from any other webpage in the website | I can quickly review the info for that service
2160 |  Customer | to contact you easily from any webpage in the website | it's convenient and easy for me to contact you

### Delivering value

This project implements the beginnings of a simple, but elegant and responsive website for **The Guitar Centre**.

It is created with the future in mind.

Use this section to provide insight into your UX process, focusing on who this website is for, what it is that they want to achieve and how your project is the best way to help them achieve these things.

## Design Paradigm

- Mobile first layout with a single level of responsive design for larger screens when screen width > 576px (i.e. > sm).
- The layout and size of buttons, navigation links and other controls accommodate one-handed navigation.
- The centered horizontal alignment of buttons and navigation links accommodate right-handed and left-handed users.
- The website is simple and consists of a one home (landing) page, two additional (content) pages and a single modal (contact form).
- A simple black and white colour scheme is used. It is functional and provides a tidy and professional appearance.
- As far as possible I try to set sizes with respect to the root em (rem) font-size to support responsiveness.
- My approach is to use the Bootstrap framework and modify templates as opposed to creating from scratch. This is time efficient, avoids unnecessary errors and leverages best practices and existing standards.

## Layout

- Each page follows the same overall layout delimited by semantic elements: `<header>`, `<main>`, and `<footer>`.
- The header and footer are sticky. This is intended so that the mobile user can navigate to content (header) and click to contact (footer) without needing to scroll.
- The footer is slightly unconventional in that it consists of a single button that opens up a contact form modal. The footer floats infront of page content.
- A media rule is used to make main margin-top responsive to the collapsable navbar menu contiained in the header.
- Styling for the header uses Bootstrap classes only.
- Styling for the footer uses Bootstrap classes and custom CSS rules.
- The `<main>` element has padding added using custom CSS rules to accommodate the sticky (collapsable nav menu) header and sticky (floating) footer.
- The app is tested for viewport widths of 320px or more.
- The Header (Navbar) feature is described further below.
- The other minor features are described here:
  - Main
     - The `<main>` element has padding added using custom CSS rules to accommodate the sticky (collapsable nav menu) header and sticky (floating) footer.
     - Set main {margin-bottom: 4.4rem; margin-top: 4.4rem;} so that there is sufficient space top and bottom when the navbar menu is collapsed.
     - Set a media rule to increase the margin-top for larger screens when screen width > 576px (i.e. > sm).
  - Footer
     - Wrap a `<button>` element containing a FontAwesome guitar icon inside a `<div>` element.
     - Add data-bs-toggle and data-bs-target properties to the `<button>` element to control the modal contact form.
     - Add class="btn" and class="btn-dark" to style the button.
     - Add `<i class="fas fa-guitar text-success text-light">` for the FontAweoms guitar icon.
     - Add class="d-flex justify-content-center" to horixontally center the button.
     - Add class="px-3 py-2" so that there is sufficient space around the button and symmetry with the header.
     - Set footer {position: fixed; bottom:0; left:0; right: 0; z-index: 1020;} so that the button is fixed to the bottom and floating infront of other content using custom CSS rules.

## Templates
I make extensive use of the Bootstrap framework and templates.

For layout I use the following components:
  - Grid
  - Utilities

For features I use the following template components:
  - Buttons
  - Card
  - Carousel
  - Modal
  - Navbar

## Customisation

I customsie functional features at the template level by modifying template components:
  - The Carousel is customised by adding controls, captions, crossfade transitions, use containers to control display width, and add anchor tags to create links to additional content pages.
  - The Cards component is customised by various styling classes from the Bootstrap framework.
  - The Navbar component is customised by using the main page heading instead of a button to toggle navigation, and centering nav items in the nav list.
  - The Modal component is customised by changing button configuration, making the phone number automatically dialable and adding a map from Googlemaps.
  
I add, remmove and modify elements, classes, ids and associated attribute-value pairs using HTML and CSS to further cusomise features:

## Features

- __Navbar__

  - Wrap the entire navbar in a `<header>`` element for semantic clarity.
  - Replace id="navbarCollapse" with id="navbarMenu" for semantic clarity.
  - Style using mainly Bootstrap classes as opposed to cutom CSS rules.
  - Add class="navbar-expand-sm" so that nav menu becomes horizontally visible for larger screens when screen width > 576px (i.e. > sm).
  - Add class="flex-column" so that main page heading and nav menu are automatically vertically stacked since the heading is wrapped in `<a>` (inline) and nav items are wrapped in `<div>` (block).
  - Add class="text-center" so that main page heading and nav items are alwys horizontally centered.
  - Add class="fixed-top" so that navbar is sticks to the top and is always visible.
  - Add class="border-bottom" so that navbar and page content are clearly visually separated.
  - Add data-toggle, data-target and aria properties to the main page heading `<h2>` element to control the collapsable nav menu.
  - Add class="nav-link p-0" so that the main page heading styles similarly to the nav items.
  - Add class="p-2" so that nav items are visually sufficiently separated and large enough to tap by finger for mobile users.
  - Set nav {background-color: #fff;} so that navbar is not transparent i.e. covers any content behind it.

![Navbar](https://github.com/oerbeyer/MS1/blob/master/assets/screenshots/D1%20mobile-navbar-expanded.jpg)

- __Carousel__

  - Appears only in the home page. It gives the user an interactive navigation to the relevant service web page.
  - Wrap the entire carousel in a `<div class="container">` element to restrict display width for very wide screens.
  - Remove class=" d-none" and class="d-md-block" so that the slide caption always displays.
  - Remove the `<img>` element and use the background-image attribute.
  - Replace id="carouselExampleCaptions" with id="carousel-home" for semantic clarity.
  - Replace the `<h5>` elements with a more prominent `<h2>` elements in each slide.
  - Add id="slide-workshop" and id="slide-lessons" to each slide to semantically identify each slide, to link with each content page and to set the background-image attribute for each slide using custom CSS rules.
  - Add class="slide-background" and set .slide-background {background-size: cover; background-repeat: no-repeat; background-position: center;} to center and stretch the backgrund image using custom CSS rules.
  - Set a media rule to display an alternative image for larger screens when screen width > 576px (i.e. > sm).
  - Set .carousel-caption {bottom: 5rem; background-color: rgba(0,0,0,0.4); border-radius: 1rem;} to vertically center the caption text, to add contrast between light text and background image, and soften corners of contrast box using custom CSS rules.
  - Set .carousel-caption > * {margin-bottom: 8px;} to remove unnecessary margin from the template using custom CSS rules.
  - Set .carousel-item {height: 18rem;} necessary since there is no `<img>` element to provide a height to each slide using custom CSS rules.

![Carousel](https://github.com/oerbeyer/MS1/blob/master/assets/screenshots/A1%20mobile-home-topscroll.jpg)

- __Clips__

  - Appears only in the home page. It shows the user some inspirational YouTube guitar performer-teacher video clips.
  - Design similar to Header-Section (Feature).
  - Video clips are wrapped in `<iframe>` elements within `<div>` elements with BS embed-responsive classes and modifiers used.

- __Services section__

  - Appears only in the workshop page. It give the use a summary of the web page and directs next steps.
  - Wrap content in `<section>` element for semantic clarity.
  - Wrap section content in `<div class="container">` element to restrict display width for very wide screens.
  - Wrap section content in `<div class="row pt-2">` element for sufficient spacing.
  - Create three card components using the same set of steps, varying only the content and formatting of the card headers.
  - Wrap each card in a `<div class="col-sm-4">` element to respond dynamically to screen width > 576px (i.e. > sm).
  - Add class=" mb-3 mb-sm-0" to all cards but for the last to manage vertical spacing between cards on smaller screens (i.e. < sm) and to maintain alignment of cards on larger scrreens (i.e. > sm).
  - Set .bg-bronze {background-color: #cd7f32;}, .bg-gold {background-color: #ffd700;} and .bg-silver {background-color: #c0c0c0;} to format card header backgrounds using custom CSS rules.
  - Set classes used for styling card body class `<div>` elements identically.  In general, use subtitles to show progression and center text.
  - Set classes used for styling card footer class `<div>` elements identically.  In general, maintain off-white background colour and set price to primary blue colour to attract attention.

![Services](https://github.com/oerbeyer/MS1/blob/master/assets/screenshots/04%20laptop-workshop.jpg)

- __Times section__ 

  - Appears only in the tuition page. It give the use a summary of the available session times and directs next steps.
  - Wrap content in `<section>` element for semantic clarity.
  - Wrap section content in `<div class="container">` element to restrict display width for very wide screens.
  - Wrap section content in `<div class="row pt-2">` element for sufficient spacing.
  - Create a table showing general availability (locations) for days (vertical) and times (horizontal).
  - Add class="table table-sm text-center" and id="table-times-section" to format table contents and uniquely identify table for custom CSS rules.
  - Set a media rule to reduce font size for smaller screens so that table fits to screen width on mobiles when screen width < 576px (i.e. < sm).
  - Add class="bg-primary text-light" and class="bg-success text-light" to `<td>` elements to help the user to visually identify different locations.

![Times](https://github.com/oerbeyer/MS1/blob/master/assets/screenshots/03%20laptop-tuition.jpg)

- __Contact us modal__ 

  - There is an ever present Contact us button at the bottom of the viewport.
  - This opens up a Contact us modal.

![Modal](https://github.com/oerbeyer/MS1/blob/master/assets/screenshots/E1%20mobile-contactus-modal.jpg)

### Future feature development

- I would liek to further develop the Contact us modal to contain an email form submission.

## Project Folder Structure

- The top level project directory contains the .html files for each of the three web pages making up the website along with the readme file: home.html, tuition.html, workshop.html, README.md.
- The /assets sub directory contains its own sub directories for parts of the project.
- The .css stylesheet are contained in the /css sub sub directory.
- The .png image files used in theproject are contained in the /img sub sub directory.
- The .pdf files showing w3c validator passes are contained in the /validators sub sub directory
- The .jpg files showing screenshots for the webpages and the contact us model and contained in the /screenshots sub sub directory.
- There are two sets of screenshots, each numbered in the order that a user is likely to navigate through the pages. The A1 - E1 set is the mobile user journy and screenshots.  The 01 - 05 set is the laptop user journey and screen shots.

## Testing

- I manually test the website. I click through each link in each page checking that it works, and I check that every feature displays and behaves as intended. I use the Chrome DevTools to inspect each page. 
- I toggle the device toolbar and check that each page responds appropriately to all the different breakpoints in protrait and landscape.
- In Chrome DevTools I specifically toggle between Responsive (which I then manually resize) and iPhone 5/SE. The restrictive screen space on the iPhone 5/SE focusses my attention on making sure that the website is truly mobile first friendly.
- In Chrome DevTools I use the Elements and Styles tabs to identify why certain elements were not centering properly and I tested alternative custom CSS rules before adding it to my CSS stylesheet.
- I run all source code through validators. My HTML web pages [W3C validator](https://validator.w3.org/) and my CSS stylesheet [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/). My source code passes validation and I've saved .pdf copies of the results in directory assets/validators.
- I review any warnings to see if there are any potentially material issues that I can solve or easy wins to be had.  There are no material issues or easy wins.

### Validator testing 

- HTML
  - No errors were returned when passing through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Foerbeyer.github.io%2FMS1%2Fhome.html)
- CSS
  - No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fvalidator.w3.org%2Fnu%2F%3Fdoc%3Dhttps%253A%252F%252Foerbeyer.github.io%252FMS1%252Fhome.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en)

### Unfixed bugs

- I review any warnings from validators to see if there are any potentially material issues that I can solve or easy wins to be had.  There are no material issues or easy wins at this time.

## Deployment

This section should describe the process you went through to deploy the project to a hosting platform (e.g. GitHub) 

- The site was deployed to GitHub pages. The steps to deploy are as follows: 
  - In the GitHub repository, navigate to the Settings tab 
  - Click on the Pages link.
  - From the source section drop-down menu, select the Master Branch
  - Once the master branch has been selected, the page will be automatically refreshed with a detailed ribbon display to indicate the successful deployment. 

The live link can be found here - https://oerbeyer.github.io/MS1/home.html 

## Credits 

### Layout & styling

- I make extensive use of the [Bootstrap](https://getbootstrap.com/) framework and templates.
- I use [mdbootstrap](https://mdbootstrap.com/docs/b4/jquery/javascript/google-maps/) as a starting point for creating custom CSS rules specific to Google Maps.

### Content

- The text for the pages are adapteed from the original webpage [sevenoaksguitarcentre.co.uk](https://www.sevenoaksguitarcentre.co.uk/)
- I use free fonts from [fonts.google.com](https://fonts.google.com/)
- I use free icons from [fontawesome.com](https://fontawesome.com)

### Media

- I resize stock images using a free service [picresize.com](https://picresize.com/)
- I use free stock images from [unsplash.com](https://unsplash.com/)
  - Photo by <a href="https://unsplash.com/@krivitskiy?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Alexander Krivitskiy</a> on <a href="https://unsplash.com/s/photos/guitar-female?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  - Photo by <a href="https://unsplash.com/@yirage?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Andriyko Podilnyk</a> on <a href="https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  - Photo by <a href="https://unsplash.com/@carteryocham?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Carter Yocham</a> on <a href="https://unsplash.com/s/photos/workshop-man?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  - Photo by <a href="https://unsplash.com/@angrytortilla?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Joel Drzycimski</a> on <a href="https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  - Photo by <a href="https://unsplash.com/@jonnyswales1989?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Jonny Swales</a> on <a href="https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
- I use videos from [youtube.com](https://youtube.com/)