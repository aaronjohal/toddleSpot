# ToddleSpot - Product Discovery

## Founder Context
- Aaron is a product manager building this as a side project alongside main job
- Goal: grow into a full business eventually
- Triggered by personal experience on paternity leave — struggled to find baby-friendly places
- Based in Upminster, Essex (launch city)

---

## Batch 1: Vision & Problem Space

### Problem Definition
- **Core pain:** Parents (especially first-time) struggle to identify baby-friendly venues — changing facilities, high chairs, pram access, best times to visit, step-free station access, nearby suitable parks
- **Current solutions are fragmented:**
  - Word of mouth / NCT class WhatsApp groups
  - Google Maps (helps find places but no baby-friendliness info)
  - Mums Reddit groups, Peanut app (community but not planning)
  - No single app consolidates this into an accessible, friendly UX
- **Gap:** Information is scattered across apps, forums, and word of mouth. First-time parents don't even know where to look. The world feels daunting with a new child.

### Target User
- **Child age range:** Newborns and toddlers (to start)
- **Primary persona:** First-time parents (but useful for all parents with newborns/toddlers)
- **Geographic scope:** Start with Upminster, Essex — build to scale to other cities

### Core Value Proposition
- Search for venues/amenities and see if they are baby-friendly, what makes them baby-friendly, and their rating
- **Key differentiator:** Joins the dots — helps you *plan* outings (e.g. best time to visit a coffee shop, how others got there, what route to take with a pram)
- Both discovery of new places AND validation of known places

### "Child-Friendly" Attributes (initial list — needs research to expand)
- Baby changing facilities
- High chairs available
- Pram/buggy access
- Best times to visit (quieter times, baby-friendly hours)
- Step-free access (stations/transport)
- Nearby suitable parks
- Breastfeeding welcome
- Noise tolerance
- Allergen-aware menus
- Play areas
- Safety considerations
- Parking availability (and ease of parking with children)
- Nearby train station (and step-free access status)

### Business Model (to be validated)
- Potential revenue streams:
  - Ads / sponsored venue placements
  - Subscription model with discounts at baby-friendly venues
  - Affiliate partnerships
- Needs validation before committing to a model

---

## Batch 2: User Experience & Features

### Core User Journey (Saturday morning example)
1. Open app → tap a tag for activity type (e.g. "Coffee")
2. List of nearby coffee shops appears
3. Tap one → see all baby-friendly info (aggregated from parent reviews)
4. Option to add own review
5. **"Book Now"** → book a slot directly with the venue, select needs (high chair, etc.) so they can prepare
6. See "How to get there" + "What others did next" (e.g. "parents went to X park after" with rating + distance)
7. **Recommendations tab** → shows baby sensory classes, other activities near me
8. **Search bar** for open-ended search
9. After visit → prompted to leave a review scoring specific baby-friendly criteria
10. Word-of-mouth growth: tell a friend → they download → register → cycle continues

