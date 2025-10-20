# Design Guidelines for Shikha Shukla's Portfolio Website

## Design Approach
**Reference-Based Approach** drawing inspiration from modern developer portfolios (Linear, Notion, GitHub profiles) combined with the structural flow of the provided example site, but with a fresh, contemporary purple-blue gradient aesthetic that appeals to tech/AI/ML space.

## Core Design Elements

### A. Color Palette

**Primary Colors (Dark Mode Focus):**
- Background Base: `250 10% 10%` (Deep charcoal)
- Surface: `250 10% 15%` (Elevated surface)
- Primary Purple: `270 70% 60%` (Vibrant purple for CTAs and accents)
- Primary Blue: `220 80% 55%` (Bright blue for links and highlights)

**Gradient Accents:**
- Hero Gradient: Purple to blue diagonal (`from-purple-600 via-blue-500 to-purple-700`)
- Section Dividers: Subtle purple-blue gradients for visual interest

**Text Colors:**
- Primary Text: `0 0% 95%` (Off-white)
- Secondary Text: `0 0% 70%` (Muted gray)
- Muted Text: `0 0% 50%` (Subtle gray for labels)

### B. Typography

**Font Families:**
- Headings: 'Inter' or 'DM Sans' (Google Fonts) - Modern, clean sans-serif
- Body: 'Inter' - Consistent throughout for cohesion
- Monospace: 'Fira Code' - For code snippets or technical details

**Type Scale:**
- Hero Heading: `text-5xl md:text-6xl lg:text-7xl font-bold`
- Section Headings: `text-3xl md:text-4xl font-bold`
- Subsection Titles: `text-xl md:text-2xl font-semibold`
- Body: `text-base md:text-lg`
- Small Text: `text-sm`

### C. Layout System

**Spacing Primitives:** Use Tailwind units of 4, 6, 8, 12, 16, 20, 24, 32
- Consistent section padding: `py-20 md:py-32`
- Card padding: `p-6 md:p-8`
- Element spacing: `space-y-8 md:space-y-12`

**Container Widths:**
- Max content width: `max-w-7xl mx-auto px-6 md:px-8`
- Narrow content (About): `max-w-4xl mx-auto`
- Full-width sections: Background extends edge-to-edge

## Section-by-Section Layout

### 1. Navigation Bar
**Layout:** Fixed top navigation with blur backdrop
- Logo/Name (left): "Shikha Shukla" in gradient text
- Nav Links (right): About, Experience, Projects, Skills, Certifications, Contact
- Mobile: Hamburger menu with slide-out drawer
- Background: Semi-transparent with backdrop blur (`bg-slate-900/80 backdrop-blur-lg`)

### 2. Hero Section
**Layout:** Full viewport height with split design
- **Left Side (60%):** 
  - Large heading: "Hi, I'm Shikha Shukla" with gradient text effect
  - Subheading: "B.Tech CSE Student | AI & ML Enthusiast | Full Stack Developer"
  - Short intro paragraph (2-3 lines) about passion for AI/ML and web development
  - CTA buttons: "View Projects" (primary gradient), "Download Resume" (outline)
- **Right Side (40%):**
  - Animated gradient orb/blob background effect
  - Professional illustration or abstract geometric pattern (not a photo - modern tech aesthetic)
- **Background:** Dark with subtle animated gradient mesh

### 3. About Me Section
**Layout:** Two-column on desktop, stacked on mobile
- **Left Column:** 
  - Section heading with gradient underline accent
  - Detailed paragraph about education (B.Tech CSE, Galgotias University, CGPA 8.71)
  - Focus on AI/ML specialization, DSA skills, full-stack journey
  - Goals and aspirations
- **Right Column:**
  - Quick stats cards (3x2 grid):
    - "8.71 CGPA" 
    - "2027 Graduate"
    - "7+ Certifications"
    - "5+ Projects"
  - Each card with icon, number, and label

### 4. Experience Section
**Layout:** Timeline-style vertical layout
- Single experience card for Eduskill Python Full Stack Internship
- Card design:
  - Company logo placeholder (left)
  - Role, company, duration (header)
  - Bullet points of responsibilities (body)
  - Gradient border accent on left edge
  - Hover effect: Subtle lift and glow

