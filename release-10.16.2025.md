# Release 10.16.2025

## Shift Changes

### Emergency Funds & Allowance

We’ve added **two new fields** under the **Compensation** section during shift creation:

* **Emergency Funds**
* **Allowance**

<figure><img src=".gitbook/assets/Screenshot 2025-10-15 at 5.05.31 PM (1).png" alt=""><figcaption><p>Shift Creation with Emergency Funds &#x26; Allowance</p></figcaption></figure>

<figure><img src=".gitbook/assets/Screenshot 2025-10-15 at 5.10.36 PM.png" alt=""><figcaption><p>Shift Summary (Shift Creation)</p></figcaption></figure>



During **shift application review**, **Emergency Funds** and **Allowance** are **always visible**, but can **only be edited if the shift has not been paid**.

<div align="center"><figure><img src=".gitbook/assets/Screenshot 2025-10-15 at 5.12.43 PM.png" alt="" width="511"><figcaption><p>Shift Review with Emergency Funds &#x26; Allowance</p></figcaption></figure></div>



* Once paid, the values will be displayed on the **HCP’s side** as follows:
  * **Emergency Funds** under _Priority Surcharge_
  * **Allowance** under _Allowances_
* **HCPs** can view these values in:
  * The **“What is Included”** modal
  * The **Payout Breakdown** page
  * The **Payslip**

<div><figure><img src=".gitbook/assets/Screenshot 2025-10-15 at 5.19.44 PM (1).png" alt=""><figcaption><p>What is included - Modal</p></figcaption></figure> <figure><img src=".gitbook/assets/Screenshot 2025-10-15 at 5.21.36 PM.png" alt=""><figcaption><p>Payout breakdown page</p></figcaption></figure></div>

 

<figure><img src=".gitbook/assets/Screenshot 2025-10-15 at 5.18.26 PM.png" alt="" width="375"><figcaption><p>Payslip</p></figcaption></figure>



## Job Changes

### Phone Interview Option

* You can now select **Mobile** as a communication channel when scheduling an interview.
* When **Mobile** is selected, you’ll be prompted to enter the **interviewer’s name** and **phone number**.
* **Note:** Phone interview option is only available for manual scheduling.
* An **email notification** will be sent to the HCP, including the interviewer’s name and phone number.

<figure><img src=".gitbook/assets/phone.png" alt="" width="524"><figcaption><p>Schedule Interview - Phone Interview Option</p></figcaption></figure>

<figure><img src=".gitbook/assets/phone email.png" alt=""><figcaption><p>Phone Interview - Email</p></figcaption></figure>

### Scheduled Interview List

We’ve added a new page for **Providers and Recruiters** to view a **consolidated list of scheduled interviews**, along with their current status (_Scheduled, Confirmed, Cancelled,_ or _Completed)._

**Key Features:**

* Accessible by selecting an **Interview State card** (e.g., _For Interview, 2nd Interview, 3rd Interview_) and clicking **View Interviews** at the top-right of the screen.
* Each Interview State has its own **View Interviews** button.
* The list displays:
  * Candidate name
  * Role applied for
  * Interview date & time
  * Mode (e.g. In-Person, Online)
  * Current status
* Recruiters can **filter interviews** by status (_Scheduled, Confirmed, Cancelled, Completed_).
* When an interview is **rescheduled**, the list automatically updates to show the latest time.
* Recruiters can **manually update** an interview’s state (Confirmed, Cancelled, or Completed) using the **action button** beside the candidate’s row.

**Status Definitions:**

* **Scheduled** – Interview has been scheduled but not yet confirmed by the applicant.
* **Confirmed** – Applicant has confirmed their attendance in the app.
* **Completed** – Interview has been conducted.
* **Cancelled** – Interview was cancelled by either the applicant or the provider.

<figure><img src=".gitbook/assets/Screenshot 2025-10-15 at 5.42.43 PM (1).png" alt=""><figcaption><p>Job details Page with View Interviews button</p></figcaption></figure>



<figure><img src=".gitbook/assets/Screenshot 2025-10-15 at 5.42.31 PM.png" alt=""><figcaption><p>Scheduled Interview List</p></figcaption></figure>



### For Interview Section UI Changes

We’ve updated the **HCP view under Jobs** to better highlight job applications that are **scheduled for interview**. This will make it easier for HCPs to identify and track their interview-related applications.

<figure><img src=".gitbook/assets/for interview.png" alt="" width="245"><figcaption><p>For Interview Section Update</p></figcaption></figure>

\


### Past shifts and job applications

We’ve added a new feature that allows **Providers and Recruiters** to view an applicant’s **past shift/job application history** with their company.

For each applicant, recruiters can see:

* Count of past completed shifts with the provider.
* Other job applications submitted to this provider.
* Each application’s **current status, applied date**, and **last updated date.**

This update helps recruiters make more informed hiring decisions by providing better context on an applicant’s previous interactions with their company.

<figure><img src=".gitbook/assets/Screenshot 2025-10-15 at 6.03.52 PM.png" alt=""><figcaption><p>Job applicant history</p></figcaption></figure>

<figure><img src=".gitbook/assets/498774946-ac9b1a8f-018a-41bd-8066-114da4003547.png" alt="" width="375"><figcaption><p>Other Job Applications with you</p></figcaption></figure>



## Bug Fixes & Improvements

### Viewed State

We’ve fixed an issue where the **viewed state** of applicants was **shared across all provider accounts**.\
The **viewed state is now tracked separately per provider account**, ensuring that when one account views an applicant, it will not appear as viewed for others.

### Shared Shift Link Access

* Fixed an issue where **logged-out users** who clicked **“View Shift Details”** from an the **"New Nearby Shift"** email were redirected to a **loading or empty screen**.
* The shared shift link now loads **properly for all users**, even when not logged in.

### Export confirmation popup

We’ve added a **confirmation popup** when exporting applicant data. Users will now be prompted to **confirm the export action** to ensure they intend to proceed before the data is exported.

<figure><img src=".gitbook/assets/Screenshot 2025-10-15 at 6.08.42 PM.png" alt=""><figcaption><p>Job Action Dropdown</p></figcaption></figure>

<figure><img src=".gitbook/assets/export-conf-modal.png" alt=""><figcaption><p>Export Confirmation Popup</p></figcaption></figure>

