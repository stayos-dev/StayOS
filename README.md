# StayOS

StayOS is a multi-tenant hotel management and website platform designed for independent hotels. It aims to help hotel owners create their online presence, manage property information and handle daily hotel operations from one place.

## Current Status

StayOS is currently in the frontend foundation stage. The Angular workspace and the first application have been initialized. The onboarding screens are being implemented as standalone Angular components from approved wireframes.

The current work is static and does not yet include APIs, authentication, database integration or live booking functionality.

## Planned Onboarding Flow

1. Signup
2. Web address
3. Property details
4. Room types
5. Photos
6. Rates
7. Website template
8. Connect Google listing
9. Confirmation / go live

## Future Plans

**Phase 1 — Onboarding UI (current)**
Build all onboarding screens as static, standalone Angular components matching the approved wireframes. No backend calls yet.

**Phase 2 — Data layer**
Design and set up the core database schema (tenants, properties, room types, rooms, rates, guests, reservations, reviews). Connect the onboarding screens to real APIs so data entered in the wizard is actually saved.

**Phase 3 — Authentication**
Add signup/login, session handling, and multi-tenant access control so each hotel only sees its own data.

**Phase 4 — Core operations**
Build the day-to-day screens: front desk (room chart, check-in/check-out), review inbox, guest profiles, and reports.

**Phase 5 — Booking engine**
Enable live availability, rates, and payments so guests can book directly through the hotel's own website.

**Phase 6 — Public launch prep**
Polish, testing, deployment pipeline, and onboarding real hotels.

Each phase builds on the previous one — later phases will only start once the current phase is stable.

## Technology

* Angular
* TypeScript
* HTML
* SCSS
* Git and GitHub

## Project Structure

```text
StayOS/
├── projects/
│   └── stayos/
│       └── src/
│           ├── app/
│           ├── index.html
│           ├── main.ts
│           └── styles.scss
├── angular.json
├── package.json
└── tsconfig.json
```

The repository uses an Angular workspace structure so additional applications and shared libraries can be added later.

## Local Setup

Clone the repository:

```bash
git clone https://github.com/stayos-dev/StayOS.git
cd StayOS
```

Install dependencies:

```bash
npm install
```

Start the StayOS application:

```bash
ng serve stayos
```

Open `http://localhost:4200` in the browser.

## Build

```bash
ng build stayos
```

## Tests

```bash
ng test stayos
```

## Development Workflow

* Pull the latest `main` branch before starting.
* Create a separate `feature/*` branch for each task.
* Keep one standalone Angular component per screen.
* Build the desktop layout first and verify it at 1280px.
* Make the same screen responsive down to 390px.
* Use shared styles and SCSS variables instead of repeating colour values.
* Open a pull request to `main`.
* Get at least one teammate review before merging.

## Team

StayOS is being designed and developed collaboratively as a hotel technology project.
