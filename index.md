# Pantri — Privacy Policy

**Last updated:** November 8, 2026

## Our approach

Pantri keeps your recipes, shopping lists, and pantry inventory on your device. We don't
sell your data, show ads, or track you across other apps or websites. There are no user
accounts and no sign-up. Data leaves your device in only three situations: when you import a
recipe or a shopping list (so an AI service can turn it into structured items), for limited
reliability diagnostics, and to verify an in-app purchase if you make one.

## Data stored on your device

Your recipes, shopping lists, pantry inventory, baskets, folders, and app settings are
stored **locally on your device**. We do not copy this to our servers and we do not sync it
across devices. Deleting the app removes this data.

## Data that leaves your device

### Recipe and shopping-list import (AI parsing)

When you import a recipe, or paste or import a shopping list for Pantri to organize, the
content you choose to import is sent through our secure relay to **OpenRouter**, which
routes it to the AI model that extracts the ingredients, items, and instructions. The
content sent is the import material itself — web page text, a video's caption or
description, text you type or paste, or text extracted from a photo — and only what is
needed for parsing. We do **not** include your name, contact details, or device
identifiers in these requests.

For **photo imports**, the text is extracted **on your device** using your phone's built-in
text-recognition capability. The photo itself is never sent to us or to any third party —
only the extracted text enters the import process above.

### Fetching public source pages

When you import from a link, the app fetches the public page — a recipe website, or public
metadata from services like YouTube, TikTok, or Instagram — the same way a web browser
would, to obtain the recipe content.

## Anonymous identity

To run the AI relay and diagnostics securely, the app creates an **anonymous identifier**
managed by our backend provider (Supabase). It is **not** linked to your name, email, or any
account. It exists so requests can be authenticated and rate-limited.

## Diagnostics

To keep the app reliable, we collect **limited, non-personal** diagnostics. They carry a
random install identifier (not your Apple or Google account, and not an advertising ID)
and are associated with the anonymous identifier above:

- **Usage events** — for example, which type of import source was used, simple counts,
  timings, and categories of errors, along with the app version, operating system version,
  and platform. When you import from a link, the **URL of the page you import** is
  recorded in our service logs so we can diagnose failed imports. These events do **not**
  include your recipes, your lists, or the text you import.
- **Crash reports** — a sanitized record of the type of error and where in the app's code it
  occurred, including crash diagnostics provided by iOS. These are stripped of your recipes,
  imported content, URLs, and any credentials.

We use this only to fix bugs and improve reliability. We do **not** use it for advertising
or for tracking you across other apps or websites.

## In-app purchases

Payments are handled entirely by Apple or Google; we never see your payment details. If you
make a purchase, we receive the transaction information needed to verify it and unlock the
feature, associated with the anonymous identifier above.

## Notifications

Import-complete notifications are scheduled locally on your device. We do not use push
notification tokens.

## Third parties we use

- **Supabase** — our backend. It manages the anonymous identity, relays parsing requests,
  verifies purchases, and stores the diagnostics described above.
- **OpenRouter** and the AI model providers it routes to — process the content you import
  in order to return the parsed result. We may change the specific underlying model over
  time; the categories of data sent do not change.
- **Apple / Google on-device text recognition** — used for photo import. Runs on your
  device; images are not sent to us or a third party.

We do not use advertising SDKs, and we do not sell or share your data with data brokers.

## Data retention and deletion

- **On-device data** (recipes, lists, pantry): stays on your device and is removed when you
  delete the app.
- **Server-side data** is deleted automatically: usage events after 180 days, crash and
  error reports after 365 days, and import and AI-usage logs (including imported URLs)
  after 400 days.
- **Delete it yourself, any time:** **Settings → Delete all Pantri data** permanently
  deletes every server record tied to your anonymous identifier, including the identifier
  itself, and clears all Pantri data on your device. You can also request deletion at
  **dev@justgoup.app**.

## Children

Pantri is not directed to children and does not knowingly collect personal information from
children.

## Changes to this policy

If we change how the app handles data, we will update this policy and its "last updated"
date.

## Contact

Questions or deletion requests: **dev@justgoup.app**
