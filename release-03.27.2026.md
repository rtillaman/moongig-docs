# Release 03.27.2026

## Talent Search V2

We’re introducing Talent Search V2, a major upgrade that enables providers to proactively discover and invite healthcare professionals directly from Moongig’s verified talent pool.

This release focuses on fixing critical issues from V1, improving search accuracy, and delivering a more reliable, structured sourcing workflow.

<figure><img src=".gitbook/assets/Screenshot 2026-03-27 at 9.57.59 AM.png" alt=""><figcaption></figcaption></figure>

**What’s New**

**Smarter Search Experience**

* Search now triggers only **on Enter or button click** (no more auto-search interruptions)
* Natural language queries are parsed into **read-only criteria chips**
* Added support for **Boolean OR logic** (e.g., “Nurse OR Technician”)
* Improved NLP parsing for:
  * Clinical abbreviations (ICU, ER, NICU, etc.)
  * Age constraints (min, max, range)

**Accurate Match Scoring**

* Fixed issue where **0-match candidates showed incorrect scores**
* Match scores now strictly follow a **weighted scoring model**
* Profiles with **0 matching criteria are excluded entirely**
* Added:
  * **Color-coded match score**s (high / medium / low)
  * “**Gaps vs your search” indicators**
  * Always-visible match criteria (no hover required)

**Improved Candidate Cards**

* Key details are now always visible:
  * Profession, specialization, location, experience, certifications
* Dynamic fields appear based on your query (e.g., age, gender)
* Added:
  * Inline match badges
  * Feedback actions (👍 / 👎)
* Privacy-first display:
  * Masked profiles until candidate applies

**Privacy-First Candidate Profiles**

* Candidate identities remain **partially hidden until application**
* Clicking a masked profile shows a **clear “Invite to unlock” modal**
* Full profile access is granted only after:
  * Candidate applies, or
  * Prior consent exists

**Streamlined Invite Workflow**

* Invite candidates directly from search results
* Supports:
  * **Single and bulk invites (up to 20 candidates)**
  * Job post selection (required before sending)
* Built-in safeguards:
  * Duplicate invite prevention
  * Profession mismatch validation
* Success feedback via real-time toasts

<figure><img src=".gitbook/assets/Screenshot 2026-03-27 at 10.00.20 AM (1).png" alt=""><figcaption></figcaption></figure>



**Key Fixes from V1**

* ❌ Auto-search on keystroke → ✅ Explicit trigger only
* ❌ Inverted age filter → ✅ Correct min/max parsing
* ❌ Incorrect match scores → ✅ Accurate scoring logic
* ❌ Hidden match criteria → ✅ Always visible
* ❌ Broken breadcrumbs → ✅ Correct navigation
* ❌ Stacking modals → ✅ Singleton modal behavior

<br>