### 5. Projects Showcase
**Layout:** Masonry grid (2-column on desktop, 1-column on mobile)
**Featured Projects:**
1. **Driver Drowsiness Detection** - Card with icon, Python/OpenCV badges
2. **Spam Email Detection (ML Model)** - New project with ML badges
3. **Google Replica** - New project with HTML/CSS/JS badges
4. **Time Series Analysis** - Data visualization focus
5. **Weather Prediction System** - API integration highlight

**Project Card Structure:**
- Thumbnail placeholder (gradient background with project icon)
- Title and brief description
- Tech stack badges (pill-shaped, colored)
- GitHub link icon button
- Hover: Scale up slightly, show "View Details" overlay

### 6. Skills Section
**Layout:** Multi-column tag cloud with grouped categories
- **Technical Skills:** Python, Java, C, HTML, CSS, SQL, JavaScript, Git, PyTorch, TensorFlow (each as colored pill badge)
- **Soft Skills:** Separate visual treatment (perhaps icon + text cards in a row)
- Use 3-column grid on desktop, responsive to 2 then 1 column

### 7. Certifications Section
**Layout:** Card grid with visual hierarchy
- **Featured Certification (Prominent):**
  - Harvard Python Programming - Larger card, gradient border, centered
- **Other Certifications (3-column grid):**
  - Java Programming (GUVI)
  - Python Programming (GUVI)
  - DBMS (Oracle)
  - Python for Beginners (Udemy)
  - JavaScript Essentials (Udemy)
  - Career Edge (TCS iON)

**Card Design:**
- Institution logo/icon placeholder
- Certification name
- Issuing organization
- Date
- Subtle hover effect

### 8. Contact Section
**Layout:** Centered content with visual elements
- Heading: "Let's Connect"
- Social links as large icon buttons in a row:
  - GitHub (primary link to https://github.com/Shikha18Shukla)
  - LinkedIn
  - Email (shikhashuklaknice@gmail.com)
- Each icon in a card with gradient border on hover
- Background: Subtle gradient effect

### 9. Footer
**Layout:** Simple centered footer
- Copyright text
- "Built with passion" tagline
- Small social icon links
- Gradient top border

## Component Specifications

### Buttons
- **Primary CTA:** Gradient background (`bg-gradient-to-r from-purple-600 to-blue-500`), white text, rounded-lg, px-8 py-3
- **Outline:** Transparent background, gradient border, hover fills with gradient
- **Icon Buttons:** Circular, gradient border, hover scale effect

### Cards
- Background: `bg-slate-800/50` with subtle border
- Rounded corners: `rounded-xl`
- Padding: `p-6 md:p-8`
- Hover: Lift effect with shadow and subtle glow
- Border: 1px solid `slate-700`

### Badges/Tags
- Pill-shaped: `rounded-full px-4 py-1.5`
- Background: Semi-transparent color matching tech (e.g., Python = blue, Java = orange)
- Text: `text-sm font-medium`

### Animations
**Minimal, purposeful animations only:**
- Smooth scroll behavior
- Fade-in on scroll for sections (Intersection Observer)
- Button hover scale (1.05)
- Card hover lift (translateY -4px)
- Hero gradient animation (slow, subtle pulse)

## Images

### Hero Section
**Type:** Abstract geometric illustration or animated gradient orb (NOT a profile photo)
**Style:** Modern, tech-aesthetic with purple-blue color scheme
**Placement:** Right 40% of hero section
**Description:** Floating geometric shapes, gradient mesh, or abstract data visualization that suggests AI/ML theme

### Project Thumbnails
**Type:** Icon-based placeholders with gradient backgrounds
**Style:** Each project gets a unique gradient variant
**Placement:** Top of each project card
**Description:** Simple tech icons (code brackets, database, weather cloud, brain for ML, search for Google) on gradient backgrounds

### Certification Cards
**Type:** Institution logo placeholders
**Style:** Monochrome icons or simple badges
**Placement:** Top-left of certification cards

**No large hero image** - The hero section uses abstract graphics/animations instead of photography for a modern, tech-forward aesthetic.

## Responsive Behavior
- Breakpoints: Mobile (< 768px), Tablet (768-1024px), Desktop (> 1024px)
- Navigation: Hamburger menu below 768px
- Grid layouts collapse: 3-col → 2-col → 1-col
- Hero section: Stacks vertically on mobile (text first, graphic second)
- Font sizes scale down on mobile (responsive type scale)