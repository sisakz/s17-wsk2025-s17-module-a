# Test Project Outline – Module A – Static Website Design

## Competition time

3 hours

## Introduction

In this module, you must develop a promotional landing site for an online classifieds service. The platform lets users post and browse listings for collectible and themed goods: LEGO sets, board games, comics, figurines, souvenirs, and more.

Your task is to build a modern landing site that presents the service's features and benefits for different user types.

## General Description of Project and Tasks

The landing site must consist of four logically connected pages. Each page must be reachable via navigation, share a consistent style, and display correctly on devices of different sizes.

Please apply SEO optimization and the required meta tags on every page. Configure **OpenGraph** on the website.

Include a **README.md** file with instructions for running the project. In that file, describe how to change the link targets of the `Publish` and `View` buttons.

The following website-wide requirements apply:

- Frameworks are not allowed
- Responsive layout: correct display on devices with different resolutions
- Consistent navigation structure on all pages
- Semantic, clean markup
- Micro-animations on hover for buttons and links
- High-quality typography and readable text
- Correct input field types and valid links

Provided content files are available under `assets/texts/`. Additional images and icons are available under `assets/images/` and `assets/icons/`.

## Requirements

The following pages must be implemented.

### Home Page

Include the following:

- Promo block with the project name, a short description, and a call-to-action
- About the project: goals, audience, platform highlights
- Product categories (`assets/texts/category.txt`)
- Service benefits
- Call-to-action block to engage users
- User testimonials section

### For Seller Page

Include the following:

- Instructions for posting listings. Describe the listing process and how easy it is. Storytelling should be engaging and reflect the service's values (`assets/texts/seller-story.txt`)
- Benefits for sellers (`assets/texts/seller.txt`)
- FAQ section (`assets/texts/seller-faq.txt`)

### For Seller – Price List

Include the following:

- Price list (`assets/texts/seller-price-list.txt`). Let the user choose the number of days to calculate the cost of each service. The user must select the number of days using a `range` input. Prices and day counts are defined in the file.
- Benefits for sellers (`assets/texts/seller-price-list-advantages.txt`)
- FAQ section (`assets/texts/seller-price-list-faq.txt`)

### For Buyer Page

Include the following:

- Step-by-step buying instructions. Describe the purchase process and how easy it is. Storytelling should be engaging and reflect the service's values (`assets/texts/buyer-story.txt`)
- Benefits for buyers (`assets/texts/buyer.txt`)
- FAQ section (`assets/texts/buyer-faq.txt`)

### Contacts

Include the following:

- Contact form (name, email, message)
- Contact details: email, business hours
- Social media links
- Map (`assets/map.png`)

Content is provided in `assets/texts/contacts.txt`.

### Policy

Place the privacy policy text from `assets/texts/policy.txt` on a separate page.

Format the text with HTML elements that ensure readability: headings, paragraphs, lists, and other appropriate markup.

### Global Elements

Every page must include a **header** with:

- Logo
- Navigation
- `Publish` and `View` buttons

These buttons currently link to the `For Seller` and `For Buyer` pages, but it must be easy to change their link targets.

Provide two distinct styles and micro-animations for these buttons; styles must switch based on the `data-type` attribute.

The navigation must include:

- Home
- For Seller
  - Advantages
  - Paid Services
  - FAQ
- For Buyer
  - Advantages
  - FAQ

Every menu item except `Home` has a second-level submenu. It must appear on hover as a separate block.

**JavaScript must not be used** to show the second-level menu.

Implement a footer on every page with navigation and links to other pages.

## Assessment

Module A will be assessed using the latest stable version of Google Chrome and Firefox. HTML and CSS will be assessed using W3C validators (https://validator.w3.org/ and https://jigsaw.w3.org/css-validator/). Accessibility will be tested using the `axe` browser extension installed in Google Chrome to assess that the website is "accessibility supported" according to WCAG.

## Mark distribution

The table below outlines how marks are broken down and how they align with the WorldSkills Occupation Standards (WSOS). Please read the Technical Description for a full explanation of the WorldSkills Occupation Standards.

| WSOS SECTION | Description                            | Points |
| ------------ | -------------------------------------- | ------ |
| 1            | Work organization and self-management  | 0      |
| 2            | Communication and interpersonal skills | 0.5    |
| 3            | Design Implementation                  | 19.5   |
| 4            | Front-End Development                  | 0      |
| 5            | Back-End Development                   | 0      |
|              |                                        |        |
| **Total**    |                                        | 20     |
