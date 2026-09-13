# Journi

**by 404 Brain Not Found**

**Team:** Yii Chin Hoo, Jasleen Kaur Sidhu A/P Karmu Singh, Mehrunisha A/P Applanaidu, Tan En Yi

**Problem Statement:** Travel Planner

- 🎥 [Video Presentation](https://youtu.be/MIz2poVAHdw)
- 📊 [Presentation Slides](https://canva.link/lcgy88ebcb6amz4)

---

## 1. Project Overview

Planning a multi-stop trip today is scattered across too many tools — travelers screenshot posts from social media, copy place names into notes apps, then separately search maps for directions and separately check the weather for each stop. When a trip involves more than one person, this gets worse: there's no shared source of truth, so groups fall back on long group chats to agree on where to go, and one person usually ends up manually consolidating everyone's preferences into a final plan. The stakeholders are therefore twofold: solo travelers who want a fast way to turn scattered inspiration into a workable itinerary, and groups of travelers who need to align on a shared plan without endless back-and-forth.

Existing apps address pieces of this but not the whole picture. **Paths (AI Travel Planner)** is the closest comparison — it lets users paste links or text to auto-generate an itinerary and offers route optimization with live maps and weather in one view. However, it is built around a single traveler's plan; it does not support real-time multi-person collaboration where a group can vote on destinations together and edit a shared itinerary simultaneously, which is where Journi differentiates itself.

### Our Solution

Journi is a travel planning app that takes a trip from scattered inspiration to a finished, shareable itinerary in one place. A traveler can paste a link or a rough description of what they want and get a day-by-day starting itinerary, refine the order of stops with a route optimizer that accounts for start/end points and travel mode, and uniquely bring their travel group into the same plan to vote on destinations and edit the itinerary together in real time, rather than negotiating over chat.

### Feature Set

- **AI Trip Planner** — describe your trip in your own words; Journi matches it against its destination catalog and generates a starting day-by-day itinerary with activities and timings.
- **Chat with a Travel Agent** — sanity-check your AI-generated plan with a human specialist, picked by destination, directly inside the AI Planner.
- **Smart Route Builder** — add must-visit stops, set a start/end point and travel mode, and get an optimized route on a live map with current weather per stop.
- **DIY Trip Builder** — a guided flow to compare and select flights, allocate your budget across flights/accommodation/food/activities/transport with drag sliders, and build a day-by-day schedule — including a "simulate flight delay" tool that reorganizes affected activities automatically.
- **Plan With Friends** — group setup with a shareable invite code, a swipe-to-match feature to vote on Tinder-style destinations, and a live collaborative board with comments and reactions on itinerary items.
- **Traveler Reviews** — browse past travelers' reviews, their real budget ranges, and full itineraries per destination, with the option to directly reuse a traveler's plan as your own starting point.
- **My Plan** — save every trip you build and reopen it later to view, edit, or remove it.

### 1. AI Trip Planner

Describe your trip in your own words: a destination, a vibe, a rough sentence like "5 days in Bali, beaches and temples." Journi matches that against its destination catalog and generates a full day-by-day itinerary with activities and timings, so travelers start from a real plan instead of a blank page.

### 2. Smart Route Builder

Add every place you want to visit, set a start and end point, and choose how you're getting around. Journi calculates the smartest order to see everything and shows it on a live map, along with real-time weather for each stop — combining routing and trip conditions into one screen.

### 3. DIY Trip Builder

For travelers who want full control, DIY Trip walks you through building a trip step by step — compare and choose real flights, allocate your budget across flights, accommodation, food, activities and transport, then build a day-by-day schedule. If plans change, a "simulate flight delay" tool reorganizes the affected parts of the schedule automatically instead of forcing a full rebuild.

### 4. Plan With Friends

Group trips usually turn into endless group-chat debates. Journi fixes that with a shareable invite code, a Tinder-style swipe to vote on destinations as a group, and a live shared itinerary board where members comment and react on plan items in real time.

### 5. Traveler Reviews

Before committing to a plan, travelers can browse genuine reviews from people who've visited the same destinations, with real ratings, budget ranges, and full itineraries. Travelers can even take a past traveler's plan directly and use it as the starting point for their own trip.

### 6. My Plan

Every itinerary a traveler builds through the AI Planner or DIY Trip is saved automatically. My Plan brings them all together in one place, so travelers can reopen, edit, customize, or remove any saved trip at any time.

---

## 2. Ideation & Process

### 2.1 Ideas We Considered

| Idea | Status | Why |
|---|---|---|
| Human/certified travel agent input (mentor-style guidance baked into the app) | Chosen — folded into AI Planner | Users wanted a second opinion beyond pure algorithmic suggestions, so we kept the "deeper local insight" idea but delivered it through curated destination data and reviews rather than a live human agent, since a real agent isn't feasible to staff for a hackathon build. |
| Route/travel map optimization | Chosen | Directly solves the "which order should I visit these places" pain point; became the Smart Route Builder. |
| Group collaboration & voting on destinations | Chosen | Identified as our key differentiator versus existing single-user planners; became the Plan with Friends feature (invite codes, swipe-to-match, live collab board). |
| Traveler reviews | Chosen | Help new users trust a suggested itinerary by seeing real past-traveler feedback, budget ranges and full itineraries they can reuse. |
| Budget planning and allocation | Chosen | Initially considered too complex to scope in time but ultimately built as a full Budget Planner step (flights, accommodation, food, activities, transport) inside the guided Trip Planner flow. |
| Guided flight + schedule builder (DIY Trip) | Chosen | Emerged as travelers needed to go from "itinerary idea" to something closer to a real, bookable plan; became the DIY Trip flow with flight comparison, budget allocation, and a schedule builder that can reorganize itself around disruptions like flight delays. |
| Fully autonomous AI agent (AI books and pays for the entire trip end-to-end with no user input) | Dropped | Too broad in scope for the hackathon timeframe and would require real payment/booking integrations we couldn't reliably build and test in time. We kept AI-assisted itinerary generation and flight comparison, but travelers still make the final selections themselves rather than the AI booking anything autonomously. |

### 2.2 Ideation Boards

![Ideation mind map](images/ideation-mindmap.jpg)

**Caption:** Our initial mind map branched the idea of "Journi – Travel Planner" into an AI agent for automated planning, a human/expert-agent angle for deeper local insight, a budget-planning angle, route optimization, and travel reviews. As the build progressed, the mind map grew further to include group collaboration (Plan with Friends), a fully guided DIY trip flow (flights, budget, schedule), destination exploration, and a My Plan area to save and revisit trips — reflecting how our scope expanded from a single AI-generated itinerary into a complete, end-to-end trip-planning experience.

### 2.3 Mentor Consultation

| Date | Mentor | Feedback Received | What Was Changed |
|---|---|---|---|
| 7 September 2026 | Mr. Khor Jia Quan (Stefan) | Brainstorming ideas; adding up AI features in the travel planner for convenient use among users. | Team have clearer picture of the project. |

---

## 3. Design & Prototype

- **UI Prototype:** https://journi-henna.vercel.app/
- **APK file:** https://drive.google.com/drive/folders/1dREvm9hM-qHYvHKFSzkalQji-qXkTf26?usp=sharing
- **AI Chatbot with functionality Prototype:** https://journi-umber.vercel.app/

### a. Homepage

Journi's landing page surfaces trending destinations and a single 'Plan Trip' entry point into the guided planner.

| Website View | Mobile App View |
|---|---|
| ![Homepage website](images/homepage-website.jpg) | ![Homepage mobile](images/homepage-mobile.jpg) |

### b. AI Planner (input + generated itinerary)

Travelers describe their trip in plain language and receive a generated day-by-day itinerary in seconds.

| Website View | Mobile App View |
|---|---|
| ![AI Planner website](images/ai-planner-website.jpg) | ![AI Planner mobile](images/ai-planner-mobile.jpg) |

### c. Chat with a Travel Agent panel

Travelers can sanity-check their AI itinerary with a human specialist picked by destination.

| Website View | Mobile App View |
|---|---|
| ![Travel agent website](images/travel-agent-website.jpg) | ![Travel agent mobile](images/travel-agent-mobile.jpg) |

### d. Route Builder (map + stops)

Adding stops and optimizing generates a live routed map with real travel times and per-stop weather.

| Website View | Mobile App View |
|---|---|
| ![Route builder website](images/route-builder-website.jpg) | ![Route builder mobile 1](images/route-builder-mobile-1.jpg) ![Route builder mobile 2](images/route-builder-mobile-2.jpg) |

### e. DIY Trip — Flights step

Guided flight comparison lets travelers pick real flight options by price and duration.

| Website View | Mobile App View |
|---|---|
| ![DIY flights website](images/diy-flights-website.jpg) | ![DIY flights mobile](images/diy-flights-mobile.jpg) |

### f. DIY Trip — Budget step

Drag-slider budget allocation across flights, accommodation, food, activities and transport.

| Website View | Mobile App View |
|---|---|
| ![DIY budget website](images/diy-budget-website.jpg) | ![DIY budget mobile](images/diy-budget-mobile.jpg) |

### g. DIY Trip — Schedule step

The day-by-day schedule can be reorganized instantly around disruptions, such as a simulated flight delay.

| Website View | Mobile App View |
|---|---|
| ![DIY schedule website](images/diy-schedule-website.jpg) | ![DIY schedule mobile](images/diy-schedule-mobile.jpg) |

### h. Plan With Friends (swipe + collab board)

Groups vote on destinations Tinder-style, then plan together in real time on a shared board.

| Website View | Mobile App View |
|---|---|
| ![Plan with friends website](images/plan-with-friends-website.jpg) | ![Plan with friends mobile 1](images/plan-with-friends-mobile-1.jpg) ![Plan with friends mobile 2](images/plan-with-friends-mobile-2.jpg) |

---

## 4. What Makes It Different

Journi's core differentiation is that it doesn't stop at generating an itinerary — it carries a trip from raw inspiration all the way through to something bookable and shareable, for both solo and group travelers, in one continuous flow rather than a single feature:

a. **Group-native planning, not solo-only.** Most AI trip planners are built around one traveler's plan. Journi's Plan with Friends turns destination selection into a group decision (swipe-to-vote) and keeps the itinerary editable live by everyone involved — this is Journi's most original feature.

b. **AI generation and human backup, in the same flow.** Rather than forcing a traveler to trust a fully automated itinerary, Journi pairs the AI Trip Planner with an optional live "Chat with a Travel Agent," so users can validate or adjust the AI's suggestions with a real specialist without leaving the app.

c. **Planning that survives real-world disruption.** The DIY Trip schedule builder includes a "simulate flight delay" tool that automatically reorganizes affected activities — most itinerary generators produce a static plan that must be manually rebuilt the moment something changes.

d. **Budget as a first-class part of planning, not an afterthought.** Flights, accommodation, food, activities and transport are allocated and visualized together against a total budget target, rather than estimated separately from the itinerary.

| Capability | Paths | Journi |
|---|:---:|:---:|
| AI-generated itinerary from text/links | ✓ | ✓ |
| Route optimization + live map/weather | ✓ | ✓ |
| Group voting & real-time collaboration | ✗ | ✓ |
| Flight comparison | ✗ | ✓ |
| Budget allocation | ✗ | ✓ |
| Human travel agent chat | ✗ | ✓ |

---

## 5. Technical Architecture & Feasibility

**UI Prototype** ([https://journi-henna.vercel.app/](https://journi-henna.vercel.app/)), used in the presentation, is a static, frontend-only travel-planning app built with plain HTML, CSS, and JavaScript — no framework or bundler, and the "backend" is entirely `localStorage`.

**AI Chatbot with functionality Prototype:** [https://journi-umber.vercel.app/](https://journi-umber.vercel.app/) — tech stack below.

### 1. Frontend

- **Next.js 16 + React 19** — delivers native streaming token rendering (`ReadableStream`), instant hydration, and modular component architecture.
- **Tailwind CSS v4** — zero-runtime utility styling with CSS variable theming, providing a dark mode default (`#121214` charcoal background, `#2e2e34` subtle borders) with instant light mode toggle.
- **Web Speech API** — zero-cost, browser-native speech recognition for voice input without external API keys.

### 2. Backend & Database

- **Supabase (Postgres + PostGIS + Auth + Realtime)** — one platform for the database, geo queries ("places near me"), login, and live sync (Realtime broadcasts row changes over WebSockets so collaborators see drags instantly); Row Level Security enforces who can edit what.
- **Supabase Edge Functions (Deno)** — keeps OpenRouter and Google API keys off the client, with fast cold starts.

**Constraints:** Vercel serverless functions have execution limits (15–60s on the Hobby tier). Exceptionally long prompts or slow models could time out.

### 3. Third-Party APIs

- **OpenRouter (free models)** — extracts structured trip data (places, dates) from messy captions/notes, at $0 per token.
- **OpenStreetMap** — free, open-source mapping iframe embeds that require no API keys, billing accounts, or rate limits for destination previews.

**Constraints:** the free tier is capped at 20 requests/minute and 50/day. Free models are generally less reliable than Claude at sticking to a schema, so we might need to add output validation + a retry-with-reprompt step. OpenStreetMap is a static iframe embed rather than a dynamic route-calculating routing engine.

### System Architecture Diagram

![System architecture diagram](images/system-architecture.jpg)

### Build Plan & Scope

As Journi evolves beyond its initial release, several targeted upgrades to the technology stack are planned to unlock advanced travel capabilities and support higher scale:

First, we plan to transition the mapping layer from OpenStreetMap frame embeds to the **Google Maps Platform API**. While OpenStreetMap serves well as a lightweight, zero-cost embed, migrating to Google Maps will unlock critical travel planning features such as the Google Maps Directions & Routes API for multi-stop itinerary route optimization, interactive turn-by-turn navigation between daily attractions, real-time public transit schedules, estimated walking and driving times between itinerary checkpoints, Google Street View previews, and rich Places API metadata including user ratings, opening hours, and photos. This allows Journi not only to suggest destinations, but to calculate the most time-efficient order to visit each attraction in a day.

Additionally, the AI integration layer will be significantly enhanced by implementing native AI function calling and tool use.

Specifically, we want to implement real-time flight searching tools to look up live airfares, flight schedules, layovers, and airline seat availability, alongside live lookup tools that fetch up-to-date travel information including current weather forecasts, currency exchange rates, visa entry requirements, destination safety advisories, and seasonal local event schedules.
