# Design Guidelines: Yanina Velazquez Wellness & Beauty Spa

## Design Approach
**Reference-Based**: Drawing inspiration from premium wellness platforms (Mindbody, Soothe) and luxury spa experiences, creating a serene yet sophisticated booking experience that builds trust and showcases expertise.

## Core Design Principles
- **Serene Sophistication**: Calming aesthetics that evoke relaxation while maintaining professional credibility
- **Trust-First**: Establish expertise through clean presentation and clear service descriptions
- **Mobile-Optimized**: Primary booking flow designed for on-the-go spa clients

---

## Color Palette

### Light Mode
- **Primary**: 25 85% 95% (Warm Beige/Cream) - Main backgrounds, cards
- **Secondary**: 38 45% 88% (Soft Beige) - Sections, subtle accents
- **Accent Therapeutic**: 239 70% 58% (Indigo) - Therapeutic massage category
- **Accent Maternal**: 330 75% 68% (Rose Pink) - Pregnancy/postpartum services
- **Accent Body**: 45 95% 60% (Warm Amber) - Body contouring treatments
- **Accent Circulatory**: 187 70% 62% (Calming Teal) - Circulatory treatments
- **Text Primary**: 30 20% 25% (Warm Charcoal)
- **Text Secondary**: 30 12% 45% (Muted Brown)

### Dark Mode
- **Primary**: 30 15% 12% (Deep Warm Brown)
- **Secondary**: 30 12% 18% (Muted Brown-Gray)
- **Accents**: Same hues as light mode, adjusted to 60% lightness for visibility
- **Text Primary**: 25 85% 95% (Warm Cream)
- **Text Secondary**: 25 40% 75% (Light Beige)

---

## Typography

### Font Families
- **Primary**: 'Inter' (Google Fonts) - All UI, body text, headings
- **Display**: 'Playfair Display' (Google Fonts) - Hero headline, section titles for elegance

### Scale
- **Hero Headline**: text-5xl md:text-6xl lg:text-7xl, font-bold
- **Section Titles**: text-3xl md:text-4xl, font-semibold
- **Service Names**: text-xl md:text-2xl, font-semibold
- **Body Text**: text-base md:text-lg
- **Small Text**: text-sm
- **CTA Buttons**: text-base md:text-lg, font-medium

---

## Layout System

### Spacing Primitives
Use Tailwind units: **2, 4, 6, 8, 12, 16, 20, 24** for consistent rhythm
- Component padding: p-6, p-8, p-12
- Section spacing: py-12 md:py-20 lg:py-24
- Grid gaps: gap-6, gap-8
- Card spacing: space-y-6

### Container Strategy
- **Max Width**: max-w-7xl for full sections, max-w-4xl for forms
- **Responsive Padding**: px-4 md:px-8 lg:px-12

---

## Component Library

### Navigation
- Sticky header with logo, services menu, contact CTA
- WhatsApp floating button (bottom-right, mobile-optimized)
- Smooth scroll to service sections

### Hero Section
- Large hero image showing serene spa environment or treatment in progress
- Overlay with headline: "Tu Santuario de Bienestar y Transformación"
- Subheadline emphasizing expertise (e.g., "Carolina Arias - Masajista Profesional")
- Primary CTA: "Reservar Turno" + WhatsApp contact button
- Trust indicators: Years of experience, client testimonials count

### Service Catalog
- **Four Category Sections** (color-coded):
  - Therapeutic Massages (Indigo accents)
  - Specialized Care (Rose Pink accents)
  - Body Contouring (Amber accents)
  - Circulatory Treatments (Teal accents)
- **Accordion Cards**: Expandable service details with smooth transitions
- **Card Design**: Soft shadows (shadow-lg), rounded corners (rounded-xl), hover lift effect
- Icons for each category (💆‍♀️ 🤰 🔥 🌊)

### Booking Form Section
- Two-column layout (desktop): Form + Contact info/map
- Form fields: Name, Phone, Email, Service Selection (dropdown), Preferred Date/Time, Message
- WhatsApp quick-book alternative prominently displayed
- Trust elements: "Respuesta en 24 horas" badge

### Social Proof
- Client testimonials carousel (2-3 columns on desktop)
- Before/after results grid (if applicable)
- Professional certifications/badges

### Footer
- Contact information (phone, WhatsApp, location)
- Quick links to services
- Social media icons
- Operating hours
- Newsletter signup (optional wellness tips)

---

## Images

### Hero Image
Large full-width hero image (60-70vh) showing:
- Serene spa setting with soft lighting, massage table, or treatment in progress
- Warm, inviting atmosphere with beige/cream tones
- Professional yet relaxing aesthetic
- Overlay: Semi-transparent dark gradient (rgba(0,0,0,0.3)) for text readability

### Service Category Images
Small decorative images or icons for each service category header to enhance visual appeal and category recognition

### Testimonial Photos
Circular client photos (optional, with permission) or placeholder silhouettes

### Background Textures
Subtle gradient overlays (linear-gradient 135deg) on section backgrounds for depth without distraction

---

## Animations & Interactions
**Minimal & Purposeful**:
- Accordion expand/collapse: 0.3s ease transitions on max-height
- Card hover: Gentle lift (transform translateY(-4px)) with shadow increase
- Button hover: Subtle scale (1.02) and color deepening
- Smooth scroll for navigation links
- No autoplay carousels or distracting motion

---

## Accessibility & Responsiveness
- Consistent dark mode across all components
- Focus states with visible outlines matching category colors
- Mobile-first: Stack columns on mobile, expand to 2-3 columns on tablet/desktop
- Touch-friendly button sizes (min 44px height)
- Semantic HTML for screen readers
- ARIA labels for accordion controls