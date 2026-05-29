# Vukani Care NPC — Website Project

**Module:** WEDE5020
**Student Name:** Nceba Nyangiwe
**Student Number:** ST10513411
**Date:** May 2026

---

## Project Overview

This website was built for Vukani Care NPC, a non-profit organisation based in Kokosi, Fochville. The organisation provides HIV/AIDS and tuberculosis (TB) support, education, and home-based care services to the community. Vukani Care was established in 2000 and today has 42 active members coordinating daily community activities including psychological support, HIV testing, health education, and VMMC outreach.

The purpose of this website is to build a credible and professional digital presence that reflects the organisation's values, attracts donors, enables volunteer registration, and serves as a central information hub for the community.

---

## Pages

The website consists of 6 pages:

- Home (index.html) — Landing page with hero image and services overview
- About Us (about.html) — Organisation history, mission, vision, and team targets
- Gallery (gallery.html) — Photo gallery documenting community programmes and impact
- Services (services.html) — HIV/AIDS and TB services offered by the organisation
- Contact Us (contact.html) — Contact form and Google Maps office location embed
- Inquiry (inquiry.html) — Detailed inquiry form with contact information

---

## Part 1 — HTML Structure

All 6 pages were built using semantic HTML5. Every page follows the same structure with a header containing the logo and navigation, a main content section, and a footer with contact information and social media icons.

### Part 1 Feedback Fixes

The following corrections were made to the HTML based on Part 1 feedback:

1. Fixed hearder typo to header on all pages
2. Fixed maim typo to main on gallery.html
3. Fixed unclosed nav and header tags on services.html
4. Fixed buttons tag to button on contact.html
5. Fixed hi tag to li in the team targets list on about.html
6. Fixed missing opening bracket on footer tag in services.html
7. Added alt attributes to all images across all pages for accessibility
8. Removed duplicate Inquiry navigation link from index.html
9. Moved stylesheet link from body to head on all pages
10. Added descriptive title tags to all pages that were missing them
11. Standardised header and footer structure across all 6 pages for consistency
12. Fixed pipe separators in navigation bar to be consistent across all pages
13. Fixed invalid h tag to h1 on inquiry.html for correct heading hierarchy

---

## Part 2 — CSS Styling and Responsive Design

### 2.1 External Stylesheet

A single external CSS file called style.css was created and linked to all 6 HTML pages. This means all pages share the same styles and any change made in style.css applies across the whole website.

The link tag used in the head of every HTML page:

```html
<link rel="stylesheet" href="style.css">
```

### 2.2 Base Styles

A CSS reset was applied using the universal selector to ensure consistent styling across all browsers. CSS variables were defined for the colour scheme, fonts, spacing, and shadows. The base colour scheme uses Forest Green #2E7D32 as the primary colour and Warm White #FAFAFA as the background colour. Default font family, font size, margin, and padding were set on the body element.

### 2.3 Typography

The following typography styles were applied using CSS:

- font-family: Georgia serif for headings, Trebuchet MS sans-serif for body text
- font-size: h1 at 2.4rem, h2 at 1.7rem, h3 at 1.15rem, body text at 1rem
- font-weight: 700 for headings, 400 for body text
- line-height: 1.75 for comfortable reading on all screen sizes
- letter-spacing: applied to navigation links and buttons

### 2.4 Layout Structure

CSS Grid was used with grid-template-areas to structure the overall page layout. The body is divided into four grid areas: header, nav, main, and footer.

```css
body {
  display: grid;
  grid-template-areas:
    "header"
    "nav"
    "main"
    "footer";
}
```

CSS Grid was also used for the gallery grid, service cards, about page mission/vision/targets boxes, and the home page service preview cards. Flexbox was used for the header and navigation bar layout.

CSS properties used: display, flex-direction, justify-content, align-items, grid-template-areas, grid-template-columns, gap

### 2.5 Visual Styles

The following CSS properties were used to style elements visually:

- color — text and heading colours
- background-color — page background, card backgrounds, navigation, and footer
- border — card borders and form input borders
- border-radius — rounded corners on cards, buttons, images, and forms
- box-shadow — depth effect on cards, forms, and images

Pseudo-classes applied:

- :hover — navigation links change background, buttons lift, gallery images scale up, footer icons enlarge
- :focus — form inputs show a green glow outline when selected
- :active — buttons darken when clicked

