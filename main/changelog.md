# Changelog

## v2.0.0 - 31-12-2025

**UI-KIT**

* **Improvements**
  * Introduced **CSS Variables** to enhance theming flexibility and maintainability.
  * Removed deprecated **Grid column properties** to align with the latest standards.
  * Resolved **Stack** layout spacing issues, including `gap`, `justifyContent`, and `alignItems`.
  * Corrected **slotProps** usage for improved component consistency.
* **Upgrades**
  * Upgraded project dependencies to the latest stable versions
  * Upgraded framework to **React v19.2.x**.
  * Updated platform to **Next.js v16.1.x**.

#### ADMIN <a href="#admin" id="admin"></a>

* **New Features**
  * Added **Dashboard animations** with interactive component demos.
  * Implemented an enhanced **authentication system** with support for:
    * **Supabase** (Google & Facebook login)
    * **JWT-based authentication**
    * **Firebase authentication**
  * Integrated **Quill Editor** plugin with demo implementation.
  * Introduced **CSS Variables** for improved theming and customization.
  * Added **Yarn** as the package manager.
* **Improvements**
  * Enhanced **Context management** aligned with the Mantis architecture.
  * Updated **menu items** for improved navigation and structure.
  * Implemented **auto system mode** support (design-ready).
  * Removed deprecated **Grid column properties**.
  * Fixed **Stack** layout spacing issues (`gap`, `justifyContent`, `alignItems`).
  * Corrected **slotProps** usage across components.
  * Centralized data fetching using a **single API call** with **Loader** and **Error Boundary** handling.
* **Upgrades**
  * Upgraded project dependencies to the latest stable versions.
  * Updated to **React v19.2**.
  * Updated to **Next.js v16**.

## v1.3.0 - 07-08-2025

**UI-KIT**

* Added Pages In Landings
  * CRM
  * Hosting
  * LMS
* Added New Blocks
  * Metrics – 10th
  * Blog – 8th, 9th, 10th
  * Blog Details – 1st
  * Clientele – 8th
  * Call-to-Action (CTA) – 13th, 14th
  * Features – 26th, 27th
  * Integration – 9th
  * Pricing – 10th
  * Small Hero – 8th
* Added theme switcher
* Added animations
* Fixes
  * MUI slotProps
  * Updated default theme typography from Archivo to Figtree (aligned with Figma)
  * Fixed navbar sticking behavior on scroll
  * Corrected content text casing (uppercase/lowercase)
  * Set real links for footer content on all landing pages
  * Fixed cookie banner positioning
  * Adjusted opacity of TwoTone custom icons
  * Removed unused images
* Package upgrades

#### ADMIN <a href="#admin" id="admin"></a>

* Added VITE package
* Added new modules
  * Billing
  * Avatar upload via Dropzone
  * Country map chart using D3
  * "Items Not Found" and "Permission Denied" blocks
* Table improvements
  * Functional filters
  * Dynamic toolbar based on applied filters
* Form improvements
* Custom Breadcrumb using SWR
* Overridden MUI LoadingButton
* Updated all packages
* Fixes
  * MUI slotProps
  * Tooltip arrow positioning
  * Resolved dark mode inconsistencies

## v1.2.0 - 15-04-2025

* UI-KIT
  * React 19
  * Package Upgrade
* ADMIN
  * React-19
  * Package upgrade
  * Bug fixes
  * Commented **`react-simple-maps`**  due to react-19 incompatibility.

## v1.1.0 - 01-04-2025

* UI-KIT
  * **Newly Added Blocks:**
    * Blog: 7
    * FAQs: 8
    * Features: 24, 25
    * Hero: 18, 19
    * Process: 8
    * Privacy Policy: 2
    * Testimonials: 12, 13
  * New Additions:
    * AI & Crypto section on the SaaS page
    * New LMS Landing
* ADMIN
  * New Modules
    * User
    * Blog
    * Settings: Internationalization
    * Settings: Pricing
  * New UI Elements
    * Snackbar
    * Dialog: Fullscreen&#x20;
    * Plugin: Dropzone
  * Improvements
    * Dynamic messages and buttons for Alert Box (e.g., Delete, Block, Publish)
    * Set real content based on modules/apps
    * Account Module: Add/Edit form fields aligned with the account list
  * Bug Fixes
    * Multi-level menu collapsing issue
    * Mobile media drawer toggler effect
    * Slider: Fixed track color
    * Tooltip: Fix background color
    * Redirect from dashboard to default login page

## v1.0.0 - 30-10-2024

* Initial release
