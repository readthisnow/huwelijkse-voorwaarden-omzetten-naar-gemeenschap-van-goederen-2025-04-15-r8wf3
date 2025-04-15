# Landing Page Maintenance Guide

This guide will help you maintain and customize the Notarissen Online landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common updates.

## 1. Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Hero Section
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-extrabold text-gray-900 mb-8 leading-tight">
    Huwelijkse Voorwaarden Omzetten Naar Gemeenschap van Goederen
</h1>
```
To update the main headline:
1. Locate the `<h1>` tag in the hero section (around line 45)
2. Replace the text between the opening and closing tags
3. Maintain the existing classes to preserve styling

#### Feature Cards
```html
<div class="bg-white rounded-xl shadow-lg p-8 hover:shadow-xl transition-shadow duration-300">
    <h3 class="text-xl font-bold mb-4">⚡ Tijdelijk Extra Voordelig</h3>
    <p class="text-gray-600">Mis deze unieke kans niet!</p>
</div>
```
To add or modify feature cards:
1. Find the features section (id="features")
2. Copy an existing card div
3. Update the heading (`<h3>`) and paragraph (`<p>`) text
4. Paste within the grid container

### Tailwind CSS Classes Explained

#### Responsive Design Classes
- `md:text-5xl`: Applies at medium screens (768px+)
- `lg:text-6xl`: Applies at large screens (1024px+)
- `grid-cols-1 md:grid-cols-2 lg:grid-cols-3`: Responsive grid layout

#### Common Style Classes
- `container mx-auto`: Centers content with auto margins
- `px-4 sm:px-6 lg:px-8`: Responsive padding
- `rounded-lg`: Rounded corners
- `shadow-lg`: Box shadow effect

## 2. Fixing Broken Links

### Navigation Menu Links
Current navigation structure:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-600 hover:text-blue-600 transition-colors">Voordelen</a>
    <a href="#benefits" class="text-gray-600 hover:text-blue-600 transition-colors">Waarom Kiezen</a>
    <a href="#faq" class="text-gray-600 hover:text-blue-600 transition-colors">FAQ</a>
    <a href="#contact" class="text-gray-600 hover:text-blue-600 transition-colors">Contact</a>
</div>
```

To update navigation links:
1. Locate the navigation div in the header
2. For internal page sections, use `#section-id`
3. For external pages, use the full URL
4. Example: `<a href="https://example.com/about">About</a>`

### Call-to-Action Links
```html
<a href="https://notarissen-online.nl" class="inline-block bg-blue-600 text-white...">
    Direct Regelen
</a>
```
To update CTA buttons:
1. Find the CTA buttons (in hero and CTA sections)
2. Replace `https://notarissen-online.nl` with your desired URL
3. Update button text between the tags

## 3. Adding Privacy and Terms Pages

### Footer Modification
Add these links to the footer section:
```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
    <!-- Existing footer content -->
    <div>
        <h3 class="text-xl font-bold mb-4">Legal</h3>
        <ul class="space-y-2">
            <li><a href="/privacy.html" class="text-gray-400 hover:text-white transition-colors">Privacy Policy</a></li>
            <li><a href="/terms.html" class="text-gray-400 hover:text-white transition-colors">Terms of Service</a></li>
        </ul>
    </div>
</div>
```

### Style Consistency
- Use `text-gray-400` for footer links
- Add `hover:text-white` for hover effects
- Maintain the `transition-colors` class for smooth transitions

## Troubleshooting Tips

1. **Broken Internal Links**
   - Ensure section IDs match href attributes
   - Check for typos in ID names
   - IDs are case-sensitive

2. **Responsive Design Issues**
   - Test at different screen sizes
   - Use browser developer tools (F12)
   - Verify breakpoint classes (sm:, md:, lg:)

3. **Style Inconsistencies**
   - Copy existing classes for new elements
   - Maintain spacing patterns
   - Check parent container classes

## Additional Notes

- Always backup before making changes
- Test all links after updates
- Maintain consistent indentation
- Preview changes in multiple browsers
- Keep the responsive design intact by preserving breakpoint classes

Need help? Contact your web development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).