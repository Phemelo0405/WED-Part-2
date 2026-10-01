# Best Cakes Website - Student Project

## Project Overview
Best Cakes is a non-profit organisation website that provides delicious and affordable cakes to customers and members of the community. This website was developed as part of a Web Development student project.

The goal of the website is to make celebrations special while using cake sales to support community objectives.

## Website Structure

### 1. File Structure
### 2. Pages / Sections Added
The website is a one-page site with anchor navigation:

- **Home (#home)** - Welcome message and call-to-action button "View Our Cakes"
- **About (#about)** - Information about Best Cakes as a non-profit organisation
- **Cakes (#cakes)** - 6 popular cakes with images, descriptions and prices:
    1. Chocolate Cake - R250
    2. Vanilla Cake - R220
    3. Strawberry Cake - R280
    4. Birthday Cake - R300
    5. Red Velvet Cake - R320
    6. Wedding Cake - From R850
- **Special Offers (#offers)** - 3 offer cards added:
    - Birthday Special - FREE message
    - Buy 2 Cakes - FREE Cupcakes
    - Community Special - SAVE 10%
- **Order (#order)** - Enquiry form for customers
- **Contact (#contact)** - Phone, Email and Locations (Johannesburg, Pretoria)
- **Footer** - Copyright and project info

### 3. CSS Features Implemented (Section 2 & 3)

**2.1 External Stylesheet:**
- External CSS file linked: `<link rel="stylesheet" href="CSS/style.css">`
- File named `style.css` inside `CSS/` folder

**2.2 Base Style & Reset:**
- CSS Reset: `* { margin:0; padding:0; box-sizing:border-box; }`
- Base font: Segoe UI, 16px, line-height 1.7
- Colour scheme: Pink (#ff4e8a), white, dark grey
- Background: #fffafc

**2.3 Typography:**
- Headings: Georgia serif, bold
- Body: Segoe UI sans-serif
- Font-size, font-weight, line-height, letter-spacing all set
- Harmonious scale: H1 2.5rem, H2 2.2rem, H3 1.3rem

**2.4 Layout Structure:**
- Flexbox: `display: flex`, `flex-direction`, `justify-content`, `align-items` used in header and nav
- Grid: `display: grid`, `grid-template-columns`, `grid-template-areas` used for cakes and offers
- Desktop: 3-column grid

**2.5 Visual Styles:**
- Colors, background-colors, borders, box-shadows used
- Pseudo-classes: `:hover` on nav and cards, `:focus` on inputs, `:active` on button

**3.1 Breakpoints & Media Queries:**
- Desktop: Default (3 columns)
- Tablet: `@media (max-width: 1024px)` - 2 columns, navigation stacks
- Mobile: `@media (max-width: 768px)` - Single-column layout, vertical navigation
- Small Mobile: `@media (max-width: 480px)` - Smaller fonts

**3.2 Relative Units:**
- `em` used for padding and gap
- `rem` used for font-size, border-radius, height
- `%` used for width (90%, 100%)

**3.3 Responsive Images:**
- CSS: `img { max-width:100%; height:auto; object-fit:cover; }`
- HTML: `srcset` and `sizes` attributes used
- `picture` element used for different screen sizes

### 4. JavaScript Functionality Added

I added JavaScript for **calculation and form validation** in the enquiry form.

**Location:** At the bottom of `index.html` inside `<script>...</script>` before `</body>`

**What the JavaScript does:**

1. **Prevents Past Dates:**
    ```javascript
    dateInput.min = new Date().toISOString().split("T")[0];

    Prevents Page Reload:javascript    event.preventDefault();
