# 101Headshots Landing Page Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the 101Headshots landing page. Follow these steps carefully to make updates while preserving the page's functionality and design.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your brand name and navigation menu. To update:

1. **Brand Name:**
```html
<a href="/" class="text-2xl font-bold text-gray-800 hover:text-gray-700 transition-colors duration-300">
    101Headshots <!-- Change this text to update brand name -->
</a>
```

2. **Navigation Menu Items:**
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Features</a>
    <!-- Repeat for each menu item -->
</div>
```

### Hero Section
Update the main headline and subheading:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight mb-6">
    Peculiar, Missouri Corporate Headshot Photography Services <!-- Main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    Headshots helping Peculiar professionals build recognition. <!-- Subheading -->
</p>
```

### Tailwind CSS Class Guide
Common classes used throughout:
- Text sizes: `text-xl`, `text-2xl`, `text-3xl`, etc.
- Colors: `text-gray-600`, `bg-blue-600`, etc.
- Spacing: `px-6`, `py-4`, `mb-12`, etc.
- Responsive design: `md:text-5xl`, `lg:text-6xl`

To modify styles:
1. Find the element you want to change
2. Locate its class attribute
3. Reference Tailwind's documentation for available classes
4. Replace or add classes as needed

Example:
```html
<!-- Original -->
<h3 class="text-xl font-bold mb-4">Style Focus</h3>

<!-- Modified with larger text and different spacing -->
<h3 class="text-2xl font-bold mb-6">Style Focus</h3>
```

## Managing Links

### Navigation Links
Current internal links:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact</a>
```

To update:
1. Locate the link in the navigation section
2. Change the `href` attribute to your desired destination
3. Update the link text between the `<a>` tags

Example:
```html
<!-- Original -->
<a href="#features" class="text-gray-600 hover:text-gray-900">Features</a>

<!-- Modified -->
<a href="#services" class="text-gray-600 hover:text-gray-900">Services</a>
```

### Call-to-Action Links
Current CTA links:
```html
<a href="https://www.101headshots.com" class="inline-block bg-blue-600 text-white px-8 py-4 rounded-lg">
    Book Your Session
</a>
```

To update:
1. Locate the CTA button in the hero or CTA section
2. Change the `href` attribute to your booking URL
3. Update the button text as needed

## Adding Privacy and Terms Pages

### Footer Links Setup
Current placeholder links:
```html
<div>
    <h3 class="text-xl font-bold mb-4">Legal</h3>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white">Terms of Service</a></li>
    </ul>
</div>
```

To add proper links:
1. Create `privacy.html` and `terms.html` in your root directory
2. Update the footer links:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white">Terms of Service</a></li>
```

## Troubleshooting

Common issues and solutions:

1. **Broken Internal Links:**
   - Ensure section IDs match href attributes
   - Check for typos in IDs and hrefs
   - Verify file paths are correct

2. **Responsive Design Issues:**
   - Check mobile view using browser dev tools
   - Verify media query classes (md:, lg:) are correct
   - Test different screen sizes

3. **Style Conflicts:**
   - Review Tailwind class order
   - Check for duplicate classes
   - Verify custom styles aren't overriding Tailwind

Remember to:
- Test all changes in multiple browsers
- Validate HTML using W3C validator
- Check mobile responsiveness
- Back up files before making changes

Need help? Contact technical support or consult the Tailwind CSS documentation for detailed class references.