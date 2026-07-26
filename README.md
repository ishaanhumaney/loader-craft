# Loader Craft

A drop-in showcase and code reference for pure CSS loading indicators and skeleton components. No heavy JavaScript frameworks, no external runtime dependencies—just clean keyframes and modern layout techniques.

## Overview

Waiting on API calls or async state updates shouldn't mean adding bloated UI libraries to your build. `css-loader-craft` provides modular, CSS-only loading indicators that rely on browser-native animation threads (`transform`, `opacity`, and custom CSS keyframes). 

Drop the raw CSS styles into your stylesheet, copy the structural HTML tags, and you're good to go.

## How it Works

The project renders loading patterns inside self-contained CSS layout cards. Each pattern uses targeted keyframe schedules to drive movement, scaling, and shimmer effects:

* **Hardware-Accelerated Motion:** Animations focus on CSS properties handled directly by the GPU (`transform: rotate()`, `scale()`, `opacity`) to reduce main-thread rendering lag.
* **Pure HTML/CSS Coupling:** States are entirely controlled by static structural elements and recurring `@keyframes` rules.

## Key Features

* **Classic Ring:** Simple 360-degree continuous rotation built on subtle border contrast.
* **Pulsing Dots:** Staggered sequence using `animation-delay` across sequential child nodes.
* **Double Ring:** Counter-rotating nested borders that give a dual-gear mechanical feel.
* **Fading Bar:** Horizontally scaling progress indicator driven by `scaleX` keyframe alterations.
* **Skeleton Loader:** Content-placeholder shimmer state leveraging moving CSS linear gradients.

## Tech Stack Breakdown

* **HTML5:** Semantic element containers layout structure.
* **CSS3:** Custom keyframe animations, Flexbox layout, CSS gradients, relative positioning.

## Prerequisites & Web-Based Quick Start

You don't need to clone this locally or set up Node.js tools. You can run and inspect everything straight through GitHub in your web browser.

### Option A: Edit & Preview in Browser (GitHub.dev)
1. Press `.` (period) on your keyboard while viewing this repository, or swap `.com` to `.dev` in the URL.
2. The browser-based VS Code environment will load automatically.
3. Edit `index.html` or `style.css` directly.

### Option B: Run in GitHub Codespaces
1. Click the **Code** button on the top right of the repository page.
2. Select the **Codespaces** tab and click **Create codespace on main**.
3. Use an extension like *Live Server* inside the web editor to preview `index.html`.

### Option C: Local Run
If you prefer running it locally, just download the zip or clone the code, then double-click `index.html` to open it in any browser.

## Project Structure

```text
loader-craft/
├── .github/
│   └── workflows/
│       └── validation.yml    # Validates HTML/CSS formatting on pull requests
├── .gitignore                # Filters out browser runtime logs and OS junk
├── index.html                # Markup displaying the five loader variants
├── style.css                 # Keyframe logic, structural styling, and layout grids
└── README.md                 # Documentation
```

## Roadmap

[ ] Add dark mode CSS variables to simplify theme swapping.

[ ] Add SCSS mixins for custom color parameterization.

[ ] Add accessibility ARIA standards guidelines for screen readers.
