# Paw & Fin UI Design Plan

## 1. Product Vision
Paw & Fin should feel like a premium editorial marketplace instead of a generic ecommerce grid. The experience combines:

- organic asymmetry
- layered glass surfaces
- nature-meets-water color contrast
- responsive layouts that stay familiar on phone, tablet, laptop, desktop, and TV
- motion that feels calm and alive rather than flashy

The visual goal is "The Organic Curator": a refined marketplace where pets, aquatic life, and trusted sellers feel carefully presented.

## 2. UX Goals
- Make discovery easy for first-time buyers.
- Make selling feel guided and low-friction.
- Give admins strong visibility without making the admin area visually harsh.
- Keep role switching simple when a user has both buyer and seller access.
- Design every major flow for future API-driven mobile reuse.

## 3. Primary User Flows

### Buyer Flow
- Land on editorial homepage
- Explore featured pets, categories, care guides, and live auctions
- Search and filter listings
- Open detail page
- Choose: buy now, bargain, chat, or join auction
- Manage profile, wishlist, orders, and saved searches

### Seller Flow
- Login with seller role or switch from buyer profile
- View seller dashboard
- Create listings
- Upload pet details, images, pricing, availability, and auction settings
- Track inquiries, bargain offers, chats, and orders

### Admin Flow
- Review seller applications
- Approve or reject pet listings
- Approve or reject auctions
- Trigger auction visibility and notifications
- Monitor platform analytics, reports, and fraud signals

## 4. Information Architecture

### Public Pages
- Home
- Marketplace / browse
- Pet detail
- Auction hub
- Seller showcase
- Care guides / editorial stories
- Login / role selection

### Authenticated Buyer Pages
- Buyer dashboard
- Wishlist
- Orders
- Messages
- Bargaining center
- Profile and role switcher

### Authenticated Seller Pages
- Seller dashboard
- Listings manager
- Create / edit listing
- Auction manager
- Orders / leads
- Messages
- Store profile

### Admin Pages
- Admin overview
- Seller approvals
- Listing moderation
- Auction approvals
- Users
- Reports / analytics

## 5. Page-by-Page Design Direction

### Home
- Large editorial hero with layered gradients and 3D ambient scene
- Split storytelling blocks for land pets and aquatic pets
- Staggered featured pet grid
- Live auction strip with countdown cards
- Trust section: verified sellers, safe handling, adoption guidance
- Footer with marketplace links and care content

### Marketplace Listing Page
- Floating filter rail on desktop, bottom sheet filters on mobile
- Search and smart category chips
- Offset card rhythm to avoid a rigid grid
- Quick actions on cards: save, chat, bargain, auction

### Pet Detail Page
- Immersive image gallery with glass overlay info cards
- Seller identity module
- Purchase panel with buy now, bargain, chat, auction tabs
- Health, breed, location, age, and care details
- Similar pets and related guides below

### Login and Role Selection
- Clean, welcoming layout with role-aware messaging
- Email-first login
- If buyer and seller both exist, show a role modal instead of forcing a separate page
- Use profile page for later switching between buyer and seller

### Buyer Dashboard
- Personalized greeting
- Order status cards
- Saved pets
- Bargain offers and chat activity
- Suggested pets based on browsing

### Seller Dashboard
- Revenue and inquiry summary
- Listing performance
- Drafts, pending approvals, live listings, auction status
- Fast action cards for new listing and auction request

### Admin Dashboard
- Modular analytics tiles
- Pending approvals queue
- Fraud / report alerts
- Email broadcast status for approved auctions
- Dense data, but still aligned with the same brand system

## 6. Visual System Translation

### Color Application
- `primary #005050` for trust, water, premium action areas
- `secondary #006e1c` for land, growth, seller-positive actions
- `surface #f7faf9` as the main canvas
- Use tonal layering instead of borders to separate sections

### Surface Strategy
- Base page: `surface`
- Section blocks: `surface_container_low`
- Cards and floating nav: `surface_container_lowest` with translucency
- Avoid hard dividers across the product

### Typography
- Plus Jakarta Sans for hero lines, headline moments, and marketplace authority
- Manrope for body copy, filters, supporting details, dashboard content
- Label text should be uppercase with tracking for polish and scanability

### Shape Language
- Hero containers: large flowing radii
- Cards: 3rem radius
- Buttons and chips: full pill shape
- Avoid sharp corners unless used as a deliberate accent in charts or admin modules

## 7. Motion and 3D Plan

### Motion Principles
- Slow, breathable, editorial pacing
- Use reveal, parallax, floating depth, and stagger instead of excessive bouncing
- Motion must never block task completion

### 3D Usage
- Homepage hero: floating abstract paw-fin sculpture or pet silhouette environment
- Listing cards: subtle hover tilt and depth lighting
- Detail page: layered parallax gallery and animated info panels
- Auction section: soft pulse and countdown emphasis

### Suggested Tech
- CSS transforms for lightweight UI motion
- GSAP for reveal sequences and scroll choreography
- Three.js for hero-only immersive 3D scenes
- Keep 3D effects optional on low-power devices

## 8. Responsive Strategy

### Mobile
- Bottom floating navigation
- Full-width cards
- Sticky action bar on detail page
- Filters inside slide-up drawer

### Tablet
- Two-column card grid
- Expanded floating nav
- Split detail layout for gallery and purchase panel

### Laptop / Desktop
- Editorial hero
- Staggered three-column browse layout
- Floating side filters
- Dual-panel dashboards

### TV / Large Displays
- Larger spacing and type scale
- Fewer columns with larger cards
- Focus-safe navigation for remote-style browsing in future

## 9. Key Components
- Floating glass nav
- Editorial hero module
- Staggered pet card
- Habitat badge
- Search field with chip filters
- Seller trust card
- Auction card with countdown
- Bargain panel
- Chat dock / assistant panel
- Role switcher modal
- Profile role chip set
- Dashboard metric tile
- Approval queue card

## 10. Feature-Specific UI Notes

### Bargaining
- Present as a respectful negotiation panel, not a discount gimmick
- Use offer timeline cards showing seller response history
- Add status states: pending, countered, accepted, declined

### Chatbot
- Floating assistant entry point on all key pages
- Use it for help, onboarding, FAQs, care tips, and marketplace support
- Desktop: right-side dock
- Mobile: expandable bottom sheet

### Auction
- Seller can request auction during listing creation
- Admin approval state should be visible in seller dashboard
- Once approved, auction card appears in live auction hub
- Add email notice event in backend flow and visible confirmation in admin panel

## 11. Build Sequence

### Phase 1
- Tokenize colors, spacing, radii, shadows, typography
- Build base layout and navigation
- Build homepage and browse page

### Phase 2
- Build pet detail page
- Build login, role modal, profile role switcher
- Build buyer dashboard

### Phase 3
- Build seller dashboard and listing creation flow
- Build bargain and chat interfaces
- Build auction request and live auction UI

### Phase 4
- Build admin moderation and analytics screens
- Add richer 3D scenes and performance fallbacks
- Refine accessibility and TV layout behavior

## 12. Accessibility Rules
- Never depend on color alone for status
- Maintain strong contrast on glass surfaces
- Respect reduced motion preferences
- Ensure touch targets are large enough on mobile and tablet
- Keep font sizes generous for long-form reading and TV distance viewing

## 13. Immediate Next Deliverables
- Wireframes for Home, Marketplace, Pet Detail, Login, Buyer Dashboard, Seller Dashboard, Admin Dashboard
- Component inventory based on the design tokens
- High-fidelity desktop and mobile homepage
- Interaction prototype for role selection, bargain flow, and auction approval journey
