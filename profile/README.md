<div align="center">

# HiQuest

**Find your next hike, climb, camp or walk in Iran — and the people going.**

<p dir="rtl">جایی برای عاشقان طبیعت، حرکت و کشف تا همدیگر را بیابند و تجربه‌ها را به‌اشتراک بگذارند.</p>

[hiquest.fit](https://hiquest.fit) · [Open data](https://hiquest.fit/data/outdoor-events-iran) · [Changelog](https://github.com/HiQ-Lifestyle/.github/blob/main/CHANGELOG.md) · [Telegram](https://t.me/hiquest_fit) · [Instagram](https://instagram.com/hiquest.fit) · [X](https://x.com/hiquest_fit)

</div>

---

HiQuest is a Persian-language platform for outdoor and active events in Iran.
Mountain clubs, hiking groups and tour leaders announce hundreds of trips a
month, mostly as posts scattered across messaging channels. HiQuest gathers
them into one place where you can search by date, province and activity, see
what a trip involves, and find who is organising it.

## For people looking for a trip

- **Browse events** by category (hiking, mountaineering, camping, cinema camp,
  walking groups and more), by province, or by date.
- **Event pages** with the meetup point on a map, difficulty, cost, the
  organiser, a gear checklist, and related trips when one has passed.
- **Outdoor personality quiz** at [hiquest.fit/personality](https://hiquest.fit/personality):
  find your archetype, then get matching activities, gear and people like you.
- **Profiles** to sign up, comment, and request to join an event.
- **Installable app** (PWA) with notifications, in Persian or English.

## For organisers

- **A public organiser page** listing every trip you run, with a verified badge.
- **Publish an event in minutes**: paste your channel post and the form fills
  itself in for you to check.
- **Featured listings** that put a trip at the top of search results, with a
  featured badge, for a set period.
- **Your own analytics**: how many people saw each trip and what they did next.

Start at [hiquest.fit/events/create-event](https://hiquest.fit/events/create-event).

## Open data

We publish what the platform has learned about the outdoor-events market in
Iran, both as a page anyone can read and as a citable dataset.

- **Market page** at [hiquest.fit/data/outdoor-events-iran](https://hiquest.fit/data/outdoor-events-iran):
  supply by month, prices in real terms, terrain, calendar, destinations,
  elevation, weather and air quality. It also lists what the data *can't* tell you.
- **Dataset**: *Iranian outdoor events*, 1,115 events published May 2025 –
  October 2026. The page refreshes weekly; the archived dataset is versioned.
  DOI [10.5281/zenodo.22734999](https://doi.org/10.5281/zenodo.22734999).
  Licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). The
  OpenStreetMap-derived destinations table is under
  [ODbL 1.0](https://opendatacommons.org/licenses/odbl/1-0/).

The public data carries no organiser names, and any destination that turns
out to be an organiser's own premises is withheld rather than put on a map.

## How it's built

| Part | What it does |
|---|---|
| Web app | Next.js 16 and React, PostgreSQL through Drizzle, Redis cache. Server-rendered and Persian-first, with a Jalali calendar throughout. |
| Event intake | Collects posts from public outdoor channels, reads Persian dates with deterministic rules, and passes them to an AI-assisted import that an editor reviews before anything is published. |
| Data pipeline | Python. Takes a weekly read-only snapshot, checks it against a data contract, adds weather, elevation, air quality and inflation-adjusted prices, and builds the public dataset. |

Our source repositories are private. What changes for users is in the
[changelog](https://github.com/HiQ-Lifestyle/.github/blob/main/CHANGELOG.md).

## Get in touch

- Organisers and partners: [hiquest.fit/contact](https://hiquest.fit/contact)
- News and new trips: [Telegram @hiquest_fit](https://t.me/hiquest_fit) ·
  [Instagram @hiquest.fit](https://instagram.com/hiquest.fit) ·
  [X @hiquest_fit](https://x.com/hiquest_fit)
- Using the dataset in research? Please cite the DOI. We'd like to hear what you build.
