# Vukani Care NPC — Website

## Project Description

Vukani Care NPC is a non-profit organisation based in Kokosi, Fochville, that provides HIV/AIDS and tuberculosis (TB) support, education, and community development services. This website was built to provide information about the organisation, its services, and how to contact or enquire about their programmes.

---

## Student Information

- Student Name: Nceba Nyangiwe
- Student Number: (add your student number here)
- Module: WEB DEVELOPMENT (INTRODUCTION) — WEDE5020
- Year: 2026

---

## Pages Included

- index.html — Home page with a welcome message, hero image, and services preview
- about.html — About Us page with the organisation history, mission, vision, and team targets
- gallery.html — Gallery page showing photos of community events and programmes
- services.html — Services page with a full list of services and a search and filter feature
- contact.html — Contact page with a contact form and an interactive map
- inquiry.html — Inquiry page with an inquiry form and a smart response system

---

## Technologies Used

- HTML5 for page structure and content
- CSS3 for styling, layout, responsive design, CSS variables, and CSS Grid
- JavaScript (Vanilla JS) for interactivity, form validation, and dynamic content
- Leaflet.js for the interactive map on the Contact page (free, no API key required)
- OpenStreetMap as the map tile provider used with Leaflet
- Font Awesome for icons in the header
- Google Fonts for typography

---

## How to Open and Run the Website

1. Download or clone the repository
2. Extract the folder if it is zipped
3. Open the folder in Visual Studio Code
4. Install the Live Server extension if not already installed
5. Right-click on index.html
6. Select Open with Live Server
7. The website will open in your browser at http://127.0.0.1:5500

---

## Folder Structure

- index.html
- about.html
- contact.html
- gallery.html
- inquiry.html
- services.html
- README.md
- css folder containing styles.css
- js folder containing script.js
- img folder containing all images used on the website

---

## JavaScript Features Added in Part 3

- Active navigation highlight — highlights the current page link in the navigation bar so the user always knows which page they are on
- Back to top button — a button that appears when the user scrolls down and takes them back to the top of the page when clicked
- Accordion — the Mission, Vision, and Team Targets boxes on the About page can be expanded and collapsed by clicking the heading
- Gallery lightbox — clicking any image in the gallery opens it in a full screen overlay with previous and next navigation buttons and a close button
- Dynamic content loading — the services on the Services page are loaded from a JavaScript data array and displayed on the page using DOM manipulation
- Search and filter — users can type a keyword to search and filter the services list in real time
- Interactive map — a Leaflet.js map on the Contact page shows the office location with a clickable marker popup and a Get Directions button
- Form validation on the Inquiry page — validates the full name, email address format, subject, and message fields and shows error messages if the input is incorrect
- Form validation on the Contact page — validates the name and message fields and shows error messages if the input is incorrect
- Thank you response — both forms display a personalised thank you message after the form is successfully submitted
- Smart inquiry response — the inquiry form detects keywords in the subject and message such as volunteer, sponsor, health, and testing and returns a relevant response to the user

---

## SEO Implementation

- Title tags added to all pages
- Meta description tags added to all pages
- Meta keyword tags added to all pages
- Descriptive alt text used on all images
- Proper heading structure using H1, H2, and H3 across all pages
- Internal linking between all pages through the navigation menu
- Mobile friendly responsive design implemented using media queries

---

## Deployment

- Platform: Netlify or GitHub Pages
- Live URL: (add your live link here once deployed)

---

## References

- Leaflet.js Documentation — https://leafletjs.com
- OpenStreetMap — https://www.openstreetmap.org
- Font Awesome — https://fontawesome.com
- MDN Web Docs for HTML, CSS, and JavaScript reference — https://developer.mozilla.org
- W3Schools — https://www.w3schools.com
- Google Fonts — https://fonts.google.com

---

## Changelog

All changes made during Part 3 are recorded below.

---

### Part 3 Changes — June 2026

#### JavaScript Added

- Added active navigation link highlight using JavaScript DOM manipulation (script.js, all HTML files)
- Added back to top button that appears when the user scrolls down (script.js)
- Added accordion feature to Mission, Vision, and Team Targets boxes on the About page (script.js, about.html)
- Added gallery lightbox with previous, next, and close button functionality (script.js, gallery.html)
- Added dynamic content loading where services are rebuilt from a JavaScript data array (script.js, services.html)
- Added real time search and filter for the services list (script.js, services.html)
- Added Leaflet.js interactive map replacing the static iframe on the Contact page (script.js, contact.html)
- Added full form validation to the inquiry form including email format checking and real time error messages (script.js, inquiry.html)
- Added full form validation to the contact form with real time error messages (script.js, contact.html)
- Added personalised thank you response messages to both forms after successful submission (script.js)
- Added smart keyword based response system to the inquiry form (script.js)

#### HTML Fixes from Part 2 Feedback

- Fixed mismatched tags by changing the opening maim tag to main in gallery.html
- Fixed broken input tag in the contact form where the name attribute was not closed properly in contact.html
- Fixed invalid hi tag and changed it to the correct li tag in about.html
- Fixed duplicate closing body tag in index.html
- Fixed buttons tag and changed it to the correct button tag in contact.html
- Moved the CSS link from inside the header to the correct position inside the head tag in inquiry.html
- Added missing main wrapper around sections in index.html
- Added id attributes to contact form fields so JavaScript can target them in contact.html
- Replaced the static Google Maps iframe with a Leaflet map mount point div in contact.html
- Fixed nested section inside section on services.html
- Removed ul tag that was incorrectly wrapped inside a p tag in about.html

#### CSS Additions

- Added styles for the active navigation link highlight
- Added styles for the back to top button
- Added styles for the accordion panels and toggle arrows
- Added styles for the gallery lightbox overlay, enlarged image, caption, and navigation buttons
- Added styles for the services search controls and dynamically loaded service cards
- Added styles for the Leaflet interactive map container and Get Directions button
- Added styles for form field validation states showing valid and invalid highlighting
- Added styles for form response panels covering loading, success, and error states

---

README last updated: June 2026