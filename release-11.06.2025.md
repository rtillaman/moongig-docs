# Release 11.06.2025

## Sort Ads: Sort job ads by salary range

As part of improving job ad discoverability and transparency for healthcare professionals, we've introduced a new sorting feature that allows users to organize job ads based on salary range.

**What’s Changed**

Users can now **sort jobs and shift ads by salary**, from **highest to lowest or lowest to highest**, allowing them to explore opportunities that best fit their compensation preferences.

![](<.gitbook/assets/unknown (3).png>)![](<.gitbook/assets/unknown (1) (1).png>)

## Shift Management: Update and delete draft shifts and posts

To give companies greater flexibility when managing job and shift postings, we’ve added the ability to **edit and delete draft shifts or posts** directly within the platform.

**What’s Changed**

Users can now:

* **Save draft shifts or job posts** without publishing immediately.
* **Delete draft posts** that are no longer needed, only enabled if no applicants are present, helping keep the list organized and up to date.



<p align="center"><img src=".gitbook/assets/unknown (2) (1).png" alt=""></p>

## New Email Templates

To help healthcare professionals stay informed and connected, we’ve launched new **email templates** designed to improve communication and ensure timely updates.

**What’s Changed:**

*   **Enable Notifications:**

    A new template encourages users to t**urn on Shift and Job Notifications**, guiding them step-by-step on how to stay updated via **SMS or Emai**l for new job or shift opportunities.

<p align="center"><img src=".gitbook/assets/unknown (3) (1).png" alt=""></p>

\


*   **Earthquake Evacuation Reminder:**

    Added emergency evacuation guidelines (e.g., for earthquakes or fires) to help ensure on-site preparedness and safety

<p align="center"><img src=".gitbook/assets/unknown (4).png" alt=""><img src=".gitbook/assets/unknown (5).png" alt=""></p>



## Bug Fixes & Minor Enhancements

* Fixed an issue where clients were unable to create a job when manually entering a job location.
* Updated job creation settings so that when a client creates a new job, the **CV requirement is now enabled by default**, ensuring applicants must upload their CVs before applying.
* Added new shift type for medgrocer when creating a shift:&#x20;
  * Medgrocer Events&#x20;
  * TH Training
* Fixed incorrect interview state colors to ensure consistency across the client and app:
  * Declined – Red
  * Cancelled – Grey
  * Accepted / Completed – Green
  * Scheduled / Pending – Orange
* Fixed an issue where the **“Select ID” dropdown in the Add Government ID** modal scrolled outside the modal when the background page was scrolled. The dropdown now remains fixed within the modal while scrolling.
* Fixed an issue where **two identical “Save” buttons** appeared in the Bank Details section of the profile page. Only one functional “Save” button is now displayed
* Fixed an issue where **users were able to create an account without uploading the required documents or a profile picture**. Account creation now correctly enforces these requirements before completion.
* Fixed empty meeting link on “Scheduled Interview” emails
* Fixed an issue where the E-wallet and Bank Account dropdowns under the Bank Details section showed no selectable options during profile creation. Both dropdowns now properly display available options such as GCash, Maya, BPI, and BDO.

[**Landing Page Bug Fixes:**](#user-content-fn-1)[^1]

* Fixed an issue where clicking the Moongig logo on the **“Looking to Hire?”** page did not redirect users back to the landing page. The logo now correctly navigates to the Moongig Landing Page.
* Fixed an issue where **job listings disappeared from the landing page after removing a selected job filter**. Job listings now properly reset and display all available jobs when filters are cleared.
* Fixed an issue where the **filter count displayed inaccurately and overlapped when multiple filters were applied**. All applied filters now remain visible and correctly reflected in the counter.
* Fixed an issue where the **navigation bar partially overlapped the “Filtered Jobs”** text when navigating to the Jobs page from the Featured Jobs section on an iPad 10th Gen. The text now displays properly across all devices.
* Fixed an issue where the **“No Matches Found”** message persisted after **clearing an invalid search input** on the landing page filter. The message now disappears once the input is removed and relevant results are shown.
* Fixed an issue where loading skeletons briefly appeared when switching between the “Within 48hrs” and “Within 7 Days” tabs in the Latest Shifts section. Transitions now display smoothly without interruptions.

\
\


[^1]: 
