# AI Map Planner


Created an AI Map Planner that helps daily commuters and occasional visitors compare vehicle prices and find alternative routes in one place built using Claude and Lovable.

---

## 1. Problem Statement

Planning a trip today whether it's a daily commute or a multi-stop errand run requires users to juggle multiple apps and manual steps: searching for a destination, comparing routes, checking traffic, and separately opening ride-hailing or transit apps to compare prices across providers. This process is fragmented, time-consuming, and cognitively taxing, especially for users who are in a hurry, unfamiliar with an area, or trying to optimize for cost rather than just speed.

**Who feels this pain:**
- **Daily commuters and city dwellers** who want the fastest or cheapest way to get somewhere without price-checking 3-4 apps.
- **Travelers and occasional visitors** to a city who don't know the local transit/ride landscape and want a single trusted assistant to just "get them there."

**The core pain point:** there is no single conversational interface where a user can simply state their destination and intent ("I want to go to X, cheapest way possible" or "get me there fastest") and receive a synthesized, ranked set of route and vehicle options instead of manually searching, comparing, and switching between apps.

---

## 2. Goals

1. **Reduce trip-planning time**: Decrease average time-to-decision (from stating intent to selecting a route) to under **30 seconds**, down from an estimated 3-5 minutes of manual cross-app comparison.
2. **Drive cost savings for users**: Achieve an average of **15% cost savings per trip** compared to a user's default/habitual choice (measured via post-trip surveys or price comparison logging).
3. **Increase task completion rate**: Reach a **70%+ route selection completion rate** i.e., of users who input a destination, 70% go on to select and act on a suggested route (vs. abandoning to search manually elsewhere).

---

## 3. User Personas

### Persona 1: "Efficient Emma" - The Daily Commuter
- **Age/context:** 29, works in a mid-size city, commutes 5 days/week, occasionally runs errands after work.
- **Behavior:** Price and time-sensitive. Currently switches between two or three ride-hailing/transit apps to compare before booking.
- **Needs:** A fast, low-effort way to see her best option without repetitive manual comparison. Values consistency and trust in recommendations over time.
- **Frustration:** "I waste 5 minutes every day just comparing apps for a trip I take all the time."

### Persona 2: "Traveling Tom" - The Occasional Visitor
- **Age/context:** 41, frequently travels to unfamiliar cities for work or leisure.
- **Behavior:** Doesn't know local transit options, pricing norms, or which apps are trustworthy/available in a new city.
- **Needs:** A single, reliable assistant that understands local context (available vehicles, typical pricing, safe routes) and removes the guesswork.
- **Frustration:** "I don't know what's normal here am I overpaying? Is there a train I don't know about?"

---

## 4. User Stories

1. As a **daily commuter**, I want to **tell the AI my destination in plain language** so that **I don't have to manually type addresses into multiple apps**.
2. As a **traveler in an unfamiliar city**, I want to **see all available route and vehicle options in one place** so that **I can make an informed choice without knowing the local transit landscape**.
3. As a **price-conscious user**, I want to **see routes ranked by price** so that **I can pick the cheapest option without comparing apps myself**.
4. As a **time-conscious user**, I want to **see routes ranked by estimated travel time** so that **I can choose speed when I'm in a hurry**.
5. As a **returning user**, I want the **AI to remember my frequent destinations and preferences** so that **future trip planning is even faster**.

---

## 5. Feature List (MVP)

- **Conversational input**: Natural-language destination entry (text and voice), e.g., "Take me to the airport."
- **Location detection**: Auto-detect current location (with permission) as the default starting point.
- **Route generation engine**: Generate 2-4 alternative routes per request across available modes (walking, driving, ride-hail, public transit, where integrated).
- **Price comparison**: Pull and display estimated pricing across integrated vehicle/ride providers for each route option.
- **Ranking & filtering**: Sort/filter results by price, time, or a "best value" blended score.
- **Route summary card**: Each option shows ETA, price, distance, and vehicle/mode type at a glance.
- **One-tap handoff**: Deep-link or handoff to the selected provider's app (or in-app booking, if supported) to finalize the trip.
- **Basic trip history**: Store recent destinations for quick re-access.

---

## 6. What We Are NOT Building (Out of Scope for MVP)

1. **In-app booking/payment processing** - MVP will deep-link to third-party provider apps rather than handling bookings or payments natively.
2. **Real-time turn-by-turn navigation** - this is a route *planning and comparison* tool, not a replacement for dedicated navigation apps like Google Maps or Waze.
3. **Multi-modal trip chaining / complex itinerary planning** (e.g., multi-city trip planning, calendar integration) - MVP focuses on single point-to-point trips only.

---

## 7. Success Metrics

- **Adoption:** % of users who complete at least one AI-guided route search per week.
- **Time-to-decision:** Median time from input to route selection (target: <30 seconds).
- **Cost savings:** Average % savings vs. baseline/self-reported habitual choice.
- **Completion rate:** % of searches that result in a selected route (target: 70%+).
- **Retention:** % of users returning to use the planner again within 7 and 30 days.
- **User satisfaction:** CSAT/NPS score collected post-trip (target: NPS > 40).

Author - Jasleen Kaur
For full PRD - https://glowing-rib-edb.notion.site/PRD-AI-Map-Planner-3a157abc392c80a39da0d34263006c26?source=copy_link
