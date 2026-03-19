# Account Deletion Policy — ZepWash Customer App

**Last updated:** March 2026

---

## Overview

ZepWash allows customers to permanently delete their account and all associated personal data directly from within the app. This policy describes what data is collected, how to request deletion, what gets deleted, and what (if anything) is retained.

---

## How to Delete Your Account

Account deletion is available entirely in-app — no email or support request is required.

1. Open the **ZepWash** app and sign in.
2. Tap the **Profile** tab (bottom navigation).
3. Scroll to the bottom and tap **Delete Account**.
4. Read the warning and tap **Continue**.
5. Confirm the final prompt by tapping **Permanently Delete**.

Your account and all associated data will be wiped immediately. You will be signed out automatically.

> If you are unable to access the app, you may also request deletion by contacting us at **support@zepwash.in** with the registered phone number. We will process the request within **7 business days**.

---

## Data Collected by ZepWash

When you use the ZepWash customer app, the following data is collected and stored:

| Data | Purpose |
|---|---|
| Mobile phone number | Account identity and OTP authentication |
| Full name | Personalization and service communication |
| Home / service address | Locating the vehicle for daily cleaning |
| Vehicle make / model | Service reference |
| Vehicle registration plate code | Uniquely identifying your vehicle |
| Vehicle type (hatchback / sedan / SUV) | Determining subscription pricing |
| Subscription details (plan, status, dates) | Managing your active car wash subscription |
| Razorpay subscription & payment records | Billing and payment history |
| Cleaning records (daily status) | Tracking service delivery |
| Complaints filed | Resolving service issues |
| Push notification token (FCM) | Sending service and payment reminders |

---

## What Gets Deleted

When you delete your account, the following data is **permanently and irreversibly removed**:

- **Account & identity** — Firebase Authentication record (phone number, UID)
- **Profile** — Name, phone number (`users` collection)
- **Customer profile** — Address, vehicle details, subscription status (`customers` collection)
- **Subscription records** — All subscription documents linked to your account
- **Cleaning records** — All daily cleaning entries (pending, completed, and missed)
- **Complaints** — All complaints you have filed
- **Payment records** — All Razorpay payment documents linked to your account
- **Staff assignment** — Your vehicle is removed from the assigned staff member's task list

Deletion is applied across all Firebase services (Firestore, Firebase Authentication).

---

## Data Retention After Deletion

| Data type | Retention |
|---|---|
| All Firestore documents listed above | Deleted immediately on confirmation |
| Firebase Auth record | Deleted immediately on confirmation |
| Razorpay subscription (payment gateway side) | Governed by [Razorpay's data retention policy](https://razorpay.com/privacy/); ZepWash has no control over records held by Razorpay |
| Aggregated / anonymised analytics | Not applicable — ZepWash does not retain anonymised derivatives of your data |

ZepWash does not retain any personally identifiable information after account deletion.

---

## Effect on Active Subscriptions

If you have an **active Razorpay subscription** at the time of deletion:

- Your ZepWash account data is deleted immediately.
- The Razorpay subscription will **not** automatically cancel on the Razorpay side. You should cancel it before deleting your account via the **Manage Subscription** screen, or contact Razorpay support directly.
- No further cleanings will be scheduled or performed after deletion.

---

## Contact

For questions about this policy or to request manual deletion:

**Email:** support@zepwash.in
**App:** Profile → Delete Account
