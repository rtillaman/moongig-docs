# Release 01.22.2026

## Jobs with Multi-profession

Jobs can now be configured to support multiple eligible professions instead of being limited to a single role.

**What’s New:**

* Allows selection of more than one profession for a job (e.g., Nurse, Nursing Associate, MedTech)
* Improves job visibility to all qualified healthcare professionals

This ensures roles that can be fulfilled by different but equally qualified professions are more accurately represented, reducing confusion and expanding the eligible talent pool.



<figure><img src=".gitbook/assets/Screenshot 2026-01-22 at 3.25.45 PM.png" alt=""><figcaption><p>Add Job Profession Field (Client Page)</p></figcaption></figure>

<figure><img src=".gitbook/assets/Screenshot 2026-01-22 at 3.26.47 PM (1).png" alt=""><figcaption><p>Job Card with Multi-Profession (Client Page)</p></figcaption></figure>

<figure><img src=".gitbook/assets/Screenshot 2026-01-22 at 3.28.29 PM.png" alt="" width="340"><figcaption><p>Job Card with Multi-Profession (Landing Page)</p></figcaption></figure>

## Profile Re-verification: Change Tracking

Updated fields of the HCPs are now clearly displayed in the Retool app under **Status Change History**. This allows Medops to easily track and verify specific changes the HCP has made.

## Automated Alerts: SMS and Fund Transfers

System alerts are now triggered for the following events:

* **Netbank** account balance is **below ₱50,000.**
* **Netbank** cannot process payments.
* **Netbank** returned a failed payment transaction.
* **TXTBOX** returned a **400 or 500** error from their API.

**New Email Templates**&#x20;

The following templates were added to support the new system alerts:

* **\[57] Alert Netbank Low Balance**
* **\[58] Alert Netbank Payout Error**
* **\[59] Alert SMS Error**

## Bug Fixes

**Compensation Display in Emails**

* **Issue**: In some "Nearby Shift" emails, the total compensation was not showing or was incorrect.
* **Fix**: The email logic has been corrected to ensure the full, accurate compensation amount is displayed.

**PRC ID Date Discrepancy**

* **Issue**: Saving a PRC ID previously resulted in an "off-by-one" date error.
* **Fix**: Added a date formatter to all PRC ID update functions. This prevents unformatted dates and ensures the timezone is strictly set to Asia/Manila (GMT+8).

**Report Extraction Timeout**

* **Issue**: Reports would get stuck in a loading state when processing large datasets due to a short 15-second timeout limit.
* **Fix**: Increased the timeout duration and added a visual progress bar to indicate the report is actively generating

**Views and Impressions**

* Views and Impressions are now available to Moongig users

<br>
