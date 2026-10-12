# HiQuest changelog

What changed on [hiquest.fit](https://hiquest.fit), newest first. HiQuest ships
continuously, so entries are grouped by month instead of by version number.

Each month has up to three groups: **New** for things you can now do,
**Improved** for things that work better, and **Fixed** for things that were
broken. **Behind the scenes** covers changes you won't see directly but that
affect what reaches the site.

---

## October 2026

### New
- **Sort events by date.** The events list can show the soonest or the furthest
  trips first.

### Improved
- **Faster, more accurate event intake.** Persian dates in organisers' posts are
  now read by deterministic rules, not guessed by an AI model. That covers
  hashtag dates such as `جمعه_۲۸_آذر`, date ranges that span two months, and
  dates followed by a Persian comma. Fewer trips get published with the wrong
  day or year.
- **Province pages** now render their events on the server, so they load
  faster and search engines can read them. Khorasan provinces now match
  correctly.
- **Organiser pages** each have a single canonical address, so search engines
  stop treating one organiser as several duplicate pages.

### Behind the scenes
- Editors have a new review queue for posts collected from public outdoor
  channels. They can keep, drop, archive, or import a post into the event form.
- The AI-assisted import can run on locally hosted models as well as hosted
  ones. Editors can see and adjust the instructions it was given, and they
  check every result before it is published.

## September 2026

### New
- **Open data: the Iranian outdoor-events market.**
  [hiquest.fit/data/outdoor-events-iran](https://hiquest.fit/data/outdoor-events-iran)
  covers supply by month, prices in real terms, terrain, calendar,
  destinations, elevation, weather and air quality, along with the claims the
  data can't support.
- **Citable dataset, v1.** The same data is archived with DOI
  [10.5281/zenodo.22734999](https://doi.org/10.5281/zenodo.22734999), under
  CC BY 4.0 with an ODbL 1.0 table of destinations.
- **Personality results, redesigned.** You now get an animated radar of your
  outdoor archetype, clickable activity suggestions, gear scored against your
  archetype, and real "people like you" matches.
- **Shareable personality card** with correct Persian text rendering.
- **"Create an event" landing page.** Organisers who aren't signed in now see
  what HiQuest offers them instead of being sent straight to sign-in.

### Improved
- **Every page is fully server-rendered.** Content arrives in the first
  response instead of after JavaScript runs, so pages show up sooner and
  search engines index them better.
- **Pages that don't exist return a real "not found"** instead of an empty page.
- **Sign-in and sign-up screens** redesigned.
- **Rich results in search.** Event, breadcrumb and featured-listing markup was
  corrected so search engines can show trip details.

### Fixed
- The header and footer appeared twice on some "not found" pages.

### Behind the scenes
- **Security hardening.** Requests are rate-limited, repeated failed logins
  trigger a lockout, and form input is validated.
- The organiser analytics dashboard loads from pre-computed totals and is
  much faster on large accounts.
- Sign-in, admin and registration-flow pages are excluded from search results.

## July 2026

### Improved
- Guests can take the personality quiz and keep their result when they sign up.
- Better date filtering on event lists.

## June 2026

### Improved
- **Much faster event pages.** Event pages are pre-rendered and cached, and
  the main image loads first.
- Better accessibility scores: colour contrast, a gentler notification
  prompt, and a fallback page description everywhere.
- Event data is cached for faster browsing.

## May 2026

### New
- **Featured listings.** Organisers can pay to put a trip at the top of search
  results, with a featured badge, for a set period. Payments go through
  Zarinpal.
- **Blog** for guides and stories.
- **Organiser landing page and SEO guide** to help organisers get their trips
  found.
- **Connect Bale and Rubika.** Organisers can verify their Bale and Rubika
  accounts and link them to their HiQuest page.
- **Personality quiz v2** with a chart of your result, which is also shown on
  your public profile.
- **Organisers' own analytics**, with views and activity per trip, now
  mobile-friendly.
- **Pages for each province × activity** combination, such as hiking in a given
  province.

### Improved
- **Better installable app**: a native splash screen and a smoother install
  prompt.
- **The event creation form** got a cleaner layout and a better AI fill-in from
  a pasted post.
- Related events are matched more cleverly when an event has few direct
  matches.

## April 2026

### New
- **Outdoor personality quiz** at [/personality](https://hiquest.fit/personality).
  Answer the questions, get your archetype, and see matching categories and
  events. You can add it to your profile.
- **Cinema camp** category.
- **"All events" pages** for every category.

### Improved
- Choosing an organiser is easier on the event form.
- Related events appear sooner on a trip that has already happened.
- New Persian font and a round of interface and translation fixes.

## March 2026

### Improved
- Organiser blocks on the homepage, and a cleaner organiser page.
- A "become an organiser" banner in the navigation.
- Long links in event descriptions no longer break the layout.

## February 2026

### New
- **Accounts.** You can sign up, including with Google, to comment on events
  and request to join them.
- **Organiser panel** for organisations to manage their own events.
- **Persian/English language switch** in the header.
- **Jalali date picker** that switches to the Gregorian calendar in English mode.

### Improved
- The event creation form was regrouped into clear sections.
- More complete sitemaps for search engines.

### Fixed
- Date filters sometimes compared dates incorrectly.

## December 2025

### Improved
- Separate sitemaps for events, categories and organisers.
- Event thumbnails are used for link previews, with terrain-specific fallback
  banners.
- Updated gear-list format on event pages.

## November 2025

### New
- **About page.**
- **Blog**, managed from the admin panel.
- **Organiser verification** and a richer organiser management workflow.

### Improved
- Category pages got descriptions, Persian labels for every filter and
  sub-category, and proper metadata.
- Event pages and event cards can be shown in English.
- "Create event" moved under Events.

## October 2025

### New
- **Installable app (PWA) with push notifications.**
- **Publish, edit and delete events** from the website, in Persian or English.
- **Verified badge** on events that the team has checked.

### Improved
- The event page header was reorganised, and the event card buttons were tidied.
- Gear suggestions load faster.

### Fixed
- Wrong dates on events published from the website.

## August 2025

### New
- **Add to calendar** on event pages.
- A gear list with images directly in the event's main tab.

## July 2025

### New
- **Blog.**
- **Gear suggestions** for each trip, with links to buy.
- **Newsletter** signup by email.
- Category and organiser index pages.

### Improved
- Event lists load a short date range first and fetch more as you scroll.

## June 2025

### New
- **Category pages** and **organiser pages**, linked from every event.

### Improved
- Event pages are cached and revalidated, so they load faster.

## May 2025 — launch

- **HiQuest goes live at hiquest.fit**, with events listed from organisers'
  announcements, filters by date, and event pages with a map, cost and
  organiser.
- Related events, a sitemap, newsletter signup, and event details for search
  engines.