### 3.1 Breakpoints and Media Queries

Three breakpoints were implemented using media queries to ensure the website works on all screen sizes:

- Desktop: default styles applied above 768px — full multi-column grid layout
- Tablet: max-width 768px — layout switches to single column, font sizes reduce, navigation wraps
- Mobile: max-width 480px — compact layout, full-width buttons, smaller gallery images

The layout switches from a multi-column grid on larger screens to a single-column layout on smaller screens. Font sizes, navigation spacing, and content layout are all modified at each breakpoint.

### 3.2 Relative Units

The following relative units were used throughout the stylesheet:

- rem — all font sizes and spacing values
- em — letter-spacing on navigation and buttons
- % — widths of containers, images, and iframe height using padding-top wrapper
- vh — body min-height and hero image height

### 3.3 Responsive Images

The picture element was used together with srcset and sizes attributes on all images across all pages. This ensures the browser loads the most appropriate image size for the screen being used, which improves performance and load speed.

Example used on the home page hero image:

```html
<picture>
  <source
    srcset="img/hero-large.jpg 1200w, img/hero-medium.jpg 768w, img/hero-small.jpg 480w"
    sizes="(max-width: 480px) 480px, (max-width: 768px) 768px, 1200px">
  <img src="img/hero.jpg" alt="Vukani Care community members working together">
</picture>
```

### 3.4 Testing — Screenshots on Different Devices

The website was tested on desktop, tablet, and mobile screen sizes using browser developer tools in Chrome.

#### Desktop View
<!-- ADD YOUR DESKTOP SCREENSHOT HERE -->
<!-- To add: save your screenshot as screenshots/desktop.png in your repo, then delete this comment and the line will show the image -->
![Desktop View](screenshots/desktop.png)

#### Tablet View
<!-- ADD YOUR TABLET SCREENSHOT HERE -->
<!-- To add: save your screenshot as screenshots/tablet.png in your repo, then delete this comment and the line will show the image -->
![Tablet View](screenshots/tablet.png)

#### Mobile View
<!-- ADD YOUR MOBILE SCREENSHOT HERE -->
<!-- To add: save your screenshot as screenshots/mobile.png in your repo, then delete this comment and the line will show the image -->
![Mobile View](screenshots/mobile.png)

---

## File Structure

```
vukani-website/
│
├── index.html
├── about.html
├── gallery.html
├── services.html
├── contact.html
├── inquiry.html
├── style.css
├── README.md
├── CHANGELOG.md
│
├── img/
│   ├── logo.png
│   ├── hero.jpg
│   ├── facebook.png
│   ├── instagram.png
│   ├── picture1.png
│   ├── picture2.png
│   ├── picture3.png
│   ├── picture4.png
│   ├── picture5.png
│   ├── picture6.png
│   ├── picture7.png
│   └── picture8.png
│
└── screenshots/
    ├── desktop.png
    ├── tablet.png
    └── mobile.png
```

---

## Changelog

All changes made in Part 1 and Part 2 are fully documented in CHANGELOG.md in this repository.

---

## References

Afrihost. (2026). Web hosting plans and pricing. Retrieved from https://www.afrihost.com

Google. (2026). Google Analytics 4 (GA4). Retrieved from https://analytics.google.com

Hetzner South Africa. (2026). Domain and hosting solutions. Retrieved from https://www.hetzner.co.za

MDN Web Docs. (2026). CSS: Cascading Style Sheets. Mozilla. Retrieved from https://developer.mozilla.org/en-US/docs/Web/CSS

MDN Web Docs. (2026). Responsive images. Mozilla. Retrieved from https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images

MDN Web Docs. (2026). CSS Grid Layout. Mozilla. Retrieved from https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout

MDN Web Docs. (2026). Using media queries. Mozilla. Retrieved from https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_media_queries/Using_media_queries

MDN Web Docs. (2026). Flexbox. Mozilla. Retrieved from https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox

South African Department of Health. (2023). National HIV, TB and STI strategic plan 2023-2028. Retrieved from https://www.health.gov.za

Vukani Care NPC. (2025). Organisation profile and community work. Internal document provided for project.

W3Schools. (2026). CSS Tutorial. Retrieved from https://www.w3schools.com/css/

World Wide Web Consortium (W3C). (2018). Web Content Accessibility Guidelines (WCAG) 2.1. Retrieved from https://www.w3.org/TR/WCAG21/