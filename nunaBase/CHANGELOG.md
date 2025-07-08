# Changelog

All notable changes to this theme will be documented here.

## [0.1.5] – 2025-07-08

### ✨ New Features

-   **SEO & Sitemap Integration:**
    Implemented SEO settings panel, JSON-LD structured data rendering, and a custom XML sitemap with multi-language support.
-   **Flexible Hero Section:**
    Refactored Hero section with improved structure, new flexible content fields, and enhanced component management.
-   **Header Scroll Effect:**
    Added new smooth scroll activation logic to header using `requestAnimationFrame`.
-   **Shortcodes for Editors:**
    Registered new shortcodes (e.g., site name) for use inside WYSIWYG content.
-   **Hotel Advantages Options Page:**
    Created new ACF field group and options page for hotel advantages using flexible content layout.

### 🖼️ Image & Icon Enhancements

-   **WebP Optimization:**
    Enhanced image handling with automatic conversion to WebP format and updated image size settings.
-   **Picture Element Support:**
    Added `<picture>` selectors for cards and rooms to improve responsive image loading.
-   **SVG Icons Update:**
    Added multiple new outline and solid icons for features (e.g., TV, WiFi, Room Size, Pets Allowed).
-   **Accessibility Improvements:**
    Updated icons for better screen reader support and visual consistency.

### 🎨 Style & SCSS Refactors

-   **Spacing Consistency:**
    Replaced all uses of `--baseline` with `--space` across SCSS for consistent spacing.
-   **Updated Variables & Colors:**
    Refined SCSS variables for room gaps, color usage, and layout adjustments.
-   **Component Styling:**
    -   Updated button styles (hover, active states)
    -   Enhanced header styling with logo filters and transitions
    -   Adjusted footer grid layout and background opacity
    -   Improved responsiveness across header and footer components

### 🛠 Code Improvements & Refactors

-   **Modular Templates:**
    Refactored multiple section templates to use flexible content components for better maintainability.
-   **Enqueue Logic:**
    Improved Vite manifest handling in `enqueue-assets.php`. Now uses `nuna_hotel_id` instead of `hotel_id`.
-   **Markup Cleanups:**
    -   Consolidated footer address display logic
    -   Removed unused image styles in Hero section
    -   Updated booking engine ID references in header & hero
    -   Renamed "Hotel Info" to "Information" in menu config
    -   Added translations for booking CTA and footer menu items

### 🔗 Dependencies & Assets

-   **Icons:**
    Added outline and solid icon sets for common amenities and contact information.
-   **SVG & Asset Management:**
    Centralized icon imports, optimized asset loading performance.

## [0.1.4] - 2025-06-23

### ✨ New Features

-   **Section Builder:** Introduced the new _Section Builder_ (replacing Section Content List) for flexible content blocks with media support.
-   **Custom Skins & Reset Control:** Added reset functionality in the Customizer. Introduced new skins _Albemarle_ and _Isamar_ with custom SCSS and color variables.
-   **Room Layout Options:** Added layout options and view button visibility control for the Rooms section via ACF fields.
-   **Flexible Content Fields:** Added new flexible content fields in ACF JSON for enhanced content management.
-   **Translation Support:** Enabled translation functionality for dynamic CTA labels like _Book_ and _Menu_. Created a new language strings file.

### 🛠️ Enhancements

#### Cards & Rooms

-   Updated `c_card` component for better media handling with conditional checks.
-   Refactored card structure and implemented `c_cards` function for improved modular rendering.
-   Enhanced SCSS for cards and rooms components for layout flexibility and responsiveness.
-   Improved image rendering in `p_image.php` with lazy loading support.
-   Removed deprecated `c_room.php` in favor of the modular `c_rooms.php`.

#### Layout & Styling

-   Expanded baseline variables in `_base.scss` for improved scalability and maintainability.
-   Updated `earth.css` and `jupiter.css` to use new baseline multipliers for padding and gaps.
-   Added layout options for cards and rooms with updated CSS variables for responsive design.
-   Refactored SCSS structure:
    -   Removed unused index files.
    -   Updated mixins with responsive breakpoints.
    -   Streamlined asset enqueueing in `functions.php`.
-   Streamlined background image handling in `s_advantages`, `s_builder`, `s_cards`, and `s_rooms`.
-   Adjusted SCSS files to improve layout consistency and responsiveness across all components.

#### Content & Accessibility

-   Enhanced content structure in `s_builder`, `s_cards`, and `s_rooms` for better readability and maintainability.
-   Updated `s_builder.php` to include early return with media presence checks.
-   Refactored `c_cards.php` to use semantic HTML and improved accessibility.
-   Updated `aria-labels` for navigation and buttons in `header.php` and `c_action_bar.php`.
-   Simplified `p_title.php` by removing unnecessary `role` attributes on heading tags.

### 🔧 Code Cleanup & Refactors

#### Footer

-   Simplified footer layout by removing unnecessary wrapper `<div>` elements.
-   Restructured `footer.php` for better organization of contact information and social media links.

#### Global Structure

-   Removed obsolete `theme-preview.php` as it was no longer needed.
-   Reordered utility function inclusions in `functions.php` for clarity.

## [0.1.3] - 2025-06-02

### ✨ Features

-   Added Header Overlay Panel and Modal component for improved user interaction.
-   Introduced Action Bar for mobile with contact options and booking button.
-   Registered new typography settings (heading and body fonts) in the Customizer.
-   Registered a new navigation menu for policies.
-   Created a custom menu walker to support menu descriptions in header navigation.

### 🎨 Enhancements

-   Enhanced theme Customizer and header functionality, including new layout options and CTA button support.
-   Updated footer layout and responsiveness, including a new hotel chain section.
-   Enhanced content list section with dynamic background image support.
-   Added eyebrow styling to content components for better visual hierarchy.

### 🛠 Refactoring

-   Refactored header template and modal styles for improved accessibility and consistency.
-   Updated CSS variables for better maintainability across components.

### ♿ Accessibility

-   Improved semantic structure and accessibility in header, footer, and action bar templates.

## [0.1.2] - 2025-05-21

-   Release version test

## [0.1.1] - 2025-05-15

-   Release version test

## [0.1.0] - 2025-05-14

### 🔧 Initial Beta Release

-   🎨 Implemented basic layout structure and core styles.
-   ⚙️ Scaffolded the theme options panel (initial draft).
