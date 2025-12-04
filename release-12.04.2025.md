# Release 12.04.2025

## Customize ATS States

We’ve enhanced ATS flexibility for Providers by allowing them to customize their applicant pipeline while keeping data integrity intact.



#### **What’s New**

* Custom ATS States\
  Providers can now create their own ATS columns (e.g., Pre-Employment Exam, Background Check) to tailor workflows based on their hiring process.
* Hide Unneeded States\
  Pre-defined ATS states (except Applied and Archived) can now be hidden—as long as they are empty. This helps Providers remove clutter and simplify their pipeline.
* State Occupancy Validation\
  A state cannot be hidden, edited, or deleted if it currently contains applicants. The system will display a warning indicating how many applicants need to be moved before the action can proceed.

#### State Management Interface

A new Manage States panel is now accessible from the Applicants view. Providers can:

* Add custom states
* Hide/show states
* Edit and delete custom states (only when empty)
* See which states are Active vs. Hidden

#### Key Behaviors

* Visibility Control: Hidden states immediately disappear from the ATS board and status dropdowns.
* Reactivation: Hidden states can be set to visible anytime from the Manage States panel.
* Data Integrity: Any action that impacts a state with existing applicants is disabled to avoid data inconsistencies.

<div align="center" data-with-frame="true"><figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure></div>



## ATS Toasts

We’ve improved the feedback and communication flow in the ATS pipeline by introducing contextual toast notifications that reflect whether an email was sent to the applicant after a recruiter action.



#### **What’s New**

#### **Action-Based Email Sending**

* Certain recruiter actions now automatically trigger emails to applicants (e.g., moving an applicant to For Interview, Offered, Hired, Not Qualified, Rejected).
* Actions that do not send emails (e.g., Shortlisted, For Pooling, No Show, No Response, Declined Offer) can be undone

#### **Toast Notifications**

* Recruiters now receive a real-time toast notification after every pipeline action, indicating:
* The action taken
* Whether an email was sent
* The applicant affected
* Email-sent notifications appear in green (success) or red (error) depending on the status/action.
* Actions without email sending display informational toasts with an option to undo the action.

#### **Undo Logic**

* If no email is sent, recruiters can undo the action directly from the toast.
* Actions that automatically trigger emails cannot be undone via the toast to prevent inconsistent communication with applicants.

#### Benefits

* Provides immediate feedback to recruiters on the result of their actions.
* Reduces mistakes or miscommunication with applicants.
* Helps recruiters understand which actions are reversible and which are final.

<div data-with-frame="true"><figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure></div>



<div data-with-frame="true"><figure><img src=".gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src=".gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure></div>

## Updated Reimbursement Template

We’ve refreshed the Shift Payout Report to improve clarity, standardization, and compatibility with internal and MedGrocer workflows. The update introduces clearer identifiers, cleaned-up formatting, and streamlined columns.



#### **What’s New**

#### **Additional Columns**

* Billing Code (Moongig) (Billing Code for all other providers)
* Shift Code (Medg – Airtable) (visible only for MedGrocer)
* Base PF Per Hour
* Base PF
* Emergency Funds
* Final Gross PF

#### Renamed Columns

* Shift Code → Shift Code (Moongig Generated) (Shift Code for other providers)
* Reliever Role → Role
* TIN Number → TIN
* Med Ops Team Remarks → Med Ops Remarks
* Review Remarks → Shift Review Remarks
* Time-In/Time-Out → Time In/Time Out\
  Late / Undertime Deduction → Late/Undertime Deductions
* Taxes withheld → Taxes Withheld
* Net Disbursed PF → Final Net Disbursed PF

#### Date/Time Formatting Improvements

* Shift Start Date now uses: DD-MMM-YYYY
* Shift Creation Date/Time & Reliever Confirmation Date/Time now use:\
  MMM DD, YYYY h:mm A\
  (with a tab prefix to prevent Excel auto-formatting)

#### Removed Columns

* Shift End Date
* Sworn Declaration
* Shift Base Comp
* Priority Surcharge
* Allowances
* Total Base PF
* Gross PF
* Status

#### MedOps-Only / Manual Fields (exported as blank)

* Leave Confirmation Date/Time
* Matrix Rate Version

## Flagging of Expired Documents

We’ve introduced an automated document expiry system to help ensure that HCPs maintain valid credentials and that Providers always see accurate, up-to-date verification information.

#### What’s New

#### **Automated Expiry Detection**

* The system now checks all uploaded documents daily (and on login).
* Any document past its Expiry Date is automatically marked as Expired.

#### **Clear Expiry Indicators (HCP View)**

* Expired documents now display a prominent Expired tag on the HCP’s Documents page.
* A “Missing/Expired Document” warning appears with the specific document name to prompt updates.

<div data-with-frame="true"><figure><img src=".gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure></div>

<div data-full-width="true" data-with-frame="true"><figure><img src=".gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure></div>

#### Notifications to HCPs

* 30 Days Before Expiry: Automated email + in-app reminder to renew the document.
* On Expiry: Automated email + in-app alert informing them that their verification is now invalid until the document is updated.

<div data-with-frame="true"><figure><img src=".gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src=".gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure></div>

#### Verification & Application Restrictions

* If a critical document expires (e.g., only PRC License), the HCP’s profile is automatically downgraded to Unverified.
* A warning icon “(!)” is shown on the HCP sides.\
  The HCP is blocked from applying for Shifts and Jobs until they upload a valid document and regain Verified status.



## Job/Shift Card Analytics: Unique User Views

We’ve added a new engagement metric that helps Providers understand how much interest their Job or Shift postings are generating. This is now visible directly on job cards and detailed views.

#### What’s New

Unique View Counter (Provider-Only)

* A new “Eye” icon + views indicator now appears on:
* The footer of each Job/Shift card
* The Job/Shift Details page
* Only Providers (job owners) and Moongig Admins can see this metric. HCPs cannot.

<div data-with-frame="true"><figure><img src=".gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure></div>

<div data-with-frame="true"><figure><img src=".gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure></div>

#### How Views Are Tracked

* A view is counted only when a unique HCP opens the Job/Shift Details and keeps it open for at least 3 seconds.
* If they close or navigate away before the 3-second threshold, no view is added.

#### Uniqueness & Exclusions

* Each HCP is counted once per job (1 unique user = 1 view).
* Repeat views by the same user do not increase the counter.
* Providers viewing their own postings are not counted.

#### Real-Time Metrics

* All view counts are stored in the database and update in real-time (or near real-time) across the Provider dashboard.

## Bug Fixes

* Fixed Shift Card Title from “Filled vacancies” to “Hired”
