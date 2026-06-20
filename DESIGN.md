# Design System (@DESIGN.md)

This document establishes the Vercel-like design system for the Name Numerology Hub.

## 1. Philosophy
- **Vercel Aesthetic**: Minimalist, clean, high-contrast, fast.
- **Glassmorphism**: Subtle translucent backgrounds with borders.
- **Responsiveness**: Fluidly adapts to mobile, tablet, and desktop screens.

## 2. Typography
- **Primary Font**: `Inter`, sans-serif.
- **Scale**:
  - `h1`: `text-4xl md:text-5xl font-extrabold tracking-tight`
  - `h2`: `text-3xl md:text-4xl font-bold tracking-tight`
  - `h3`: `text-2xl font-semibold tracking-tight`
  - `body`: `text-base md:text-lg text-gray-400`
  - `small`: `text-sm text-gray-500`

## 3. Colors (Dark Mode Default)
- **Background**: `#000000` (Pure Black)
- **Surface / Cards**: `#0A0A0A` (Near Black) with a `border-zinc-800` outline.
- **Text Primary**: `#FFFFFF` (White)
- **Text Secondary**: `#A1A1AA` (Zinc 400)
- **Accents**: 
  - Subtle glowing gradients: `bg-gradient-to-r from-purple-500 to-cyan-500`
  - Action buttons: White background with black text (`bg-white text-black hover:bg-gray-200`)

## 4. UI Components

### Cards (Glassmorphism)
```html
<div class="bg-zinc-900/50 border border-zinc-800 backdrop-blur-md rounded-xl p-6 hover:border-zinc-700 transition-all duration-300">
  <!-- Content -->
</div>
```

### Buttons
```html
<!-- Primary -->
<button class="bg-white text-black px-6 py-2 rounded-md font-medium hover:bg-zinc-200 transition-colors">
  Calculate
</button>

<!-- Secondary -->
<button class="bg-zinc-900 text-white border border-zinc-800 px-6 py-2 rounded-md font-medium hover:bg-zinc-800 transition-colors">
  Learn More
</button>
```

### Inputs
```html
<input type="text" class="w-full bg-zinc-900 border border-zinc-800 text-white rounded-md px-4 py-2 focus:outline-none focus:ring-2 focus:ring-zinc-600 focus:border-transparent transition-all" />
```

## 5. Layout & Spacing
- **Container**: `max-w-5xl mx-auto px-4 sm:px-6 lg:px-8`
- **Section Spacing**: `py-16 md:py-24`
- **Flex/Grid Gaps**: `gap-6 md:gap-8`

## 6. Responsiveness
- All pages will use Tailwind's `md:` and `lg:` prefixes to ensure fluid layouts across mobile, tablet, and desktop viewports.
