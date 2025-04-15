# Landing Page Maintenance Guide
## Best Websites TX Landing Page

This guide provides detailed instructions for maintaining and customizing the Best Websites TX landing page. It's written for beginners with no prior coding experience.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<div class="text-2xl font-bold text-blue-600">
    Best Websites TX  <!-- Update company name here -->
</div>
```
To modify the company name, simply replace "Best Websites TX" with your desired text.

#### Hero Section
The main headline and subtext can be found here:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight mb-8">
    Custom Websites For Your Business  <!-- Main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12 leading-relaxed">
    Transform your online presence...  <!-- Subheading text -->
</p>
```

#### Features Section
Each feature card follows this structure:
```html
<div class="bg-white rounded-xl p-8 shadow-lg hover:shadow-xl transition-shadow duration-300">
    <h3 class="text-xl font-bold mb-4">Easy to Use</h3>  <!-- Feature title -->
    <p class="text-gray-600 leading-relaxed">
        Intuitive interface...  <!-- Feature description -->
    </p>
</div>
```

### Tailwind CSS Classes Explained

#### Common Class Patterns
- Text sizes: `text-xl`, `text-2xl`, etc. (larger number = bigger text)
- Colors: `text-blue-600`, `bg-white`, etc.
- Spacing: `p-8` (padding), `mb-4` (margin-bottom)
- Responsive design: `md:text-5xl` (applies at medium screens and up)

#### Modifying Colors
To change colors, locate classes starting with:
- `text-`: Text color
- `bg-`: Background color
- `border-`: Border color

Example:
```html
<!-- Original -->
<div class="text-blue-600">

<!-- Change to red -->
<div class="text-red-600">
```

## Fixing Broken Links

### Navigation Menu Links
Current navigation links are:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

To update:
1. Locate the `href` attribute
2. Replace the value with your new link:
   - Internal sections: Use `#section-name`
   - External pages: Use full URL `https://example.com`

### Call-to-Action Links
Currently pointing to:
```html
<a href="https://sigmaseo.io" class="inline-block bg-blue-600...">
```

To update:
1. Replace `https://sigmaseo.io` with your desired URL
2. Ensure the URL includes `https://` for external links

## Linking Privacy and Terms Pages

### Current Footer Links Structure
```html
<div>
    <h4 class="text-lg font-semibold text-white mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

### Adding Privacy and Terms Links
1. Create your privacy.html and terms.html files
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues

1. **Broken Internal Links**
   - Ensure section IDs match href values
   - Example: `href="#features"` needs matching `id="features"` in section

2. **Responsive Design Issues**
   - Check for `md:` and `lg:` prefixes
   - Don't remove these classes as they control mobile responsiveness

3. **Icon Problems**
   - If icons don't appear, verify Font Awesome inclusion:
   ```html
   <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
   ```

### Best Practices
- Always test changes in multiple browsers
- Check mobile responsiveness using browser dev tools
- Keep backup copies of working code before making changes
- Maintain consistent spacing and indentation
- Test all links after updating

Need additional help? Contact your web development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).