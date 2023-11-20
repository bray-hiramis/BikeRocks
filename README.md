# BikeRocks
A static website for an imaginary bike shop. This is part of study on learning web development.

# HTML Documentation: BikeRocks Website

# 1. Introduction<a name="introduction"></a>
This HTML document represents the structure of a website for BikeRocks, a platform related to bicycles and biking accessories. The website includes sections for home, bike frames, bike parts, accessories, apparel, and a footer.

# 2. Document Structure<a name="document-structure"></a>
Document Type Declaration (DOCTYPE): Specifies the HTML version and language.
* HTML Element: The root element of the HTML document.
* Head Section: Contains metadata such as character set, viewport settings, and links to stylesheets.
* Body Section: Contains the content of the webpage, including headers, sections, and the footer.
# 3. Header<a name="header"></a>
* Header Element (home-header): Contains the logo and navigation links.
* Logo: BikeRocks logo with a highlighted "Bike" in the text.
* Navigation: Links to different sections of the website.
# 4. Showcase Section<a name="showcase-section"></a>
* Showcase Element: Displays highlighted content with cards for buying, new arrivals, meet-ups, and a blog.
* Card Structure: Each card includes a heading, a brief description, and a button linking to relevant pages.
# 5. Shop Section<a name="shop-section"></a>
* Shop Section: Divided into subsections for bike frames, bike parts, accessories, and apparel.
* Shop Content: Displays images and titles for bike frames, parts, accessories, and apparel.
* Anchor Links: Enable easy navigation to specific sections within the shop.
# 6. Footer<a name="footer"></a>
* Footer Element (main-footer): Contains information about BikeRocks, subscription form, social media links, and copyright details.
* Footer Cards: Divided into sections providing information about BikeRocks, a subscription form, social media links, and copyright details.

# CSS Documentation: BikeRocks Website
This CSS document defines the styling for the BikeRocks website. The styles are organized into sections, each corresponding to different components of the website.

# 1. Global Styles
* Font: The website uses the 'Poppins' font family from Google Fonts with varying weights (300, 400).
* Color Variables: Custom color variables are defined for the primary, secondary, third, light, and dark colors, as well as logo colors in dark and light shades.
* Padding and Margin Variables: Various padding and margin variables are defined for consistent spacing throughout the website.
# 2. Reset Styles
* The * selector resets margin, padding, and sets box-sizing to border-box for all elements.
* html and body elements define basic styling such as line height, font family, background color, and text color.
* Anchor (a) styling removes underlines, sets text color, and makes them inline-block for consistent styling.
* i (icon) styling sets a pointer cursor and reduces opacity on hover.
* Styling for input elements sets them to 100% width.
# 3. Header Styles
* The header section contains styles for the logo and navigation.
* Logo styles include a hover effect with scaling and rotation.
* Navigation links have a hover effect with scaling, a light border-bottom, and a color change.
# 4. Showcase Section Styles
* The showcase section is styled as a grid with three columns.
* Showcase cards have a background image, a dark overlay, and content centered within.
* A hover effect is applied to showcase cards, scaling them slightly.
# 5. Shop Section Styles
* The shop section is styled as a grid with three columns.
* Shop items have a flex display and are centered both horizontally and vertically.
* Images have 100% width and height, with a margin at the bottom.
* Hovering over shop items triggers a scaling effect.
* Specific styles are applied to certain shop items, like larger grid spans and background images.
# 6. Footer Styles
* The footer section has a light background and dark text color.
* Footer content is organized into a three-column grid.
* The logo in the footer has specific styling, including an image with a width of 90px.
* Input styles include padding, border-radius, and a focus outline.
* Social media icons have padding.
* The copyright text is centered.

# CSS Documentation: Styling Guide for BikeRocks Website
This CSS document provides styling guidelines for the BikeRocks website. The stylesheet is organized into sections, including global variables, container styles, utility classes, and specific styles for headings and buttons.

