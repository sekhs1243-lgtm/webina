# Webina Website — Quick Edit Guide

This guide explains exactly how and where to update your information, content, images, and contact links in your website.

All website content and configurations are cleanly organized inside [`index.html`](file:///c:/Users/sekhs/Desktop/WebinaFinal/index.html).

---

## 1. Contact & Social Settings (Email, WhatsApp, Phone)

**File:** [`index.html`](file:///c:/Users/sekhs/Desktop/WebinaFinal/index.html#L3995-L4000)  
**Location:** Lines 3995–4000  

```javascript
const contactConfig = {
    businessEmail: "business@webina.agency",       // Business / Quotes / Meetings email
    contactEmail: "webinasolutions@gmail.com",     // General / Legal contact email
    inquiryEmail: "business@webina.agency",        // Project Inquiry form email
    floatingWhatsAppNumber: "+91 6291462207",      // WhatsApp & direct phone number
    whatsappDefaultMessage: "Hi Webina Team! 👋\n\nI'm reaching out from your website. I'm interested in your services and would love to discuss a potential project."
};
```

- **Inquiry & Quote Email (`business@webina.agency`):** Used for project inquiries, custom quotes, and meeting bookings.
- **Privacy & Terms Contact Email (`webinasolutions@gmail.com`):** Listed on Privacy Policy and Terms of Service documents.
- **Floating WhatsApp Number (`+91 6291462207`):** Attached to the floating WhatsApp chat widget and direct phone call links.

---

## 2. Privacy Policy & Terms of Service (Written Text)

**File:** [`index.html`](file:///c:/Users/sekhs/Desktop/WebinaFinal/index.html)  
**Location:** Inside `#legal-modal` (`#legal-privacy-content` and `#legal-terms-content`)

Both Privacy Policy and Terms of Service are formatted as clean, readable text inside the modal. You can edit the numbered clauses directly in the HTML.

---

## 3. Hero Section Typewriter Words

**File:** [`index.html`](file:///c:/Users/sekhs/Desktop/WebinaFinal/index.html#L4012)  
**Location:** Line 4012  

```javascript
const typewriterWords = ["Businesses", "Startups", "Agencies"];
```

- Change or add words to display in the animated hero headline ("Websites for ...").

---

## 4. Portfolio Projects

**File:** [`index.html`](file:///c:/Users/sekhs/Desktop/WebinaFinal/index.html#L4013-L4020)  
**Location:** Lines 4013–4020  

```javascript
const projects = [
    { 
        title: "Restaurant", 
        description: "Elegant dining and culinary showcase website with interactive menu and reservation booking system.", 
        image: "https://images.pexels.com/photos/262978/pexels-photo-262978.jpeg?auto=compress&cs=tinysrgb&w=800&h=600&fit=crop", 
        link: "https://restaurantsampleweb.netlify.app/" 
    },
    // Add, remove, or edit project objects here...
];
```

- **`title`:** Name of the project or industry.
- **`description`:** Short summary displayed on the card.
- **`image`:** Preview image URL (recommended ratio: 4:3 or 16:9, ~800x600px).
- **`link`:** Live preview URL that opens in a new tab when clicked.

---

## 5. Pricing & Service Packages

**File:** [`index.html`](file:///c:/Users/sekhs/Desktop/WebinaFinal/index.html#L4023-L4064)  
**Location:** Lines 4023–4064  

```javascript
const pricingPlans = [
    {
        name: "Starter",
        target: "Ideal for small businesses establishing their initial online presence.",
        price: "",
        subtext: "Delivery Time: 3–4 Days",
        isPopular: false,
        buttonText: "Get Quote",
        buttonLink: "#contact",
        features: [
            "3–5 Page Responsive Website",
            "Mobile-Optimized Design",
            "Integrated WhatsApp Chat Button",
            "Secure Contact Form",
            "Comprehensive Hosting Setup"
        ]
    },
    // Other plans: Business, Shop Management, Custom Web App...
];
```

- **`name`:** Name of the package.
- **`target`:** Audience description.
- **`subtext`:** Delivery timeline or pricing subtitle.
- **`isPopular`:** Set to `true` to highlight with the glowing border and "Most Popular" badge.
- **`features`:** Array of bullet points with checkmark icons.

---

## 6. Global Coverage Countries & Flags

**File:** [`index.html`](file:///c:/Users/sekhs/Desktop/WebinaFinal/index.html#L4067-L4072)  
**Location:** Lines 4067–4072  

```javascript
const servingCountries = [
    { name: "Qatar", flagCode: "qa" },
    { name: "Bahrain", flagCode: "bh" },
    { name: "Singapore", flagCode: "sg" },
    { name: "UAE", flagCode: "ae" },
    { name: "Australia", flagCode: "au" },
    { name: "UK", flagCode: "gb" },
    { name: "USA", flagCode: "us" },
    { name: "Canada", flagCode: "ca" },
    { name: "India", flagCode: "in" },
    { name: "Germany", flagCode: "de" },
    { name: "Malaysia", flagCode: "my" }
];
```

- **`name`:** Display name of the country.
- **`flagCode`:** 2-letter ISO country code (e.g. `us`, `ca`, `gb`, `qa`, `de`, `fr`, `jp`). Flags are rendered automatically via [FlagCDN](https://flagcdn.com).

---

## 7. Technologies & Tools

**File:** [`index.html`](file:///c:/Users/sekhs/Desktop/WebinaFinal/index.html#L4074-L4087)  
**Location:** Lines 4074–4087  

```javascript
const technologies = [
    { name: "HTML5", iconUrl: "https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/html5/html5-original.svg", desc: "Structure & Content." },
    // Add or edit technologies here...
];
```

- Uses standard Devicon vector icons hosted via CDN.

---

## 8. Why Choose Us Highlights

**File:** [`index.html`](file:///c:/Users/sekhs/Desktop/WebinaFinal/index.html#L4089-L4095)  
**Location:** Lines 4089–4095  

```javascript
const whyChooseUsFeatures = [
    { title: "Lightning Fast", description: "We build websites optimized for sub-second load times.", iconSvg: `...` },
    // Edit feature cards here...
];
```

---

## 9. Website Title & SEO Metadata

**File:** [`index.html`](file:///c:/Users/sekhs/Desktop/WebinaFinal/index.html#L10-L20)  
**Location:** Lines 10–20  

- **Title Tag (Line 10):**  
  `<title>Webina | Web Development Company &amp; Custom Web Solutions</title>`
- **Meta Description (Line 11):**  
  `<meta name="description" content="..." />`
- **Keywords (Line 13):**  
  `<meta name="keywords" content="..." />`
- **Canonical URL (Line 20):**  
  `<link rel="canonical" href="https://webinaagency.com/" />`
- **Open Graph / Twitter Cards (Lines 29–50):**  
  Update `og:title`, `og:description`, `og:url`, `og:image` as needed when changing domain or banner image.

---

## 10. Structured Data (JSON-LD)

**File:** [`index.html`](file:///c:/Users/sekhs/Desktop/WebinaFinal/index.html#L64-L181)  
**Location:** Lines 64–181  

Contains Google rich snippet definitions for:
- `WebSite`
- `Organization`
- `ProfessionalService`

Update telephone (`+916291462207`), email (`contact@webinaagency.com`), and address details to match your registered business info.

---

## 11. Favicon

**File:** [`index.html`](file:///c:/Users/sekhs/Desktop/WebinaFinal/index.html#L23-L27)  
**Location:** Lines 23–27  

Currently uses a clean vector SVG Globe icon (`🌐`). To use a custom `.ico` or `.png` file:
```html
<link rel="icon" type="image/png" href="favicon.png" />
<link rel="apple-touch-icon" href="apple-touch-icon.png" />
```

---

## ⚠️ Important Caution: What NOT to Modify Arbitrarily

To ensure the website remains bug-free and responsive:

1. **Do not modify the compiled CSS block** (Lines 184–2913) unless you are familiar with Tailwind CSS utility classes.
2. **Do not delete HTML element IDs** (`id="home"`, `id="booking-modal"`, `id="meeting-modal"`, `id="legal-modal"`, `id="projects-grid"`, etc.) as JavaScript interacts directly with these IDs.
3. **Do not modify core helper functions** (`openBookingModal`, `openMeetingModal`, `playIntro`, `initScrollSpyAndReveal`, `toggleMobileMenu`) unless updating functionality intentionally.
