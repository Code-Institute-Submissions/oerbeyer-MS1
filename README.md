# The Guitar Centre

I've chosen to redesign the website for my local guitar shop, [The Guitar Centre](https://www.sevenoaksguitarcentre.co.uk/).

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

[Landing Page](https://github.com/oerbeyer/MS1/blob/master/assets/screenshots/02%20laptop-home-workshop-carousel.jpg)

## Design Paradigm

- Mobile first layout with a single level of responsive design for larger screens when screen width > 576px (i.e. > sm).
- The layout and size of buttons, navigation links and other controls accommodate one-handed navigation.
- The centered horizontal alignment of buttons and navigation links accommodate right-handed and left-handed users.
- The website is simple and consists of a one home (landing) page, two additional (content) pages and a single modal (contact form).
- A simple black and white colour scheme is used. It is functional and provides a tidy and professional appearance.
- As far as possible I try to set sizes with respect to the root em (rem) font-size to support responsiveness.
- My approach is to use the Bootstrap framework and modify templates as opposed to creating from scratch. This is time efficient, avoids unnecessary errors and leverages best practices and existing standards.

## Layout

- Each page follows the same overall layout delimited by semantic elements: <header>, <main>, and <footer>.
- The header and footer are sticky. This is intended so that the mobile user can navigate to content (header) and click to contact (footer) without needing to scroll.
- The footer is slightly unconventional in that it consists of a single button that opens up a contact form modal. The footer floats infront of page content.
- A media rule is used to make main margin-top responsive to the collapsable navbar menu contiained in the header.
- Styling for the header uses Bootstrap classes only.
- Styling for the footer uses Bootstrap classes and custom CSS rules.
- The <main> element has padding added using custom CSS rules to accommodate the sticky (collapsable nav menu) header and sticky (floating) footer.
- The app is tested for viewport widths of 320px or more.

## Templates
I make extensive use of the Bootstrap framework and templates.

For layout I use the following components:
  * Grid
  * Utilities

For features I use the following template components:
  * Buttons
  * Card
  * Carousel
  * Form
  * Modal
  * Navbar

## Customisation:

I customsie functional features at the template level by modifying template components:
- The Carousel is customised by adding controls, captions, crossfade transitions, use containers to control display width, and add anchor tags to create links to additional content pages.
- The Cards component is customised by TODO
- The Navbar component is customised by using the main page heading instead of a button to toggle navigation, and centering nav items in the nav list.
- The Form component is customised by TODO
- The Modal component is customised by TODO
  
I add, remmove and modify elements, classes, ids and associated attribute-value pairs using HTML and CSS to further cusomise features:

## Primary Features 

- __Navbar__

  - Wrap the entire navbar in a <header> element for semantic clarity.
  - Replace id="navbarCollapse" with id="navbarMenu" for semantic clarity.
  - Style using mainly Bootstrap classes as opposed to cutom CSS rules.
  - Add class="navbar-expand-sm" so that nav menu becomes horizontally visible for larger screens when screen width > 576px (i.e. > sm).
  - Add class="flex-column" so that main page heading and nav menu are automatically vertically stacked since the heading is wrapped in <a> (inline) and nav items are wrapped in <div> (block).
  - Add class="text-center" so that main page heading and nav items are alwys horizontally centered.
  - Add class="fixed-top" so that navbar is sticks to the top and is always visible.
  - Add class="border-bottom" so that navbar and page content are clearly visually separated.
  - Add data-toggle, data-target and aria properties to the main page heading <h2> element to control the collapsable nav menu.
  - Add class="nav-link p-0" so that the main page heading styles similarly to the nav items.
  - Add class="p-2" so that nav items are visually sufficiently separated and large enough to tap by finger for mobile users.
  - Set nav {background-color: #fff;} so that navbar is not transparent i.e. covers any content behind it.

![Navbar](https://github.com/oerbeyer/MS1/blob/master/assets/screenshots/D1%20mobile-navbar-expanded.jpg)

- __Carousel__

  - Appears only in the home page. It gives the user an interactive navigation to the relevant service web page.
  - Wrap the entire carousel in a <div class="container"> element to restrict display width for very wide screens.
  - Remove class=" d-none" and class="d-md-block" so that the slide caption always displays.
  - Remove the <img> element and use the background-image attribute.
  - Replace id="carouselExampleCaptions" with id="carousel-home" for semantic clarity.
  - Replace the <h5> elements with a more prominent <h2> elements in each slide.
  - Add id="slide-workshop" and id="slide-lessons" to each slide to semantically identify each slide, to link with each content page and to set the background-image attribute for each slide using custom CSS rules.
  - Add class="slide-background" and set .slide-background {background-size: cover; background-repeat: no-repeat; background-position: center;} to center and stretch the backgrund image using custom CSS rules.
  - Set a media rule to display an alternative image for larger screens when screen width > 576px (i.e. > sm).
  - Set .carousel-caption {bottom: 5rem; background-color: rgba(0,0,0,0.4); border-radius: 1rem;} to vertically center the caption text, to add contrast between light text and background image, and soften corners of contrast box using custom CSS rules.
  - Set .carousel-caption > * {margin-bottom: 8px;} to remove unnecessary margin from the template using custom CSS rules.
  - Set .carousel-item {height: 18rem;} necessary since there is no <img> element to provide a height to each slide using custom CSS rules.

![Carousel](https://github.com/oerbeyer/MS1/blob/master/assets/screenshots/A1%20mobile-home-topscroll.jpg)

- __Clips__

  - Appears only in the home page. It shows the user some inspirational YouTube guitar performer-teacher video clips.
  - Design similar to Header-Section (Feature).
  - Video clips are wrapped in <iframe> elements within <div> elements with BS embed-responsive classes and modifiers used.

- __Services section__

  - Appears only in the workshop page. It give the use a summary of the web page and directs next steps.
  - Wrap content in <section> element for semantic clarity.
  - Wrap section content in <div class="container"> element to restrict display width for very wide screens.
  - Wrap section content in <div class="row pt-2"> element for sufficient spacing.
  - Create three card components using the same set of steps, varying only the content and formatting of the card headers.
  - Wrap each card in a <div class="col-sm-4"> element to respond dynamically to screen width > 576px (i.e. > sm).
  - Add class=" mb-3 mb-sm-0" to all cards but for the last to manage vertical spacing between cards on smaller screens (i.e. < sm) and to maintain alignment of cards on larger scrreens (i.e. > sm).
  - Set .bg-bronze {background-color: #cd7f32;}, .bg-gold {background-color: #ffd700;} and .bg-silver {background-color: #c0c0c0;} to format card header backgrounds using custom CSS rules.
  - Set classes used for styling card body class <div> elements identically.  In general, use subtitles to show progression and center text.
  - Set classes used for styling card footer class <div> elements identically.  In general, maintain off-white background colour and set price to primary blue colour to attract attention.

![Services](https://github.com/oerbeyer/MS1/blob/master/assets/screenshots/04%20laptop-workshop.jpg)

- __Times section__ 

  - Appears only in the tuition page. It give the use a summary of the available session times and directs next steps.
  - Wrap content in <section> element for semantic clarity.
  - Wrap section content in <div class="container"> element to restrict display width for very wide screens.
  - Wrap section content in <div class="row pt-2"> element for sufficient spacing.
  - Create a table showing general availability (locations) for days (vertical) and times (horizontal).
  - Add class="table table-sm text-center" and id="table-times-section" to format table contents and uniquely identify table for custom CSS rules.
  - Set a media rule to reduce font size for smaller screens so that table fits to screen width on mobiles when screen width < 576px (i.e. < sm).
  - Add class="bg-primary text-light" and class="bg-success text-light" to <td> elements to help the user to visually identify different locations.

![Times](https://github.com/oerbeyer/MS1/blob/master/assets/screenshots/03%20laptop-tuition.jpg)

- __Contact us modal__ 

  - There is an ever present Contact us button at the bottom of the viewport.
  - This opens up a Contact us modal.

![Modal](https://github.com/oerbeyer/MS1/blob/master/assets/screenshots/E1%20mobile-contactus-modal.jpg)

### Features Left to Implement

- I would liek to further develop the Contact us modal to contain an email form submission.

## Project Folder Structure

- The top level project directory contains the .html files for each of the three web pages making up the website along with the readme file: home.html, tuition.html, workshop.html, README.md.
- The /assets sub directory contains its own sub directories for parts of the project.
- The .css stylesheet are contained in the /css sub sub directory.
- The .png image files used in theproject are contained in the /img sub sub directory.
- The .pdf files showing w3c validator passes are contained in the /validators sub sub directory
- The .jpg files showing screenshots for the webpages and the contact us model and contained in the /screenshots sub sub directory.
- There are two sets of screenshots, each numbered in the order that a user is likely to navigate through the pages. The A1 - E1 set is the mobile user journy and screenshots.  The 01 - 05 set is the laptop user journey and screen shots.

## Manual Testing

- I manually test the website. I click through each link in each page checking that it works, and I check that every feature displays and behaves as intended. I use the Chrome DevTools to inspect each page. 
- I toggle the device toolbar and check that each page responds appropriately to all the different breakpoints in protrait and landscape.
- In Chrome DevTools I specifically toggle between Responsive (which I then manually resize) and iPhone 5/SE. The restrictive screen space on the iPhone 5/SE focusses my attention on making sure that the website is truly mobile first friendly.
- In Chrome DevTools I use the Elements and Styles tabs to identify why certain elements were not centering properly and I tested alternative custom CSS rules before adding it to my CSS stylesheet.
- I run all source code through validators. My HTML web pages [W3C validator](https://validator.w3.org/) and my CSS stylesheet [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/). My source code passes validation and I've saved .pdf copies of the results in directory assets/validators.
- I review any warnings to see if there are any potentially material issues that I can solve or easy wins to be had.  There are no material issues or easy wins.

### Validator Testing 

- HTML
  - No errors were returned when passing through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Foerbeyer.github.io%2FMS1%2Fhome.html)
- CSS
  - No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fvalidator.w3.org%2Fnu%2F%3Fdoc%3Dhttps%253A%252F%252Foerbeyer.github.io%252FMS1%252Fhome.html&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en)

### Unfixed Bugs

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

### Layout and styling

- I make extensive use of the [Bootstrap](https://getbootstrap.com/) framework and templates.

### Content

- The text for the pages are adapteed from the original webpage [sevenoaksguitarcentre.co.uk](https://www.sevenoaksguitarcentre.co.uk/)
- I use free fonts from [fonts.google.com](https://fonts.google.com/)
- I use free icons from [fontawesome.com](https://fontawesome.com)
- I use [mdbootstrap](https://mdbootstrap.com/docs/b4/jquery/javascript/google-maps/) as a starting point for creating custom CSS rules specific to Google Maps.

### Media

- I resize stock images using a free service [picresize.com](https://picresize.com/)
- I use free stock images from [unsplash.com](https://unsplash.com/)
  - Photo by <a href="https://unsplash.com/@krivitskiy?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Alexander Krivitskiy</a> on <a href="https://unsplash.com/s/photos/guitar-female?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  - Photo by <a href="https://unsplash.com/@yirage?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Andriyko Podilnyk</a> on <a href="https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  - Photo by <a href="https://unsplash.com/@carteryocham?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Carter Yocham</a> on <a href="https://unsplash.com/s/photos/workshop-man?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  - Photo by <a href="https://unsplash.com/@angrytortilla?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Joel Drzycimski</a> on <a href="https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
  - Photo by <a href="https://unsplash.com/@jonnyswales1989?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Jonny Swales</a> on <a href="https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
- I link to videos from [youtube.com](https://youtube.com/)