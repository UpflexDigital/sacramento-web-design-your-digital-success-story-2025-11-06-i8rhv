# Sacramento Web Design Landing Page - Maintenance & Customization Guide

Welcome! This comprehensive guide will help you maintain, update, and customize your Upflex Digital landing page. Whether you're updating text, fixing links, or adding new pages, this document provides step-by-step instructions tailored to your specific HTML structure.

---

## Table of Contents

1. [Getting Started](#getting-started)
2. [Understanding the Page Structure](#understanding-the-page-structure)
3. [Updating Text Content](#updating-text-content)
4. [Working with Tailwind CSS Classes](#working-with-tailwind-css-classes)
5. [Fixing and Managing Links](#fixing-and-managing-links)
6. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
7. [Mobile Menu Customization](#mobile-menu-customization)
8. [FAQ Section Management](#faq-section-management)
9. [Troubleshooting Guide](#troubleshooting-guide)

---

## Getting Started

### What You Need

- A text editor (we recommend [Visual Studio Code](https://code.visualstudio.com/) - it's free!)
- Your `index.html` file
- Basic understanding of HTML tags (covered below)

### How to Open Your File

1. Right-click on your `index.html` file
2. Select "Open with" → "Visual Studio Code" (or your preferred text editor)
3. The file will open in the editor, ready for editing

### Basic HTML Structure You'll See

```html
<tag>Content goes here</tag>
```

**Example:**
```html
<h1>Sacramento Web Design: Your Digital Success Story</h1>
```

The `<h1>` tags contain your main heading. To change the text, simply replace what's between the tags while keeping the tags themselves intact.

---

## Understanding the Page Structure

Your landing page is organized into distinct sections. Here's a visual breakdown:

```
┌─────────────────────────────────────────┐
│  HEADER (Navigation & Logo)             │
├─────────────────────────────────────────┤
│  HERO SECTION (Main Banner)             │
├─────────────────────────────────────────┤
│  FEATURES SECTION                       │
├─────────────────────────────────────────┤
│  BENEFITS SECTION                       │
├─────────────────────────────────────────┤
│  TESTIMONIALS SECTION                   │
├─────────────────────────────────────────┤
│  CTA SECTION (Call to Action)          │
├─────────────────────────────────────────┤
│  ABOUT US SECTION                       │
├─────────────────────────────────────────┤
│  FAQ SECTION                            │
├─────────────────────────────────────────┤
│  FOOTER                                 │
└─────────────────────────────────────────┘
```

Each section has an ID (like `id="features"`) that allows navigation links to jump directly to that section.

---

## Updating Text Content

### Hero Section (Main Banner)

The hero section is the first large section visitors see. It's located near the top of your HTML file.

#### Updating the Main Heading

**Location:** Search for this text in your file:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight md:leading-tight lg:leading-tight tracking-tight mb-6">
    Sacramento Web Design: Your Digital Success Story
</h1>
```

**To update:**
1. Find the text between `<h1>` and `</h1>`
2. Delete "Sacramento Web Design: Your Digital Success Story"
3. Type your new heading
4. Keep all the `class="..."` attributes exactly as they are

**Example of correct update:**
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight md:leading-tight lg:leading-tight tracking-tight mb-6">
    Your New Heading Here
</h1>
```

#### Updating the Hero Subtitle

**Location:** Find this paragraph in the hero section:
```html
<p class="text-lg md:text-xl text-gray-600 max-w-3xl mx-auto mb-8 leading-relaxed">
    Crafting stunning, high-performing websites to grow your Sacramento business...
</p>
```

**To update:**
1. Find the text between `<p>` and `</p>`
2. Replace with your new description
3. Keep the `class="..."` attributes unchanged

### Features Section

The Features section contains three cards describing your main services.

#### Updating Feature Titles

**Location:** Search for "Responsive Design" (first feature):
```html
<h3 class="text-xl font-bold text-gray-900 mb-3">Responsive Design</h3>
```

**To update:**
1. Replace "Responsive Design" with your new feature title
2. Keep the `<h3>` tags and class attributes

**Repeat this process for:**
- "SEO Optimization" (second feature)
- "Custom Graphics & Design" (third feature)

#### Updating Feature Descriptions

**Location:** Find the paragraph after each feature title:
```html
<p class="text-gray-600 leading-relaxed mb-4">
    Your website looks stunning on every device, from desktop computers to tablets and smartphones...
</p>
```

**To update:**
1. Replace the entire description text
2. Keep the `<p>` tags and all class attributes

#### Updating Feature Bullet Points

**Location:** Find the list items under each feature:
```html
<li class="flex items-start">
    <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
    <span>Mobile-first development approach</span>
</li>
```

**To update:**
1. Find the text between `<span>` and `</span>`
2. Replace with your new bullet point
3. Keep the `<i>` icon tag and all class attributes
4. Keep the `<li>` tags intact

### Benefits Section

This section highlights measurable results.

#### Updating Benefit Cards

**Location:** Find sections starting with "Increased Traffic":
```html
<h3 class="text-2xl font-bold text-gray-900 mb-3">Increased Traffic</h3>
<p class="text-gray-700 leading-relaxed mb-4">
    Watch your website traffic soar with our strategic approach...
</p>
```

**To update:**
1. Change the `<h3>` text for the title
2. Change the `<p>` text for the description
3. Find the statistics line: `<div class="flex items-center text-purple-600 font-semibold">`
4. Update the text after the icon

**Example:**
```html
<div class="flex items-center text-purple-600 font-semibold">
    <i class="fas fa-chart-line mr-2"></i>
    Average 200% traffic increase  <!-- Update this text -->
</div>
```

### Testimonials Section

Update customer testimonials and names.

#### Updating Testimonial Text

**Location:** Find testimonial paragraphs:
```html
<p class="text-gray-700 leading-relaxed mb-6">
    "Upflex Digital completely transformed our online presence..."
</p>
```

**To update:**
1. Replace the quote text between `<p>` and `</p>`
2. Keep the quotation marks if desired
3. Keep all class attributes

#### Updating Customer Names and Titles

**Location:** Find customer information blocks:
```html
<p class="font-bold text-gray-900">Jennifer Martinez</p>
<p class="text-sm text-gray-600">Owner, Martinez Dental Studio</p>
```

**To update:**
1. Replace "Jennifer Martinez" with new name
2. Replace "Owner, Martinez Dental Studio" with new title
3. Keep the `<p>` tags and class attributes

#### Updating Customer Initials

**Location:** Find the avatar circle above the name:
```html
<div class="w-12 h-12 gradient-accent rounded-full flex items-center justify-center text-white font-bold mr-4">
    JM
</div>
```

**To update:**
1. Replace "JM" with the customer's initials
2. Keep everything else the same

### About Us Section

#### Updating Company Description

**Location:** Find the About Us paragraphs:
```html
<p class="text-lg text-gray-700 leading-relaxed">
    Upflex Digital was founded in 2018 by a team of passionate web designers...
</p>
```

**To update:**
1. Replace the paragraph text
2. Keep the `<p>` tags and class attributes
3. Update all paragraphs in this section

#### Updating Statistics

**Location:** Find the statistics grid:
```html
<div class="text-4xl font-bold gradient-accent bg-clip-text text-transparent mb-2">150+</div>
<p class="text-gray-600 font-semibold">Successful Projects</p>
```

**To update:**
1. Replace "150+" with your new number
2. Replace "Successful Projects" with new label
3. Repeat for the other two statistics

### FAQ Section

#### Updating FAQ Questions

**Location:** Find FAQ items:
```html
<button class="faq-question w-full px-6 py-4 flex items-center justify-between hover:bg-gray-50 transition-colors duration-300 cursor-pointer">
    <span class="text-lg font-semibold text-gray-900 text-left">How long does it take to build a website?</span>
```

**To update:**
1. Replace the question text between `<span>` and `</span>`
2. Keep all the surrounding tags and classes

#### Updating FAQ Answers

**Location:** Find the answer sections:
```html
<div class="faq-answer hidden px-6 pb-4 border-t border-gray-200">
    <p class="text-gray-700 leading-relaxed">
        The timeline for building a website depends on the complexity...
    </p>
</div>
```

**To update:**
1. Replace the text between `<p>` and `</p>`
2. Keep all tags and class attributes
3. **Important:** Keep the `hidden` class - it controls whether the answer shows or hides

### Footer Section

#### Updating Footer Company Description

**Location:** Find the footer company info:
```html
<p class="text-gray-400 text-sm leading-relaxed mb-4">
    Crafting stunning, high-performing websites for Sacramento businesses since 2018.
</p>
```

**To update:**
1. Replace the description text
2. Keep the `<p>` tags and class attributes

#### Updating Contact Information

**Location:** Find the contact section:
```html
<p class="font-semibold text-white">Sacramento, CA</p>
<p class="text-gray-400 text-sm">Serving Northern California</p>
```

**To update:**
1. Replace the location and service area
2. Update email and phone information similarly
3. Keep all tags and classes

---

## Working with Tailwind CSS Classes

Your landing page uses **Tailwind CSS**, a utility-first CSS framework. This means styling is controlled through class names rather than separate CSS files.

### Understanding Tailwind Classes

Every class name describes what it does:

| Class | What It Does | Example |
|-------|-------------|---------|
| `text-4xl` | Font size (4xl = extra large) | `<h1 class="text-4xl">` |
| `font-bold` | Makes text bold | `<p class="font-bold">` |
| `text-gray-900` | Text color (dark gray) | `<p class="text-gray-900">` |
| `bg-white` | Background color (white) | `<div class="bg-white">` |
| `px-4` | Horizontal padding | `<div class="px-4">` |
| `py-8` | Vertical padding | `<div class="py-8">` |
| `rounded-lg` | Rounded corners | `<div class="rounded-lg">` |
| `shadow-md` | Drop shadow | `<div class="shadow-md">` |
| `mb-6` | Margin bottom | `<p class="mb-6">` |
| `flex` | Flexbox layout | `<div class="flex">` |
| `grid` | Grid layout | `<div class="grid">` |
| `md:text-5xl` | Responsive - larger on medium+ screens | `<h1 class="md:text-5xl">` |
| `hidden` | Hide element | `<div class="hidden">` |

### Common Responsive Prefixes

Your page uses these breakpoints for responsive design:

- **No prefix** = Mobile phones (default)
- **`sm:`** = Small devices (640px and up)
- **`md:`** = Medium devices (768px and up)
- **`lg:`** = Large devices (1024px and up)

**Example:**
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl">
```

This means:
- On phones: text size is 4xl
- On tablets (md): text size is 5xl
- On desktops (lg): text size is 6xl

### Modifying Colors

Your page uses a purple gradient theme. Here are the key colors:

| Color Class | Used For |
|------------|----------|
| `text-gray-900` | Dark text (headings) |
| `text-gray-600` | Medium text (descriptions) |
| `text-gray-400` | Light text (footer) |
| `text-white` | White text |
| `bg-white` | White background |
| `bg-gray-50` | Light gray background |
| `bg-purple-600` | Purple accent |
| `text-purple-600` | Purple text |
| `gradient-accent` | Purple gradient (custom class) |

#### Changing the Accent Color

If you want to change from purple to a different color, you'll need to:

1. **Find the custom gradient definition** (near the top):
```html
<style>
    .gradient-accent {
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    }
</style>
```

2. **Replace the color codes:**
   - `#667eea` = Light purple
   - `#764ba2` = Dark purple

3. **Use a color picker** like [Coolors.co](https://coolors.co/) to find new hex codes

4. **Example - changing to blue:**
```html
<style>
    .gradient-accent {
        background: linear-gradient(135deg, #3b82f6 0%, #1e40af 100%);
    }
</style>
```

### Modifying Spacing

Spacing classes control margins and padding:

- `m-4` = 4 units of margin on all sides
- `mt-4` = margin on top only
- `mb-4` = margin on bottom only
- `p-8` = 8 units of padding on all sides
- `px-4` = padding on left and right only
- `py-8` = padding on top and bottom only

**Example - increasing space between sections:**

Find:
```html
<section class="py-16 md:py-24">
```

Change to:
```html
<section class="py-20 md:py-32">
```

This increases the vertical padding from 16/24 units to 20/32 units.

### Modifying Text Sizes

Text size classes determine font size:

- `text-sm` = Small (14px)
- `text-base` = Normal (16px)
- `text-lg` = Large (18px)
- `text-xl` = Extra large (20px)
- `text-2xl` = 2x large (24px)
- `text-3xl` = 3x large (30px)
- `text-4xl` = 4x large (36px)
- `text-5xl` = 5x large (48px)
- `text-6xl` = 6x large (60px)

**Example - making hero heading larger:**

Find:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold...">
```

Change to:
```html
<h1 class="text-5xl md:text-6xl lg:text-7xl font-bold...">
```

### Modifying Border Radius (Rounded Corners)

- `rounded-none` = No rounding
- `rounded-sm` = Slightly rounded
- `rounded` = Default rounding
- `rounded-lg` = Large rounding
- `rounded-xl` = Extra large rounding
- `rounded-full` = Completely circular

**Example - making cards more rounded:**

Find:
```html
<div class="... rounded-xl shadow-md...">
```

Change to:
```html
<div class="... rounded-2xl shadow-md...">
```

### Modifying Shadows

Shadow classes add depth:

- `shadow-sm` = Small shadow
- `shadow` = Default shadow
- `shadow-md` = Medium shadow
- `shadow-lg` = Large shadow
- `shadow-xl` = Extra large shadow

---

## Fixing and Managing Links

### Understanding Links in Your Page

Links are created with the `<a>` tag:

```html
<a href="https://upflexdigital.com">Get Started</a>
```

The `href` attribute contains the URL. To change where a link goes, you update this URL.

### Current Links in Your Page

Here's a complete list of all links on your page:

#### Navigation Links (Header)

**Location:** Find the desktop menu section:
```html
<a href="#features" class="text-gray-700 hover:text-purple-600...">Features</a>
<a href="#benefits" class="text-gray-700 hover:text-purple-600...">Benefits</a>
<a href="#testimonials" class="text-gray-700 hover:text-purple-600...">Testimonials</a>
<a href="#faq" class="text-gray-700 hover:text-purple-600...">FAQ</a>
<a href="#about" class="text-gray-700 hover:text-purple-600...">About</a>
```

**What they do:** These links jump to different sections on the same page (notice the `#` symbol).

**Status:** ✅ These are working correctly and shouldn't be changed unless you rename sections.

#### Call-to-Action Links

**Location:** Find "Get Started" buttons throughout the page:
```html
<a href="https://upflexdigital.com" class="gradient-accent text-white px-6 py-2...">
    Get Started
</a>
```

**Current URL:** `https://upflexdigital.com`

**Status:** ⚠️ **This needs to be updated** to your actual website URL.

**To update:**
1. Find all instances of `href="https://upflexdigital.com"`
2. Replace with your actual URL (e.g., `https://yourcompany.com`)
3. Keep the quotes around the URL

**How many to update:** Search for "upflexdigital.com" - you'll find approximately 8-10 instances.

#### Email Link

**Location:** Find the email link:
```html
<a href="mailto:info@upflexdigital.com" class="border-2 border-white text-white...">
    Email Us
</a>
```

Also in footer:
```html
<a href="mailto:info@upflexdigital.com" class="text-gray-400 hover:text-purple-400...">info@upflexdigital.com</a>
```

**Status:** ⚠️ **This needs to be updated** to your email address.

**To update:**
1. Find `mailto:info@upflexdigital.com`
2. Replace with your email: `mailto:your-email@yourcompany.com`

**Important:** Keep the `mailto:` part - it tells the browser to open the email client.

#### Footer Links

**Location:** Find the footer navigation sections:

```html
<!-- Services Links -->
<li><a href="#features" class="text-gray-400 hover:text-purple-400...">Web Design</a></li>
<li><a href="#features" class="text-gray-400 hover:text-purple-400...">SEO Optimization</a></li>
<li><a href="#features" class="text-gray-400 hover:text-purple-400...">Branding</a></li>
<li><a href="#" class="text-gray-400 hover:text-purple-400...">E-commerce</a></li>
<li><a href="#" class="text-gray-400 hover:text-purple-400...">Maintenance</a></li>

<!-- Company Links -->
<li><a href="#about" class="text-gray-400 hover:text-purple-400...">About Us</a></li>
<li><a href="#testimonials" class="text-gray-400 hover:text-purple-400...">Testimonials</a></li>
<li><a href="blog.html" class="text-gray-400 hover:text-purple-400...">Blog</a></li>
<li><a href="#faq" class="text-gray-400 hover:text-purple-400...">FAQ</a></li>
<li><a href="https://upflexdigital.com" class="text-gray-400 hover:text-purple-400...">Contact</a></li>

<!-- Legal Links -->
<li><a href="privacy.html" class="text-gray-400 hover:text-purple-400...">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-purple-400...">Terms of Service</a></li>
<li><a href="#" class="text-gray-400 hover:text-purple-400...">Cookie Policy</a></li>
<li><a href="#" class="text-gray-400 hover:text-purple-400...">Disclaimer</a></li>
```

**Status:** ⚠️ **Several need updating:**
- `blog.html` - needs to point to your blog
- `privacy.html` - needs to be created or updated
- `terms.html` - needs to be created or updated
- `#` links - placeholder links that need real URLs

### Step-by-Step: Update All Links

#### Step 1: Update Main Website URLs

**Find:** All instances of `href="https://upflexdigital.com"`

**Replace with:** Your website URL (e.g., `href="https://mycompany.com"`)

**Locations:**
- Header "Get Started" button (desktop)
- Header "Get Started" button (mobile menu)
- Hero section "Start Your Project Today" button
- Hero section "Learn More" button (internal link - don't change)
- CTA section "Get Your Free Consultation" button
- Footer "Contact" link

**Using Find & Replace (Easiest Method):**
1. Press `Ctrl+H` (Windows) or `Cmd+H` (Mac)
2. In "Find" field: `https://upflexdigital.com`
3. In "Replace" field: `https://yourcompany.com`
4. Click "Replace All"

#### Step 2: Update Email Address

**Find:** All instances of `mailto:info@upflexdigital.com`

**Replace with:** `mailto:your-email@yourcompany.com`

**Locations:**
- CTA section "Email Us" button
- Footer contact information

**Using Find & Replace:**
1. Press `Ctrl+H` (Windows) or `Cmd+H` (Mac)
2. In "Find" field: `info@upflexdigital.com`
3. In "Replace" field: `your-email@yourcompany.com`
4. Click "Replace All"

#### Step 3: Update Service Links

If you have service pages, update these:

**Find:**
```html
<li><a href="#" class="text-gray-400 hover:text-purple-400...">E-commerce</a></li>
<li><a href="#" class="text-gray-400 hover:text-purple-400...">Maintenance</a></li>
```

**Replace with:**
```html
<li><a href="services/ecommerce.html" class="text-gray-400 hover:text-purple-400...">E-commerce</a></li>
<li><a href="services/maintenance.html" class="text-gray-400 hover:text-purple-400...">Maintenance</a></li>
```

Or link to external pages:
```html
<li><a href="https://yourcompany.com/services/ecommerce" class="text-gray-400 hover:text-purple-400...">E-commerce</a></li>
```

#### Step 4: Update Blog Link

**Find:**
```html
<li><a href="blog.html" class="text-gray-400 hover:text-purple-400...">Blog</a></li>
```

**Replace with:**
```html
<li><a href="https://yourcompany.com/blog" class="text-gray-400 hover:text-purple-400...">Blog</a></li>
```

Or if you have a local `blog.html` file:
```html
<li><a href="blog.html" class="text-gray-400 hover:text-purple-400...">Blog</a></li>
```

Also update in footer copyright:
```html
<a href="blog.html" class="hover:text-purple-400 transition-colors duration-300">Blog</a>
```

### Verifying Links Work

After updating links:

1. **Save your file** (Ctrl+S or Cmd+S)
2. **Open your page in a browser**
3. **Test each link:**
   - Click navigation items (should jump to sections)
   - Click "Get Started" buttons (should go to your website)
   - Click "Email Us" (should open email client)
   - Click footer links (should work appropriately)

**If a link doesn't work:**
- Check that the URL is spelled correctly
- Make sure external URLs include `https://`
- Make sure internal links start with `#` or have the correct filename
- Check that files exist (blog.html, privacy.html, etc.)

---

## Adding Privacy and Terms Pages

Your landing page references `privacy.html` and `terms.html` files, but these files don't exist yet. Here's how to create them.

### Step 1: Create the Privacy Policy Page

#### Create the File

1. Open your text editor
2. Create a new file: File → New File
3. Save it as `privacy.html` in the same folder as your `index.html`

#### Add the Basic HTML Structure

Copy and paste this template into your new `privacy.html` file:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy - Upflex Digital">
    <meta name="author" content="Upflex Digital">
    <title>Privacy Policy - Upflex Digital</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        html {
            scroll-behavior: smooth;
        }
        .gradient-accent {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
    </style>
</head>
<body class="bg-white text-gray-900">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <div class="w-10 h-10 gradient-accent rounded-lg flex items-center justify-center text-white font-bold text-lg">
                    UD
                </div>
                <span class="font-bold text-xl text-gray-900 hidden sm:inline">Upflex Digital</span>
            </div>
            <a href="index.html" class="text-gray-700 hover:text-purple-600 font-medium transition-colors duration-300">
                Back to Home
            </a>
        </nav>
    </header>

    <!-- Main Content -->
    <main class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 py-16 md:py-24">
        <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8">Privacy Policy</h1>
        
        <div class="prose prose-lg max-w-none text-gray-700 space-y-6">
            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">1. Introduction</h2>
                <p>
                    Upflex Digital ("Company," "we," "our," or "us") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you visit our website, including any other media form, media channel, mobile website, or mobile application related to, operated, or connected therewith (collectively, the "Site").
                </p>
                <p>
                    Please read this privacy policy carefully. If you do not agree with our policies and practices, please do not use our Site. By accessing or using Upflex Digital, you acknowledge that you have read, understood, and agree to be bound by all the provisions of this Privacy Policy.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">2. Information We Collect</h2>
                <p>
                    We may collect information about you in a variety of ways. The information we may collect on the Site includes:
                </p>
                <ul class="list-disc pl-6 space-y-2">
                    <li><strong>Personal Data:</strong> Name, email address, phone number, and any other information you voluntarily provide when contacting us.</li>
                    <li><strong>Derivative Data:</strong> Information our servers automatically collect when you access the Site, such as your IP address, browser type, operating system, and referring URLs.</li>
                    <li><strong>Financial Data:</strong> Financial information, such as data related to your payment method, if you make a purchase.</li>
                    <li><strong>Data from Third Parties:</strong> Information from third parties, including but not limited to marketing partners and analytics providers.</li>
                </ul>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">3. Use of Your Information</h2>
                <p>
                    Having accurate information about you permits us to provide you with a smooth, efficient, and customized experience. Specifically, we may use information collected about you via the Site to:
                </p>
                <ul class="list-disc pl-6 space-y-2">
                    <li>Generate a personal profile about you so that future visits to the Site will be personalized.</li>
                    <li>Increase the efficiency and operation of the Site.</li>
                    <li>Monitor and analyze usage and trends to improve your experience with the Site.</li>
                    <li>Notify you of updates to the Site.</li>
                    <li>Offer new products, services, and/or recommendations to you.</li>
                </ul>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">4. Disclosure of Your Information</h2>
                <p>
                    We may share your information in the following situations:
                </p>
                <ul class="list-disc pl-6 space-y-2">
                    <li><strong>By Law or to Protect Rights:</strong> If we believe the release of information is necessary to comply with the law, enforce our Site policies, or protect ours or others' rights, property, and safety.</li>
                    <li><strong>Third-Party Service Providers:</strong> We may share your information with third parties that perform services for us, including payment processors, hosting providers, and customer service platforms.</li>
                    <li><strong>Business Transfers:</strong> Your information may be transferred as part of our business assets if we are acquired or merged with another entity.</li>
                </ul>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">5. Security of Your Information</h2>
                <p>
                    We use administrative, technical, and physical security measures to protect your personal information. However, no method of transmission over the Internet or method of electronic storage is 100% secure. While we strive to use commercially acceptable means to protect your personal information, we cannot guarantee its absolute security.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">6. Contact Us</h2>
                <p>
                    If you have questions or comments about this Privacy Policy, please contact us at:
                </p>
                <div class="bg-gray-50 p-6 rounded-lg mt-4">
                    <p><strong>Upflex Digital</strong></p>
                    <p>Sacramento, CA</p>
                    <p>Email: <a href="mailto:info@upflexdigital.com" class="text-purple-600 hover:text-purple-700">info@upflexdigital.com</a></p>
                </div>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">7. Updates to This Privacy Policy</h2>
                <p>
                    We may update this Privacy Policy from time to time to reflect changes in our practices, technology, legal requirements, or other factors. We will notify you by updating the "Last Updated" date of this Privacy Policy. Your continued use of the Site following the posting of a revised Privacy Policy means that you accept and agree to the changes.
                </p>
                <p class="text-sm text-gray-600 mt-4">
                    <strong>Last Updated:</strong> January 2025
                </p>
            </section>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-8 mt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-gray-400 text-sm">
                &copy; 2025 Upflex Digital. All rights reserved.
            </p>
        </div>
    </footer>
</body>
</html>
```

#### Customize the Privacy Policy

1. **Update company information:**
   - Find: `Upflex Digital`
   - Replace with: Your company name

2. **Update contact information:**
   - Find: `Sacramento, CA`
   - Replace with: Your location
   - Find: `info@upflexdigital.com`
   - Replace with: Your email

3. **Add your specific policies:**
   - Review each section
   - Update to reflect your actual practices
   - Add or remove sections as needed

4. **Save the file:**
   - Press `Ctrl+S` (Windows) or `Cmd+S` (Mac)

### Step 2: Create the Terms of Service Page

#### Create the File

1. Open your text editor
2. Create a new file: File → New File
3. Save it as `terms.html` in the same folder as your `index.html`

#### Add the Basic HTML Structure

Copy and paste this template into your new `terms.html` file:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service - Upflex Digital">
    <meta name="author" content="Upflex Digital">
    <title>Terms of Service - Upflex Digital</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        html {
            scroll-behavior: smooth;
        }
        .gradient-accent {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
    </style>
</head>
<body class="bg-white text-gray-900">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <div class="w-10 h-10 gradient-accent rounded-lg flex items-center justify-center text-white font-bold text-lg">
                    UD
                </div>
                <span class="font-bold text-xl text-gray-900 hidden sm:inline">Upflex Digital</span>
            </div>
            <a href="index.html" class="text-gray-700 hover:text-purple-600 font-medium transition-colors duration-300">
                Back to Home
            </a>
        </nav>
    </header>

    <!-- Main Content -->
    <main class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 py-16 md:py-24">
        <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8">Terms of Service</h1>
        
        <div class="prose prose-lg max-w-none text-gray-700 space-y-6">
            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">1. Agreement to Terms</h2>
                <p>
                    These Terms of Service ("Terms") constitute a legally binding agreement between you and Upflex Digital ("Company," "we," "our," or "us") concerning your use of our website and services (collectively, the "Services"). By accessing and using our website, you acknowledge that you have read, understood, and agree to be bound by all the provisions of these Terms of Service.
                </p>
                <p>
                    If you do not agree with any part of these Terms, you may not use our Services. We reserve the right to modify these Terms at any time. Your continued use of the Services following any changes constitutes your acceptance of the new Terms.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">2. Use License</h2>
                <p>
                    Permission is granted to temporarily download one copy of the materials (information or software) on Upflex Digital's website for personal, non-commercial transitory viewing only. This is the grant of a license, not a transfer of title, and under this license you may not:
                </p>
                <ul class="list-disc pl-6 space-y-2">
                    <li>Modify or copy the materials</li>
                    <li>Use the materials for any commercial purpose or for any public display</li>
                    <li>Attempt to decompile or reverse engineer any software contained on the website</li>
                    <li>Remove any copyright or other proprietary notations from the materials</li>
                    <li>Transfer the materials to another person or "mirror" the materials on any other server</li>
                    <li>Violate any applicable laws or regulations</li>
                </ul>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">3. Disclaimer</h2>
                <p>
                    The materials on Upflex Digital's website are provided on an 'as is' basis. Upflex Digital makes no warranties, expressed or implied, and hereby disclaims and negates all other warranties including, without limitation, implied warranties or conditions of merchantability, fitness for a particular purpose, or non-infringement of intellectual property or other violation of rights.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">4. Limitations</h2>
                <p>
                    In no event shall Upflex Digital or its suppliers be liable for any damages (including, without limitation, damages for loss of data or profit, or due to business interruption) arising out of the use or inability to use the materials on Upflex Digital's website, even if Upflex Digital or an authorized representative has been notified orally or in writing of the possibility of such damage.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">5. Accuracy of Materials</h2>
                <p>
                    The materials appearing on Upflex Digital's website could include technical, typographical, or photographic errors. Upflex Digital does not warrant that any of the materials on its website are accurate, complete, or current. Upflex Digital may make changes to the materials contained on its website at any time without notice.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">6. Links</h2>
                <p>
                    Upflex Digital has not reviewed all of the sites linked to its website and is not responsible for the contents of any such linked site. The inclusion of any link does not imply endorsement by Upflex Digital of the site. Use of any such linked website is at the user's own risk.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">7. Modifications</h2>
                <p>
                    Upflex Digital may revise these Terms of Service for its website at any time without notice. By using this website, you are agreeing to be bound by the then current version of these Terms of Service.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">8. Governing Law</h2>
                <p>
                    These Terms and Conditions are governed by and construed in accordance with the laws of the State of California, United States, and you irrevocably submit to the exclusive jurisdiction of the courts in that location.
                </p>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">9. Contact Information</h2>
                <p>
                    If you have any questions about these Terms of Service, please contact us at:
                </p>
                <div class="bg-gray-50 p-6 rounded-lg mt-4">
                    <p><strong>Upflex Digital</strong></p>
                    <p>Sacramento, CA</p>
                    <p>Email: <a href="mailto:info@upflexdigital.com" class="text-purple-600 hover:text-purple-700">info@upflexdigital.com</a></p>
                </div>
            </section>

            <section>
                <h2 class="text-2xl font-bold text-gray-900 mt-8 mb-4">10. Entire Agreement</h2>
                <p>
                    These Terms of Service constitute the entire agreement between you and Upflex Digital regarding your use of the website and supersede all prior and contemporaneous agreements, whether written or oral.
                </p>
                <p class="text-sm text-gray-600 mt-4">
                    <strong>Last Updated:</strong> January 2025
                </p>
            </section>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-8 mt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-gray-400 text-sm">
                &copy; 2025 Upflex Digital. All rights reserved.
            </p>
        </div>
    </footer>
</body>
</html>
```

#### Customize the Terms of Service

1. **Update company information:**
   - Find: `Upflex Digital`
   - Replace with: Your company name

2. **Update contact information:**
   - Find: `Sacramento, CA`
   - Replace with: Your location
   - Find: `info@upflexdigital.com`
   - Replace with: Your email

3. **Update jurisdiction:**
   - Find: `State of California, United States`
   - Replace with: Your jurisdiction

4. **Add your specific terms:**
   - Review each section
   - Update to reflect your actual business practices
   - Add or remove sections as needed

5. **Save the file:**
   - Press `Ctrl+S` (Windows) or `Cmd+S` (Mac)

### Step 3: Verify Links Work

Now that you've created the policy pages:

1. **Open your `index.html` in a browser**
2. **Scroll to the footer**
3. **Click on "Privacy Policy"** - it should load `privacy.html`
4. **Click on "Terms of Service"** - it should load `terms.html`
5. **Click "Back to Home"** on each policy page - should return to `index.html`

**If links don't work:**
- Make sure all three files (`index.html`, `privacy.html`, `terms.html`) are in the same folder
- Check that filenames match exactly (lowercase, no spaces)
- Try refreshing your browser

### Step 4: Update Policy Pages Later

When you want to update your privacy policy or terms:

1. Open `privacy.html` or `terms.html` in your editor
2. Find the section you want to change
3. Update the text
4. Save the file
5. Refresh your browser to see changes

---

## Mobile Menu Customization

Your landing page has a mobile menu that appears on small screens. Here's how to customize it.

### Understanding the Mobile Menu

The mobile menu consists of three parts:

1. **Menu Button** (hamburger icon)
2. **Menu Container** (hidden by default)
3. **Menu Links** (navigation items)

### Current Mobile Menu Structure

**Location:** Find the mobile menu button in the header:

```html
<!-- Mobile Menu Button -->
<button class="md:hidden mobile-menu-button p-2 rounded-lg hover:bg-gray-100 transition-colors duration-300">
    <i class="fas fa-bars text-gray-900 text-xl"></i>
</button>

<!-- Mobile Menu -->
<div class="mobile-menu hidden absolute top-full left-0 right-0 bg-white border-t border-gray-200 md:hidden shadow-lg">
    <div class="flex flex-col space-y-4 px-4 py-6">
        <a href="#features" class="text-gray-700 hover:text-purple-600 font-medium transition-colors duration-300">Features</a>
        <a href="#benefits" class="text-gray-700 hover:text-purple-600 font-medium transition-colors duration-300">Benefits</a>
        <a href="#testimonials" class="text-gray-700 hover:text-purple-600 font-medium transition-colors duration-300">Testimonials</a>
        <a href="#faq" class="text-gray-700 hover:text-purple-600 font-medium transition-colors duration-300">FAQ</a>
        <a href="#about" class="text-gray-700 hover:text-purple-600 font-medium transition-colors duration-300">About</a>
        <a href="https://upflexdigital.com" class="gradient-accent text-white px-6 py-2 rounded-lg font-semibold text-center button-hover hover:shadow-lg">
            Get Started
        </a>
    </div>
</div>
```

### Adding a New Menu Item

To add a new link to the mobile menu:

1. **Find the mobile menu section** (shown above)
2. **Locate the last link before the "Get Started" button**
3. **Add a new line after it:**

```html
<a href="#your-section" class="text-gray-700 hover:text-purple-600 font-medium transition-colors duration-300">Your Link Text</a>
```

**Example - adding a "Services" link:**

```html
<a href="#about" class="text-gray-700 hover:text-purple-600 font-medium transition-colors duration-300">About</a>
<a href="#services" class="text-gray-700 hover:text-purple-600 font-medium transition-colors duration-300">Services</a>
<a href="https://upflexdigital.com" class="gradient-accent text-white px-6 py-2 rounded-lg font-semibold text-center button-hover hover:shadow-lg">
    Get Started
</a>
```

### Changing Mobile Menu Colors

**Find the mobile menu container:**
```html
<div class="mobile-menu hidden absolute top-full left-0 right-0 bg-white border-t border-gray-200 md:hidden shadow-lg">
```

**To change:**
- **Background color:** Replace `bg-white` with another color (e.g., `bg-gray-50`)
- **Border color:** Replace `border-gray-200` with another color (e.g., `border-gray-300`)
- **Shadow:** Replace `shadow-lg` with another shadow size (e.g., `shadow-md`, `shadow-xl`)

**Example - darker background:**
```html
<div class="mobile-menu hidden absolute top-full left-0 right-0 bg-gray-900 border-t border-gray-800 md:hidden shadow-lg">
```

### Changing Link Colors in Mobile Menu

**Find the menu links:**
```html
<a href="#features" class="text-gray-700 hover:text-purple-600 font-medium transition-colors duration-300">Features</a>
```

**To change:**
- **Text color:** Replace `text-gray-700` with another color (e.g., `text-gray-900`)
- **Hover color:** Replace `hover:text-purple-600` with another color (e.g., `hover:text-blue-600`)

**Example - white text for dark background:**
```html
<a href="#features" class="text-white hover:text-purple-300 font-medium transition-colors duration-300">Features</a>
```

### How the Mobile Menu Works (JavaScript)

The mobile menu uses JavaScript to toggle visibility. Here's what happens:

```javascript
// When hamburger button is clicked
mobileMenuButton.addEventListener('click', () => {
    mobileMenu.classList.toggle('hidden');  // Shows/hides menu
    const icon = mobileMenuButton.querySelector('i');
    if (icon) {
        icon.classList.toggle('fa-bars');   // Changes icon from ☰ to ✕
        icon.classList.toggle('fa-times');
    }
});

// When a menu link is clicked
mobileMenuLinks.forEach(link => {
    link.addEventListener('click', () => {
        mobileMenu.classList.add('hidden');  // Closes menu
        const icon = mobileMenuButton.querySelector('i');
        if (icon) {
            icon.classList.remove('fa-times');
            icon.classList.add('fa-bars');   // Changes icon back to ☰
        }
    });
});
```

**Important:** Don't modify this JavaScript unless you're comfortable with code. The mobile menu relies on these specific class names and functions.

---

## FAQ Section Management

Your FAQ section uses an accordion system where clicking a question reveals the answer. Here's how to manage it.

### Understanding the FAQ Structure

Each FAQ item has this structure:

```html
<div class="faq-item bg-white rounded-lg border border-gray-200 overflow-hidden">
    <!-- The Question (clickable button) -->
    <button class="faq-question w-full px-6 py-4 flex items-center justify-between hover:bg-gray-50 transition-colors duration-300 cursor-pointer">
        <span class="text-lg font-semibold text-gray-900 text-left">Your Question Here?</span>
        <i class="faq-icon fas fa-chevron-down text-purple-600 transition-transform duration-300"></i>
    </button>
    
    <!-- The Answer (hidden by default) -->
    <div class="faq-answer hidden px-6 pb-4 border-t border-gray-200">
        <p class="text-gray-700 leading-relaxed">
            Your answer goes here.
        </p>
    </div>
</div>
```

### Adding a New FAQ Item

To add a new question and answer:

1. **Find the last FAQ item** in your HTML
2. **After the closing `</div>` of the last item, add:**

```html
<!-- FAQ Item 6 -->
<div class="faq-item bg-white rounded-lg border border-gray-200 overflow-hidden">
    <button class="faq-question w-full px-6 py-4 flex items-center justify-between hover:bg-gray-50 transition-colors duration-300 cursor-pointer">
        <span class="text-lg font-semibold text-gray-900 text-left">Your New Question Here?</span>
        <i class="faq-icon fas fa-chevron-down text-purple-600 transition-transform duration-300"></i>
    </button>
    <div class="faq-answer hidden px-6 pb-4 border-t border-gray-200">
        <p class="text-gray-700 leading-relaxed">
            Your answer text goes here. You can make it as long as needed.
        </p>
    </div>
</div>
```

3. **Save your file**

The JavaScript will automatically make this new item work with the accordion functionality.

### Editing Existing FAQ Items

#### Changing a Question

**Find:**
```html
<span class="text-lg font-semibold text-gray-900 text-left">How long does it take to build a website?</span>
```

**Replace the text between `<span>` and `</span>`:**
```html
<span class="text-lg font-semibold text-gray-900 text-left">What is your design process?</span>
```

#### Changing an Answer

**Find:**
```html
<div class="faq-answer hidden px-6 pb-4 border-t border-gray-200">
    <p class="text-gray-700 leading-relaxed">
        The timeline for building a website depends on the complexity...
    </p>
</div>
```

**Replace the text between `<p>` and `</p>`:**
```html
<div class="faq-answer hidden px-6 pb-4 border-t border-gray-200">
    <p class="text-gray-700 leading-relaxed">
        Your new answer text goes here.
    </p>
</div>
```

### Making Answers Multi-Paragraph

If your answer needs multiple paragraphs:

```html
<div class="faq-answer hidden px-6 pb-4 border-t border-gray-200">
    <p class="text-gray-700 leading-relaxed mb-3">
        First paragraph of your answer.
    </p>
    <p class="text-gray-700 leading-relaxed">
        Second paragraph of your answer.
    </p>
</div>
```

**Note:** Add `mb-3` to all paragraphs except the last one to add spacing between them.

### Removing an FAQ Item

To delete a question:

1. **Find the entire FAQ item block** (from `<div class="faq-item">` to the closing `</div>`)
2. **Delete the entire block**
3. **Save your file**

### Styling FAQ Items

#### Changing Question Background Color on Hover

**Find:**
```html
<button class="faq-question w-full px-6 py-4 flex items-center justify-between hover:bg-gray-50 transition-colors duration-300 cursor-pointer">
```

**Change `hover:bg-gray-50` to another color:**
- `hover:bg-purple-50` = light purple
- `hover:bg-blue-50` = light blue
- `hover:bg-gray-100` = slightly darker gray

#### Changing Icon Color

**Find:**
```html
<i class="faq-icon fas fa-chevron-down text-purple-600 transition-transform duration-300"></i>
```

**Change `text-purple-600` to another color:**
- `text-blue-600` = blue
- `text-gray-600` = gray
- `text-green-600` = green

#### Changing Card Border Color

**Find:**
```html
<div class="faq-item bg-white rounded-lg border border-gray-200 overflow-hidden">
```

**Change `border-gray-200` to another color:**
- `border-purple-200` = light purple
- `border-gray-300` = darker gray

### How FAQ JavaScript Works

The FAQ uses this JavaScript to toggle answers:

```javascript
// For each FAQ item
faqItems.forEach(item => {
    const question = item.querySelector('.faq-question');
    if (question) {
        question.addEventListener('click', () => {
            const answer = item.querySelector('.faq-answer');
            
            // Close all other FAQ items
            faqItems.forEach(otherItem => {
                if (otherItem !== item) {
                    otherItem.querySelector('.faq-answer')?.classList.add('hidden');
                    otherItem.querySelector('.faq-icon')?.classList.remove('rotate-180');
                }
            });
            
            // Toggle current item
            answer?.classList.toggle('hidden');        // Shows/hides answer
            item.querySelector('.faq-icon')?.classList.toggle('rotate-180');  // Rotates icon
        });
    }
});
```

**Important:** Don't modify the `hidden` class or the JavaScript. The system relies on these to work properly.

---

## Troubleshooting Guide

### Common Issues and Solutions

#### Issue 1: Links Don't Work

**Problem:** Clicking a link doesn't go anywhere or shows an error.

**Solutions:**

1. **Check the URL spelling:**
   ```html
   <!-- Wrong -->
   <a href="https://upflex.digital.com">
   
   <!-- Correct -->
   <a href="https://upflexdigital.com">
   ```

2. **Make sure external URLs include `https://`:**
   ```html
   <!-- Wrong -->
   <a href="upflexdigital.com">
   
   <!-- Correct -->
   <a href="https://upflexdigital.com">
   ```

3. **Make sure internal links start with `#`:**
   ```html
   <!-- Wrong -->
   <a href="features">
   
   <!-- Correct -->
   <a href="#features">
   ```

4. **Check that files exist:**
   If linking to `privacy.html`, make sure the file exists in the same folder.

#### Issue 2: Styling Looks Broken

**Problem:** Colors, sizes, or spacing look wrong.

**Solutions:**

1. **Check that class names are spelled correctly:**
   ```html
   <!-- Wrong -->
   <div class="text-4xl fond-bold">
   
   <!-- Correct -->
   <div class="text-4xl font-bold">
   ```

2. **Make sure you didn't accidentally delete class attributes:**
   ```html
   <!-- Wrong -->
   <h1>My Heading</h1>
   
   <!-- Correct -->
   <h1 class="text-4xl font-bold">My Heading</h1>
   ```

3. **Check that Tailwind CSS is still loaded:**
   ```html
   <!-- Make sure this line is still in <head> -->
   <script src="https://cdn.tailwindcss.com"></script>
   ```

#### Issue 3: Mobile Menu Doesn't Work

**Problem:** Hamburger menu button doesn't open the menu on mobile.

**Solutions:**

1. **Check that you didn't modify the class names:**
   - Button must have class: `mobile-menu-button`
   - Menu must have class: `mobile-menu`
   - These names are referenced in the JavaScript

2. **Make sure JavaScript section is intact:**
   ```html
   <!-- At the bottom of your file, before </body> -->
   <script>
       document.addEventListener('DOMContentLoaded', function() {
           // Mobile Menu Toggle code...
       });
   </script>
   ```

3. **Check browser console for errors:**
   - Press `F12` to open developer tools
   - Click "Console" tab
   - Look for red error messages

#### Issue 4: FAQ Accordion Doesn't Work

**Problem:** Clicking FAQ questions doesn't show/hide answers.

**Solutions:**

1. **Check that you didn't modify class names:**
   - Items must have class: `faq-item`
   - Questions must have class: `faq-question`
   - Answers must have class: `faq-answer`
   - Icons must have class: `faq-icon`

2. **Make sure the `hidden` class is present on answers:**
   ```html
   <!-- Correct - answer is hidden by default -->
   <div class="faq-answer hidden px-6 pb-4 border-t border-gray-200">
   ```

3. **Check JavaScript is intact:**
   The FAQ code must be in the `<script>` section at the bottom.

#### Issue 5: Page Looks Weird on Mobile

**Problem:** Layout breaks or looks strange on phones.

**Solutions:**

1. **Check responsive classes are present:**
   ```html
   <!-- Should have mobile and larger screen sizes -->
   <h1 class="text-4xl md:text-5xl lg:text-6xl">
   ```

2. **Check viewport meta tag is present:**
   ```html
   <!-- In <head> section -->
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   ```

3. **Test with browser dev tools:**
   - Press `F12`
   - Click the mobile icon (top left)
   - Select different device sizes

#### Issue 6: Images Not Showing

**Problem:** Images appear as broken image icons.

**Solutions:**

1. **Check image URLs are correct:**
   ```html
   <!-- Background image example -->
   <div style="background-image: url('https://images.unsplash.com/photo-...?w=1200')">
   ```

2. **Make sure external image URLs are complete:**
   ```html
   <!-- Wrong -->
   <div style="background-image: url('images/photo.jpg')">
   
   <!-- Correct for external URLs -->
   <div style="background-image: url('https://images.unsplash.com/...')">
   ```

#### Issue 7: Colors Look Different Than Expected

**Problem:** Colors don't match what you specified.

**Solutions:**

1. **Check you're using valid color class names:**
   ```html
   <!-- Valid Tailwind colors -->
   text-purple-600
   bg-gray-50
   text-blue-400
   
   <!-- Not valid -->
   text-purple
   bg-gray
   ```

2. **Remember color numbers (50-900):**
   - `50` = very light
   - `100-400` = light shades
   - `500` = medium
   - `600-700` = darker shades
   - `800-900` = very dark

3. **If using custom gradient:**
   ```html
   <!-- Check this is in <style> section -->
   <style>
       .gradient-accent {
           background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
       }
   </style>
   ```

#### Issue 8: Text Content Changes Don't Show

**Problem:** You edited text but it still shows the old content.

**Solutions:**

1. **Save your file:**
   - Press `Ctrl+S` (Windows) or `Cmd+S` (Mac)

2. **Hard refresh your browser:**
   - Press `Ctrl+Shift+R` (Windows) or `Cmd+Shift+R` (Mac)
   - This clears the cache and reloads the page

3. **Check you edited the correct file:**
   - Make sure you're editing `index.html` (not a copy)
   - Check the file path in your editor

#### Issue 9: Buttons Don't Look Right

**Problem:** Buttons look broken or have wrong colors.

**Solutions:**

1. **Check button classes are present:**
   ```html
   <!-- Should have gradient and styling -->
   <a href="..." class="gradient-accent text-white px-6 py-2 rounded-lg font-semibold">
   ```

2. **Make sure you didn't remove the gradient class:**
   ```html
   <!-- Wrong -->
   <a href="..." class="text-white px-6 py-2">
   
   <!-- Correct -->
   <a href="..." class="gradient-accent text-white px-6 py-2 rounded-lg">
   ```

#### Issue 10: Navigation Links Don't Jump to Sections

**Problem:** Clicking navigation items doesn't scroll to sections.

**Solutions:**

1. **Check section IDs match link references:**
   ```html
   <!-- Link -->
   <a href="#features">Features</a>
   
   <!-- Section must have matching ID -->
   <section id="features">
   ```

2. **Make sure IDs are spelled correctly:**
   ```html
   <!-- Wrong - ID is "feature" but link is "features" -->
   <section id="feature">
   <a href="#features">
   
   <!-- Correct -->
   <section id="features">
   <a href="#features">
   ```

3. **Check smooth scroll CSS is present:**
   ```html
   <!-- In <style> section -->
   <style>
       html {
           scroll-behavior: smooth;
       }
   </style>
   ```

### Getting More Help

If you're still stuck:

1. **Check the browser console for errors:**
   - Press `F12`
   - Click "Console"
   - Look for red error messages

2. **Compare your code to the original:**
   - Check if you accidentally deleted something
   - Make sure all tags are properly closed

3. **Test in a different browser:**
   - Try Chrome, Firefox, or Safari
   - This helps identify browser-specific issues

4. **Clear browser cache:**
   - Press `Ctrl+Shift+Delete` (Windows) or `Cmd+Shift+Delete` (Mac)
   - Select "All time"
   - Click "Clear data"

---

## Best Practices for Maintenance

### Regular Updates

**Update these items regularly:**

1. **Testimonials** - Add new customer feedback quarterly
2. **Statistics** - Update numbers (projects, satisfaction rate, years)
3. **Contact information** - If your details change
4. **Links** - Check quarterly to ensure they still work

### Backup Your Files

**Always keep backups:**

1. Save a copy of your files to a cloud service (Google Drive, Dropbox, OneDrive)
2. Keep a copy on an external hard drive
3. Consider using version control (GitHub) for advanced tracking

### Testing

**Test your page regularly:**

1. Test on different devices (phone, tablet, desktop)
2. Test all links work correctly
3. Test contact forms (if added)
4. Check page loads quickly
5. Test on different browsers

### Security

**Keep your site secure:**

1. Keep file permissions appropriate (not world-readable for sensitive files)
2. Use HTTPS when deploying to a server
3. Keep any backend code updated
4. Don't include sensitive information in HTML

### Performance

**Keep your page fast:**

1. Optimize images (use tools like [TinyPNG](https://tinypng.com/))
2. Minimize CSS and JavaScript
3. Use a Content Delivery Network (CDN) for faster loading
4. Monitor page load speed with [Google PageSpeed Insights](https://pagespeed.web.dev/)

---

## Quick Reference Cheat Sheet

### Common Tailwind Classes

| Purpose | Class Examples |
|---------|---|
| **Text Size** | `text-sm`, `text-base`, `text-lg`, `text-xl`, `text-2xl`, `text-3xl`, `text-4xl`, `text-5xl`, `text-6xl` |
| **Text Weight** | `font-normal`, `font-semibold`, `font-bold` |
| **Text Color** | `text-gray-900`, `text-gray-600`, `text-white`, `text-purple-600`, `text-blue-600` |
| **Background** | `bg-white`, `bg-gray-50`, `bg-purple-600`, `bg-gradient-to-r` |
| **Padding** | `p-4`, `px-6`, `py-8`, `pt-4`, `pb-4` |
| **Margin** | `m-4`, `mx-auto`, `my-8`, `mt-4`, `mb-6` |
| **Rounded Corners** | `rounded`, `rounded-lg`, `rounded-xl`, `rounded-full` |
| **Shadows** | `shadow-sm`, `shadow-md`, `shadow-lg`, `shadow-xl` |
| **Display** | `flex`, `grid`, `hidden`, `block`, `inline-block` |
| **Responsive** | `md:text-5xl`, `lg:text-6xl`, `sm:px-6` |
| **Hover Effects** | `hover:text-purple-600`, `hover:bg-gray-50`, `hover:shadow-lg` |

### Common HTML Tags

| Tag | Purpose | Example |
|-----|---------|---------|
| `<h1>` - `<h6>` | Headings | `<h1>Main Title</h1>` |
| `<p>` | Paragraph | `<p>Text content</p>` |
| `<a>` | Link | `<a href="url">Link text</a>` |
| `<div>` | Container | `<div class="...">Content</div>` |
| `<section>` | Section | `<section id="features">...</section>` |
| `<button>` | Button | `<button>Click me</button>` |
| `<ul>` / `<li>` | Lists | `<ul><li>Item</li></ul>` |
| `<span>` | Inline text | `<span>Highlighted text</span>` |
| `<i>` | Icon | `<i class="fas fa-check"></i>` |

### File Organization

```
your-project-folder/
├── index.html          (Main landing page)
├── privacy.html        (Privacy policy)
├── terms.html          (Terms of service)
├── blog.html           (Blog page - if you have one)
└── assets/             (Folder for images, etc.)
    ├── logo.png
    ├── hero-image.jpg
    └── ...
```

---

## Conclusion

You now have a comprehensive guide to maintaining and customizing your Upflex Digital landing page. Remember:

- **Start small** - Make one change at a time
- **Save frequently** - Use Ctrl+S or Cmd+S
- **Test thoroughly** - Check your changes in a browser
- **Keep backups** - Always have copies of your files
- **Don't be afraid** - HTML and CSS are forgiving; you can't break anything permanently

For questions or issues, refer back to the relevant section of this guide or contact your web developer.

Happy maintaining! 🚀