# Om Luxe Properties - Website

A luxury vacation rental website for "Perch in the Clouds" in Ellijay, GA.

## Folder Structure

```
omluxe/
├── index.html              # Main landing page
├── amenities.html          # Amenities page (placeholder)
├── todo.html               # Things to Do page (placeholder)
├── attractions.html        # Attractions page (placeholder)
├── restaurants.html        # Restaurants page (placeholder)
├── rules.html              # House Rules page (placeholder)
├── howto.html              # How-To Videos page (placeholder)
├── css/
│   └── style.css           # Main stylesheet
├── js/
│   └── script.js           # Main JavaScript file
└── assets/
    └── images/
        ├── logo.png        # Company logo
        └── property/       # Property images folder (add your images here)
```

## Setup Instructions

### 1. Add Property Images

Place your property photos in the `assets/images/property/` folder with the following naming convention:

- `hero-1.jpg` (Main hero image)
- `hero-2.jpg`
- `hero-3.jpg`
- ... up to `hero-15.jpg` (or more)

**Note:** The carousel is set up for 15 slides by default. To add or remove slides:

1. Open `index.html`
2. Find the `<div class="carousel-track">` section
3. Add or remove `<div class="carousel-slide">` blocks as needed

### 2. Update Facebook Link

In each HTML file, find this section in the footer:

```html
<a href="#" target="_blank" rel="noopener noreferrer" aria-label="Follow us on Facebook">
```

Replace `href="#"` with your Facebook page URL.

### 3. Add GHL Contact Form

In each HTML file, find this section:

```html
<div class="contact-form-container">
    <p>&lt;!-- GHL FORM EMBED CODE GOES HERE --&gt;</p>
</div>
```

Replace the `<p>` tag with your GHL form iframe embed code.

### 4. Connect Call Button (Optional)

The "Call Us" button has the ID `callBtn`. You can:
- Add a phone number link: Change the button to an `<a>` tag with `href="tel:+1XXXXXXXXXX"`
- Connect GHL AI Voice: Add the appropriate GHL integration script

## Customization

### Colors

Edit the CSS variables in `css/style.css`:

```css
:root {
    --color-primary-bg: #FFFFFF;
    --color-secondary-bg: #F9F9F9;
    --color-text: #333333;
    --color-accent: #2C5530;  /* Deep Forest Green */
    /* ... more variables */
}
```

### Fonts

The site uses Google Fonts:
- **Headings:** Playfair Display (serif)
- **Body:** Montserrat (sans-serif)

To change fonts, update the `@import` URL at the top of `style.css`.

## Features

- ✅ Responsive design (mobile, tablet, desktop)
- ✅ Image carousel with auto-play, touch/swipe support, keyboard navigation
- ✅ Fixed header with scroll effect
- ✅ Contact modal with GHL form container
- ✅ Mobile hamburger menu
- ✅ Airbnb booking link
- ✅ Property stats section
- ✅ Consistent header/footer across all pages

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome for Android)

## Notes for GHL Integration

This website is designed to be embedded in GoHighLevel funnels. Each page is a standalone HTML file that can be:

1. Uploaded directly to GHL's file hosting
2. Embedded via iframe in GHL funnel pages
3. Hosted externally and linked from GHL

The clean separation of HTML, CSS, and JS files makes it easy to update and maintain.

---

© 2025 Om Luxe Properties LLC
