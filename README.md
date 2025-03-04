# Elite Diet 974 Landing Page - Maintenance Guide

This guide will help you maintain and customize the Elite Diet 974 landing page. It's written for beginners with no prior coding experience.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu. To update:

1. **Company Name:**
```html
<div class="text-2xl font-bold bg-gradient-to-r from-purple-500 to-pink-500 bg-clip-text text-transparent">
    Elite Diet 974  <!-- Change this text -->
</div>
```

2. **Navigation Menu Items:**
```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="hover:text-purple-400 transition-colors duration-300">Accueil</a>
    <a href="#" class="hover:text-purple-400 transition-colors duration-300">Produits</a>
    <a href="#" class="hover:text-purple-400 transition-colors duration-300">Contact</a>
</div>
```

### Hero Section
Located at the top of the page with the main headline:

```html
<h1 class="text-4xl md:text-6xl lg:text-7xl font-extrabold mb-8 bg-gradient-to-r from-purple-400 to-pink-500 bg-clip-text text-transparent">
    Elite Diet 974  <!-- Main headline -->
</h1>
<p class="text-xl md:text-2xl lg:text-3xl text-gray-300 mb-12">
    Le plus grand choix de protéines à la Réunion  <!-- Subheadline -->
</p>
```

### Features Section
To modify the product cards:

```html
<div class="bg-gray-900 rounded-2xl p-8 hover:shadow-xl hover:shadow-purple-500/10 transform hover:scale-105 transition-all duration-300">
    <div class="w-16 h-16 bg-gradient-to-br from-purple-500 to-pink-500 rounded-lg mb-6"></div>
    <h3 class="text-xl font-bold mb-4">Whey</h3>  <!-- Product title -->
    <p class="text-gray-400">Protéines premium pour vos objectifs</p>  <!-- Product description -->
</div>
```

### Understanding Tailwind Classes
- `text-4xl`: Text size (increases with number)
- `md:text-6xl`: Applies at medium screens and up
- `font-bold`: Text weight
- `mb-8`: Margin bottom (spacing)
- `bg-gray-900`: Background color
- `rounded-2xl`: Border radius
- `hover:scale-105`: Grows element on hover

## Managing Links

### Current Link Locations

1. **Navigation Menu Links:**
```html
<div class="hidden md:flex space-x-8">
    <a href="#">Accueil</a>  <!-- Replace # with actual URL -->
    <a href="#">Produits</a>
    <a href="#">Contact</a>
</div>
```

2. **Call-to-Action Button:**
```html
<a href="#contact" class="inline-block bg-gradient-to-r from-purple-500 to-pink-500 px-8 py-4 rounded-full">
    Découvrir nos produits
</a>
```

3. **Email Link:**
```html
<a href="mailto:contact@valdeno.re">contact@valdeno.re</a>
```

To update links:
1. Replace `#` with your page URL
2. For internal pages, use relative paths (e.g., `/products.html`)
3. For external links, use full URLs (e.g., `https://example.com`)

## Adding Privacy and Terms Pages

### Step 1: Update Footer Links
Locate this section in the footer:

```html
<ul class="space-y-2">
    <li><a href="privacy.html" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Mentions légales</a></li>
    <li><a href="terms.html" class="text-gray-400 hover:text-purple-400 transition-colors duration-300">Politique de confidentialité</a></li>
</ul>
```

### Step 2: Create New Pages
1. Create `privacy.html` and `terms.html` in your root directory
2. Copy the header and footer from `index.html`
3. Add your privacy policy and terms content

## Troubleshooting

### Common Issues:

1. **Broken Links**
- Check for typos in URLs
- Ensure files exist in the correct directory
- Verify file extensions (.html, .php, etc.)

2. **Styling Problems**
- Check class names for typos
- Maintain the same class structure when copying elements
- Keep responsive classes (`md:`, `lg:`) in order

3. **Layout Issues**
- Preserve container structure:
```html
<div class="container mx-auto px-6">
    <!-- Content must stay inside container -->
</div>
```

### Need Help?
- Validate HTML at [W3C Validator](https://validator.w3.org/)
- Check Tailwind documentation for class references
- Keep backup copies before making changes

Remember to test all changes across different screen sizes using your browser's developer tools (F12).