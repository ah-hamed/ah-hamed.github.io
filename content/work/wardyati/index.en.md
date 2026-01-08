---
title: Wardyati (وردياتي) - Shift Management System for Doctors
tags:
  - Webapp
  - Django
date: 2024-08-11
cover:
    image: "cover/wardyati-cover.png"
    alt: "Wardyati Cover Image"
---

**Wardyati** is a shift management system I developed and launched to solve a real problem I experienced as an intern doctor: scheduling shifts fairly and efficiently. The platform currently serves thousands of intern doctors across university hospitals in Egypt.

## The Problem Wardyati Solves

At the beginning of my internship year, I personally experienced the recurring problems in shift scheduling:

- **Unfairness:** Using Google Forms and Google Sheets gives preference to those who respond faster, creating significant disparities among team members
- **Manipulation:** The ability to delete colleagues' names or modify their selections
- **Conflicts:** Booking overlapping shifts or exceeding allowed limits
- **Chaos:** Data loss and randomness in schedule organization
- **High Effort:** Spending hours trying to organize the schedule manually

I decided to find a radical solution to these problems, so I created a comprehensive vision for Wardyati and started working on it - a smart system that ensures fairness, transparency, and organization.

## Core Features

### Smart Booking System
- Display shifts in an organized calendar-like format with all details
- Allow booking only available shifts with clear explanations for unavailability
- Automatically prevent conflicts (overlapping shifts, exceeding limits, filled spots)

### Fairness and Transparency
- **Wait Time Between Bookings:** Prevent any member from booking multiple shifts consecutively, giving equal opportunities to everyone
- **Real-time Direct Booking:** All members enter together and book interactively with instant live updates
- **Timestamp Recording:** Order bookings by time to ensure transparency

### Flexible Management
- **Multiple Distribution Patterns:** Manual (specify count per member), equal (automatic distribution), or free (no maximum limit)
- **Coordination Control:** Open and close booking manually or with automatic time scheduling
- **Assignments:** Assign specific members to specific shifts

### Additional Features
- **Shift Swapping:** Send swap requests with messages and suggest alternative shifts
- **Shift Groups:** Link related shifts together (e.g., morning and evening of the same type)
- **Excel Export:** Export the complete schedule with one click instantly
- **Notifications:** Real-time notifications within the app and on browser for important events
- **Summary and Statistics:** Comprehensive view of room status and what's required from each member

## How Wardyati Works

1. **Team Coordinator** creates a room and invites members, sets shift times, required numbers, and rules
2. **Members** book shifts based on the rules, with the ability for direct group booking
3. **Real-time Updates** reach all members instantly with any booking or cancellation
4. **Smart System** prevents any conflicts and ensures an accurate, problem-free schedule

## Take a Tour

{{< youtube "8egpSJy-S9M" >}}

## Integrated Ecosystem

Wardyati is not just a shift scheduling system, but an integrated ecosystem that includes:

- **Complete Ad Platform:** Full platform serving advertisers targeting the medical field, with dashboard and precise performance tracking (impressions, clicks, CTR)
- **Testimonial Collection and Display System:** Automated mechanism to collect user experiences and display them professionally to build trust
- **Survey System:** To collect continuous feedback and improve the product based on actual user needs
- **Case Studies Publishing Platform:** To document success stories and share them with the community

## Development Journey and Challenges

I started working on Wardyati in March 2024 after directly experiencing the recurring problems in shift scheduling during the beginning of my internship.

I developed the project from scratch using **Django** as the core framework, with **HTMX** and **JavaScript** for the frontend, **PostgreSQL** as the database, **WebSockets** for real-time instant updates, **Redis** for in-memory caching, **Celery** as a task queue system for background tasks, and **Docker** for easy deployment on **Azure**.

The project launched in August 2024 and continues to be under active development and improvement, with me handling multiple responsibilities including technical development, server setup and maintenance, database management, and ensuring system stability and security.

### Key Technical Challenges

**Real-time Synchronization:** The biggest challenge was ensuring instant data synchronization among hundreds of users booking at the same time, while preventing any conflicts or race conditions. This was solved through advanced architecture combining WebSockets and precise database transaction management.

**Rate Limiting:** Building an advanced rate limiting system customizable per room, to prevent users from booking multiple shifts consecutively and ensure equal opportunity. This feature was crucial in achieving fairness among users.

**Conflict Prevention:** Building complex logic to prevent all possible types of conflicts before they occur (overlapping shifts, exceeding limits, etc.), while providing clear messages to users about why any shift is unavailable.

This project taught me a lot about the difference between building a demo project and building a real production system serving thousands of users monthly, where I gained experience in infrastructure management, handling real-time synchronization, and managing the product lifecycle from idea to continuous maintenance.

## Impact and Achievement

Since its launch, Wardyati has helped thousands of intern doctors in Egyptian university hospitals to:
- Save hours of time and effort in organizing shifts
- Eliminate conflicts and problems resulting from traditional methods
- Ensure fair and transparent shift distribution
- Dramatically improve the coordination experience

## User Testimonials

> "Wardyati changed my life! I've been using it for a year and a half for everything, from rooms with 4 members to rooms with 250. Instead of needing two full days to organize and create the schedule, I now need only 10 minutes. Now I can easily create the room and go to sleep knowing that 99% of things will go smoothly without my presence. Wardyati improves itself day after day and solves problem after problem. Truly, Wardyati saved tremendous effort and time and prevented many conflicts and disputes."
> 
> **— Dr. Omar, Intern Doctor - Al-Hussein University Hospital**
> [Read the full story](https://wardyati.com/stories/user/omar-ahmed-alazhar-success-story/)

> "It was a new and strange experience for most people, but overall the experience was very nice. One time I was traveling and the schedule was being made, and while I was on the road I was following until the schedule was complete in record time, less than half an hour, after scheduling used to be sacred to me and could take 24 or 48 hours. For me, this was a historic moment and the experience was very beautiful, and I can say that the transparency and clarity in Wardyati is 100%, one of the things that made me confident in the schedule it produces."
> 
> **— Dr. Ammar, Intern Doctor - Kasr Al-Ainy Hospitals**
> [Read the full story](https://wardyati.com/stories/user/ammar-shawky-kasr-alainy-success-story/)

> "Before Wardyati there were many problems; Google Sheets wouldn't open for everyone at the same time, and two people could choose the same shift, and someone could write their name instead of another, and the entire schedule could be deleted. Also, I couldn't set a specific number of shifts for each person, I had to follow them and see who took more and who took less, and many problems honestly. After Wardyati, most if not all of these problems were solved, and it's very easy for anyone to use, and there's fairness in shift distribution. I would recommend it to anyone 100%."
> 
> **— Dr. Hesham, Intern Doctor - Alexandria University Hospitals**
> [Read the full story](https://wardyati.com/stories/user/hesham-sabri-alexandria-success-story/)

*These testimonials are translated from Arabic.*

[View more user testimonials](https://wardyati.com/testimonials/user/)

## Project Links

- **Website:** [wardyati.com](https://wardyati.com)
- **User Guide:** [wardyati.com/how-to-use](https://wardyati.com/how-to-use/)
- **Telegram Community:** 
    - Channel: [t.me/wardyati_app](https://t.me/wardyati_app)
    - Group: [t.me/wardyati_chat](https://t.me/wardyati_chat)