### Search & Discovery Model
- Both "search engine" (I know what I want) AND "feed/discovery" (show me what's good nearby)

### Planning is Core
- Very important — help parents plan their whole outing, not just find one venue
- Key pattern: parents want options around a primary activity (coffee shop → then sensory class → then park)
- Surface context like: mums meetups happening nearby, classes, parks within walking distance

### Content & Data Strategy
- **Crowdsourced** — parents input reviews based on specific baby-friendly criteria
- Each criterion gets a score/percentage (e.g. "100% of reviewers said this place has a high chair")
- **Accuracy/trust system:** If pattern emerges (e.g. multiple parents tick "no high chair"), system flags the venue for update
- Confidence score builds trust (parents can see how many people confirmed each attribute)

### Photo Uploads
- (Not yet discussed — to revisit)

### Social & Community
- **Utility tool first** — not trying to replace WhatsApp groups
- Forum/community could come later as a future phase
- **User-generated itineraries** — yes, dedicated tab (e.g. "My perfect rainy day in Upminster with a 6-month-old")

### Personalisation
- **User profile setup** with child information:
  - Number of children
  - Ages of each child
  - Ability to update over time (e.g. new baby born)
- App adapts recommendations based on child age (newborn vs walking toddler = different needs)

### Filters
- To be discovered/evolved over time through user research
- Initial candidates: distance, cost, indoor/outdoor, time available, transport mode
- List will change as we learn from users
## Batch 3: Technical & Platform

### Platform Decision
- **iOS native app** — chosen for functionality over PWA
- Go-to-market on iOS first; Android later based on demand

### Build Context
- Solo founder building with AI assistance (needs hands-on help)
- Small personal budget (bootstrapped)
- No fixed timeline but wants steady progress

### Data Seeding
- Aaron will manually seed venue data for Upminster himself (visit places, enter first reviews)

### Offline
- App won't work offline but some caching should be in place for smoother UX

### Booking Integration
- Post-MVP — approach TBD (direct venue relationships vs. platform integration like OpenTable)

---

## MVP Definition (v1.0)

### In Scope
1. **Tag-based browse** — tap activity tags (Coffee, Parks, Soft Play, etc.) to see nearby venues
2. **Venue detail page** — baby-friendly attributes with crowdsourced scores:
   - Baby changing facilities
   - High chairs
   - Pram/buggy access
   - Parking availability
   - Nearest train station + step-free access
   - Breastfeeding welcome
   - Noise tolerance
   - Allergen-aware menus
   - Play areas
   - Safety considerations
3. **Leave a review** — structured form (tick/rate specific baby-friendly criteria, not just stars)
4. **User profile** — sign up, add children (name, age), location
5. **Map view** — venues on a map relative to user location
6. **Basic search** — search by name or type of venue

### Out of Scope (Roadmap / Post-MVP)
- Book Now (requires venue partnerships)
- "What others did next" trip chaining
- User-generated itineraries tab
- Recommendations / classes / events
- Forum / community features
- Offline mode
- Personalised recommendations based on child age (profile captures data, smart recs come later)

### Key Validation Metric
- Are parents leaving reviews without being prompted? If yes → product-market fit signal
## Batch 4: Go-to-Market & Growth

### Launch Strategy
- **Seed 20-30 venues** before launch across categories:
  - 8-10 cafes/restaurants
  - 5-6 parks
  - 3-4 soft play / indoor venues
  - 3-4 other (libraries, leisure centres, baby classes)
  - Cover Upminster + surrounding areas (Hornchurch, Cranham, Harold Wood)
  - Aaron to seed from personal experience
- **Beta testers:** Small group of parent friends available
- **First 50-500 users strategy:**
  - Promote at NCT groups
  - Online forums, Reddit parenting subs
  - Social media (Instagram, Facebook parenting groups)

### Brand & Identity
- **App name:** toddleSpot
- **Look & feel:** TBD — needs prototypes to decide (playful? minimal? warm?)
- Design exploration needed as a next step

### Competition
- **Research needed** — Aaron to ask Claude to conduct competitor analysis (Hoop, Kiddio, Mumli, FamilyApp, etc.)

### Positioning / Why Choose toddleSpot Over WhatsApp?
- Convenience — everything in one place
- Trust — crowdsourced scores with confidence percentages
- Features that make it the go-to (eventually removes the need to ask on WhatsApp because more validation lives here)

### Legal & Data Privacy
- **GDPR applies** — collecting data about children (ages) in the UK
- **UK Children's Code (Age Appropriate Design Code)** is relevant
- **MVP decision: collect child AGE only, not name** — reduces privacy burden significantly
- Will need: basic privacy policy, lawful basis for data processing
- Full compliance review needed before launch
- Venue self-service listings = post-MVP (but future revenue path)

---

## Outstanding Actions
- [ ] Competitor research (Hoop, Kiddio, Mumli, FamilyApp, others)
- [ ] Design prototypes / look & feel exploration
- [ ] Define detailed user stories for MVP features
- [ ] Technical architecture decision (Swift native? React Native? Flutter?)
- [ ] Data model design (venues, reviews, users, attributes)
- [ ] Privacy policy draft
- [ ] Venue seeding plan for Upminster area
