# Release 12.11.2025

## Profile Badge

We’ve updated the Profile Type system to create a clearer, more consistent progression for Professionals, ensuring both HCPs and MedOps teams have full visibility into verification status, required documents, and application eligibility.

### **What’s New**

### **Streamlined Profile Progression**

The profile journey has been restructured into a transparent, standardized flow:\
**New → Basic → Basic (Under Review) → Basic (Verified) → Professional (Under Review) → Professional (Verified)**.\
This progression dynamically updates based on requirements completed and MedOps review actions.

**Clearer Rules Per Profile Type**

Each profile state now reflects what the Professional can access and what actions are required:

* **New Profile**
  * Triggered when an HCP skips CV extraction (“I’ll do it on my own”).
  * Cannot apply for jobs.
  * Guided to complete Basic Profile requirements.
* **Basic Profile**
  * Granted when an HCP completes all **8/8 basic requirements**.
  * Can apply for jobs unless a specific posting requires an additional document.
  * Missing required docs display contextual warnings.
* **Basic (Under Review)**
  * Triggered once supporting documents are uploaded.
  * Can apply for jobs; lower match score since not yet verified.
  * MedOps can approve verification in Retool.
* **Basic (Verified)**
  * Granted once MedOps sets status to `BASIC_PROFILE_VERIFIED`.
  * If a verified doc expires, automatically downgrades to Basic (Under Review).
* **Professional (Under Review)**
  * Triggered when all 12/12 requirements are completed.
  * Eligible for all jobs/shifts.
  * Awaiting MedOps verification in Retool.
* **Professional (Verified)**
  * Final and highest status.
  * Auto-downgrades to Professional (Under Review) if a required doc expires.

![](<.gitbook/assets/image (20).png>)&#x20;

![](<.gitbook/assets/image (21).png>)  ![](<.gitbook/assets/image (25).png>)

<div align="left"><figure><img src=".gitbook/assets/image (23).png" alt="" width="316"><figcaption></figcaption></figure> <figure><img src=".gitbook/assets/image (1).webp" alt="" width="311"><figcaption></figcaption></figure></div>

<figure><img src=".gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

## Shift Reset Workaround

We’ve implemented a more transparent and applicant-friendly system to address the issues caused by “stale” shifts and their reset behavior.

### **What’s New**

### **Reset Behavior Fix**

Shifts that undergo a reset (due to updated rates, aging listings, or low engagement) previously removed all applicants without notifying them.\
We’ve introduced a notification workflow to ensure HCPs are properly informed and encouraged to reapply if still interested.

**Automatic Applicant Notifications**

When a shift is reset:

* All existing applications are cleared
* Once the shift reopens, HCPs receive both an email and SMS informing them that:
* Their prior application was reset
* They may reapply if still available\
  This resolves confusion for HCPs who may have applied weeks earlier and were unaware of the reset.

**Proactive Outreach to Nearby Users**

In addition to notifying previous applicants:

* The system also alerts nearby HCPs who haven’t applied yet
* This boosts visibility and helps refill resets quickly

**Improved Shift Freshness**

Resetting helps Providers:

* Refresh outdated postings
* Account for HCP schedule changes over time
* Improve the chances of matching with currently available Professionals

<div align="left"><figure><img src=".gitbook/assets/image (26).png" alt="" width="360"><figcaption></figcaption></figure> <figure><img src=".gitbook/assets/image (2).webp" alt="" width="263"><figcaption></figcaption></figure></div>

## Pinned Shifts and Jobs

We’ve added a visibility and prioritization mechanism for key opportunities. High-priority Shifts and Jobs are now “Featured” and automatically elevated to the top of the Professional feed based on backend logic.

### What’s New

### **Featured Opportunities**

**Pinned items now:**

* Appear at the top of the Home Page feed
* Display a Featured badge for distinction
* Include Local, Overseas, Jobs, and Shifts
* Are visible on both the Mobile App and Landing Page

Pinned logic is backend-defined and hardcoded—MedOps cannot manually toggle pins.

**Context-Aware Ranking**

Pinned items respect the Professional’s selected tags on the Home Page:

* **Nearby Selected**
  * Overseas items: Always shown
  * Local items: Shown only if matching the user’s region
* **Profession Selected**
  * Displays pinned items relevant to the user’s profession
* **No Tags Selected**
  * Shows all pinned items by default

**Three-Tiered Priority Sorting**

Pinned items follow a backend-defined hierarchy:

1. Urgent or high-importance Shifts/Jobs
2. Critically under-viewed items (low exposure)
3. Regular pinned items

This ensures that the most time-sensitive or struggling posts gain visibility first.

**Search Page Integrity**

Pinned items do not override sorting on the Search page.\
Search remains unbiased, filter-driven, and does not show pinned items at the top.

**No Provider-Side Changes**

Providers do not need to (and cannot) manage pins.\
This system is purely backend-driven.

<figure><img src=".gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

<div align="left"><figure><img src=".gitbook/assets/image (29).png" alt="" width="375"><figcaption></figcaption></figure> <figure><img src=".gitbook/assets/image (2) (1).png" alt="" width="375"><figcaption></figcaption></figure></div>

&#x20;

## &#x20;Bug Fixes

* Required Fields For Medgrocer during Shift Creation
