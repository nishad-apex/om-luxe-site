# Om Luxe Properties Website - Handoff Document

**Last Updated:** January 19, 2026
**Live Site:** https://omluxeproperties.com (deployed via Vercel from GitHub)

---

## What's Completed

### Homepage (index.html)
- Hero video (aerial drone tour, 71MB, compressed 50% quality)
- SVG logo throughout site (sharp at all sizes)
- Navigation menu with all pages
- Contact modal (placeholder for form)
- Footer with social/contact section

### How-To Videos Page (howto.html)
- 5 YouTube video embeds with proper styling:
  - TV & Fireplace
  - Theater Remote
  - Murphy Bed
  - Google Home
  - Basement Shower

### All Pages Have
- Consistent header with logo and navigation
- Mobile-responsive design
- Contact modal (needs form embed)
- Footer (needs Facebook URL)

---

## What Needs to Be Done

### 1. Facebook URL (All Pages)
**Priority:** Medium
**Files:** All 7 HTML files
**Location:** Footer section, line ~159 in each file

Currently the Facebook link goes to `href="#"`. Replace with actual Om Luxe Properties Facebook page URL.

```html
<!-- Find this in footer: -->
<a href="#" target="_blank" rel="noopener noreferrer" aria-label="Follow us on Facebook">

<!-- Change to: -->
<a href="https://facebook.com/YOUR-PAGE-URL" target="_blank" rel="noopener noreferrer" aria-label="Follow us on Facebook">
```

### 2. Contact Form Embed (All Pages)
**Priority:** Medium
**Files:** All 7 HTML files
**Location:** Contact modal section, around line ~190

Currently shows placeholder: `<!-- GHL FORM EMBED CODE GOES HERE -->`

Replace with the GHL (Go High Level) or HubSpot form embed code.

### 3. Amenities Page Content (amenities.html)
**Priority:** High
**Current State:** Shows placeholder

Content needed:
- Hot tub details
- Mountain views
- Fully equipped kitchen
- Bedroom descriptions
- Entertainment systems
- Other amenities

### 4. Things to Do Page Content (todo.html)
**Priority:** High
**Current State:** Shows placeholder

Content needed:
- On-property activities
- Nearby outdoor activities
- Seasonal activities

### 5. Attractions Page Content (attractions.html)
**Priority:** High
**Current State:** Shows placeholder

Content needed:
- Local attractions near Ellijay, GA
- Apple orchards
- Hiking trails
- State parks
- Shopping areas

### 6. Restaurants Page Content (restaurants.html)
**Priority:** High
**Current State:** Shows placeholder

Content needed:
- Local restaurant recommendations
- Categories (casual, fine dining, etc.)
- Approximate distances from property

### 7. House Rules Page Content (rules.html)
**Priority:** High
**Current State:** Shows placeholder

Content needed:
- Check-in/check-out times
- Quiet hours
- Pet policy
- Smoking policy
- Parking information
- Hot tub rules
- Other policies

---

## How to Add Content

### Working with Claude

1. Open a new Claude conversation
2. The MCP server will give Claude context about Om Apex Holdings and pending tasks
3. Simply provide the content text and ask Claude to add it to the appropriate page
4. Example: "Here's the content for the Amenities page: [your text]. Please add this to amenities.html"

### Page Structure

Each content page follows this structure:
```html
<section class="content-section">
    <div class="container">
        <!-- Content goes here -->
    </div>
</section>
```

### Deployment

After making changes:
1. Claude will commit and push to GitHub
2. Vercel automatically deploys from the main branch
3. Changes go live within 1-2 minutes

---

## File Structure

```
om-luxe-site/
├── index.html          # Homepage
├── amenities.html      # Amenities (needs content)
├── todo.html           # Things to Do (needs content)
├── attractions.html    # Attractions (needs content)
├── restaurants.html    # Restaurants (needs content)
├── rules.html          # House Rules (needs content)
├── howto.html          # How-To Videos (complete)
├── css/
│   └── style.css       # All styles
├── js/
│   └── script.js       # Navigation, modal, etc.
└── assets/
    └── images/
        ├── logo.svg    # Main logo (vector)
        ├── logo.png    # Fallback logo
        ├── photos/     # Property photos
        └── videos/
            └── hero/
                └── aerial-drone-tour.mp4  # Hero video
```

---

## Technical Notes

- **Hosting:** Vercel (free tier, auto-deploys from GitHub)
- **Domain:** omluxeproperties.com (connected to Vercel)
- **Repository:** GitHub (Om Luxe site repo)
- **Video:** 71MB compressed, committed directly to repo

---

## Contact

For technical issues, work with Claude who has full context through the MCP server.
