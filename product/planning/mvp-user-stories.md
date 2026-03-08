# toddleSpot — MVP User Stories

> Platform: iOS native (Swift)
> Auth model: Browse free, account required to contribute (reviews, favourites)
> Launch area: London (starting with Upminster and surrounding neighbourhoods)

---

## 1. Venue Discovery

### 1.1 Browse by Category
**As a** parent browsing the app,
**I want to** tap a category tag (e.g. Cafés, Parks, Soft Play, Restaurants),
**So that** I can see nearby venues of that type.

**Acceptance criteria:**
- Home screen shows category tags (Cafés, Parks, Soft Play, Restaurants, Libraries, Leisure Centres, Pubs)
- Tapping a tag shows a list of venues in that category, ordered by distance from user
- Each venue card shows: name, distance, overall baby-friendliness score, top 2-3 attribute icons
- Empty state if no venues in category nearby

### 1.2 Search by Name or Type
**As a** parent looking for a specific place,
**I want to** search by venue name or type,
**So that** I can quickly find what I'm looking for.

**Acceptance criteria:**
- Search bar accessible from home screen
- Returns results matching venue name or category
- Results show same venue card format as category browse
- Shows "No results" state with suggestion to browse categories

### 1.3 Map View
**As a** parent planning an outing,
**I want to** see venues on a map relative to my location,
**So that** I can find places nearby at a glance.

**Acceptance criteria:**
- Map centres on user's current location
- Venues shown as pins with colour coding by baby-friendliness score (green = great, amber = ok, red = poor, grey = not yet rated)
- Tapping a pin shows a mini venue card with name, score, and distance
- Tapping the mini card navigates to the full venue detail page
- Can filter map pins by category

---

## 2. Venue Detail

### 2.1 View Venue Details
**As a** parent considering a venue,
**I want to** see detailed baby-friendliness information,
**So that** I can decide if it's suitable before I go.

**Acceptance criteria:**
- Venue detail page shows:
  - Venue name, address, category
  - Overall baby-friendliness score (composite)
  - Individual attribute scores with icons:
    - Baby changing facilities
    - High chairs available
    - Pram/buggy access
    - Parking availability
    - Nearest train station + step-free access
    - Breastfeeding welcome
    - Noise tolerance
    - Allergen-aware menus
    - Play areas
    - Safety considerations
  - Each attribute shows a confidence indicator (e.g. "4 out of 5 parents confirmed")
  - Number of reviews
  - Link to open location in Apple Maps for directions

### 2.2 Read Parent Reviews
**As a** parent researching a venue,
**I want to** read reviews from other parents,
**So that** I can get real-world advice and tips.

**Acceptance criteria:**
- Reviews section on venue detail page
- Each review shows: author display name, date, child age at time of visit, attribute ratings, free-text tip/comment
- Reviews ordered by most recent first
- Shows "No reviews yet — be the first!" if empty

---

## 3. Reviews & Contributions (Auth Required)

### 3.1 Create an Account
**As a** parent who wants to contribute,
**I want to** create an account,
**So that** I can leave reviews and save favourites.

**Acceptance criteria:**
- Sign up with email + password or Sign in with Apple
- Profile setup: display name, number of children, age of each child
- Child age stored as date of birth (to auto-update age over time)
- Clear explanation of why child age is collected ("to help us show you relevant info")
- Can skip child info and add later

### 3.2 Sign In
**As a** returning user,
**I want to** sign into my account,
**So that** I can access my profile and leave reviews.

**Acceptance criteria:**
- Sign in with email + password or Sign in with Apple
- "Forgot password" flow via email
- Stays signed in until explicit sign out

### 3.3 Leave a Review
**As a** parent who has visited a venue,
**I want to** leave a structured review,
**So that** other parents benefit from my experience.

**Acceptance criteria:**
- Review form accessible from venue detail page
- Must be signed in (prompt to sign up/in if not)
- Structured rating: tick yes/no/not sure for each baby-friendly attribute
- Optional free-text field for tips and comments (e.g. "Ask for the high chair, they keep them in the back")
- Optional: child age at time of visit (pre-filled from profile if available)
- Submit updates the venue's attribute scores in real time
- One review per user per venue (can edit their own review later)
- Confirmation message on successful submission

### 3.4 Edit My Review
**As a** parent who left a review,
**I want to** edit it if things have changed,
**So that** the information stays accurate.

**Acceptance criteria:**
- "Edit review" option on venues where user has reviewed
- Same form as leaving a review, pre-filled with previous answers
- Updated review replaces the old one (with updated date)

---

## 4. Favourites (Auth Required)

### 4.1 Save a Venue to Favourites
**As a** parent planning future outings,
**I want to** save venues I'm interested in,
**So that** I can easily find them later.

**Acceptance criteria:**
- Heart/bookmark icon on venue cards and venue detail page
- Must be signed in (prompt if not)
- Tapping saves/unsaves the venue
- Visual feedback (filled/unfilled icon)

### 4.2 View My Favourites
**As a** parent with saved venues,
**I want to** see all my favourites in one place,
**So that** I can quickly pick where to go.

**Acceptance criteria:**
- Favourites tab/section accessible from main navigation
- Shows saved venues in same card format as browse
- Can remove from favourites
- Empty state: "No favourites yet — start exploring!"

---

## 5. User Profile

### 5.1 View and Edit Profile
**As a** registered user,
**I want to** view and update my profile,
**So that** my information stays current.

**Acceptance criteria:**
- Profile screen shows: display name, email, children (name-free, age only)
- Can edit display name
- Can add/remove children and update ages
- Can sign out
- Link to privacy policy

---

## 6. Location

### 6.1 Use Current Location
**As a** parent using the app,
**I want** the app to use my location,
**So that** I see venues near me.

**Acceptance criteria:**
- iOS location permission prompt on first use with clear explanation
- App uses current location to sort venues by distance and centre map
- Graceful fallback if permission denied: allow manual location entry or postcode search
- Location refreshes when app returns to foreground

---

## Out of Scope (Post-MVP)

- Book Now / venue reservations
- "What others did next" trip chaining
- User-generated itineraries
- Recommendations / classes / events feed
- Forum / community features
- Offline mode
- Personalised recommendations based on child age
- Photo uploads on reviews
- Push notifications
- Android version
- Venue owner self-service / claiming