# 1. Global Variables
Colors
--primary-color: Main color used for backgrounds and primary elements.
--secondary-color: Secondary color for additional accents.
--third-color: Third color for buttons and highlighted elements.
--light-color: Light color for text and backgrounds.
--dark-color: Dark color for text and borders.
--logo-color-dark: Dark color variant for logo elements.
--logo-color-light: Light color variant for highlighted logo elements.
Padding and Margin
Padding variables (--pad-large, --pad-mid, --pad-small) control spacing.
Vertical padding variables (--pad-large-vr, --pad-mid-vr, --pad-small-vr) for vertical spacing.
Margin variables (--margin-large-bottom, --margin-mid-bottom, --margin-small-bottom) for bottom margin.
Container Width
--max-width: Maximum width for the container, set to 1150px.
# 2. Container Styles
.container
Centers content using margin: auto.
Sets a maximum width based on the --max-width variable.
# 3. Utility Classes
.txt-highlight
Applies light logo color for highlighting text.
Headings
.large-heading: Styles for large headings, including font size and bottom margin.
.medium-heading: Styles for medium headings, including font size and bottom margin.
Buttons
.btn: Primary button style with padding, background color, and transition effect on hover.
.btn:hover: Hover effect for primary buttons with scaling.
.btn-secondary: Secondary button style with transparent background and border.
.btn-secondary:hover: Hover effect for secondary buttons with background color and no border.
# Example Usage:

```html

<div class="container">
    <h1 class="large-heading txt-highlight">Welcome to BikeRocks</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
    <a href="#" class="btn">Explore Bikes</a>
    <a href="#" class="btn-secondary">Learn More</a>
</div>
```

```css
Copy code
/* Custom styles for specific elements */
.custom-element {
    background: var(--primary-color);
    padding: var(--pad-mid);
    margin-bottom: var(--margin-small-bottom);
}
```

# CSS Responsive Styles Documentation: BikeRocks Website
This CSS documentation outlines the responsive styles for the BikeRocks website, focusing on adjustments made for screens with a maximum width of 800 pixels.

# 1. Responsive Styles Overview
The provided styles are designed to enhance the user experience on smaller screens by adjusting the layout and appearance of key elements.

# 2. Media Query
The @media only screen and (max-width: 800px) media query targets screens with a maximum width of 800 pixels.

# 3. Header Adjustments
.header-items
Flex-direction is changed to column to stack header items vertically.
Justify-content is set to center to center-align items.
# 4. Showcase Section
#showcase
Grid-template-columns is set to 1fr to create a single-column layout.
.showcase-card-1
Grid-column and grid-row are set to 1 to ensure the first showcase card spans the full width.
# 5. Shop Section
#shop-section .shop-content
Grid-template-columns is set to 1fr for a single-column layout.
.shop
Grid-column is set to 1 to ensure each shop item spans the full width.
.shop img
Width and height are set to 400px to control the size of shop item images.
# 6. Footer Adjustments
.footer .footer-card
Grid-column is set to 1 / span 3 to make each footer card span the full width.
Border-bottom is added to create a visual separation between footer cards.
.footer .footer-card:last-child
Removes the border-bottom from the last footer card for a cleaner appearance.
.logo-footer
Justify-content is set to center to center-align items in the logo-footer.
Example Usage:
CSS

```css
@media only screen and (max-width: 800px) {
    /* Responsive styles go here */
    .header-items {
        flex-direction: column;
        justify-content: center;
    }

    #showcase {
        grid-template-columns: 1fr;
    }

    .showcase-card-1 {
        grid-column: 1;
        grid-row: 1;
    }

    #shop-section .shop-content {
        grid-template-columns: 1fr;
    }

    .shop {
        grid-column: 1;
    }

    .shop img {
        width: 400px;
        height: 400px;
    }

    .footer .footer-card {
        grid-column: 1 / span 3;
        border-bottom: 1px var(--dark-color) solid;
    }

    .footer .footer-card:last-child {
        border-bottom: none;
    }

    .logo-footer {
        justify-content: center;
    }
}
```
