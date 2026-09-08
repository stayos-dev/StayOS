# StayOS

StayOS is a multi-tenant hotel management and website platform designed for independent hotels. It aims to help hotel owners create their online presence, manage property information and handle daily hotel operations from one place.

## Current Status

StayOS is currently in the frontend foundation stage. The Angular workspace and the first application have been initialized. The onboarding screens are being implemented as standalone Angular components from approved wireframes.

The current work is static and does not yet include APIs, authentication, database integration or live booking functionality.

## Planned Product Screens

### Public and Account

1. Landing Page
2. Sign Up
3. Sign In

### Hotel Onboarding

4. Web Address
5. Property Details
6. Room Types
7. Photos
8. Rates
9. Website
10. Connect Google
11. You Are Live

### Hotel Operations

12. Morning Queue
13. Front Desk
14. Review Inbox
15. Review Reply
16. Check In
17. Guest Profile
18. Reports


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
