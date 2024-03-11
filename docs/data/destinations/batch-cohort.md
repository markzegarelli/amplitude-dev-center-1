---
title: Send Cohorts to Batch
description: Sync cohorts from Amplitude to Batch
---

!!!Tip

    This integration is maintained by Batch. Contact the Batch support team for support with this integration. 

[Batch](https://batch.com/)  is a customer engagement platform that allows publishers to personalize push notifications and emails across multiple mobile platforms and web browsers. Batch offers a SaaS solution, integrating with clients' apps and websites via an SDK. This integration lets you sync cohorts from Amplitude to Batch.  

## Considerations

- This integration is available for customers who have paid plans with Amplitude.
- You must enable this integration in each Amplitude project you want to use it in.
- This integration requires a paid Batch plan.
- The integration requires both custom audiences and third-party connections in Batch.
- Batch expects an identifier that matches the Batch Custom User ID or the Installation ID field. This means the `user_id` or user property you select in Amplitude must contain the same identifier as the one tracked in Batch in one of these fields.

## Setup
Two types of cohort destinations can be setup for Batch:

- Use the **Batch (Profile)** destination if you want your cohorts to be synced with your Batch Omnichannel project.
- Use the **Batch** destination if you want your cohorts to be synced with a specific mobile app or website.

### Batch setup

1. In Batch, navigate to Settings > General.
2. Copy the API Key ("Live API Key" for mobile or "SDK API Key" for web) of the application in which you want to use Amplitude’s Cohorts OR the Project key of the omnichannel project in which you want to use Amplitude’s Cohorts.
3. Copy your account's REST API Key.

### Amplitude setup

1. In Amplitude Data, click **Catalog** and select the **Destinations** tab.
2. In the Cohort section, click **Batch** or  **Batch (Profile)**.
3. Click **Add another destination**.
4. Enter a **Name** and paste in the **API key** you copied from Batch.
5. Select the type of identifier composing your segment on Batch (Custom User ID / Installation ID).
6. Map the Amplitude `user_id` field to the Batch `user_id` field.
7. Save when finished.

## Send a cohort

To sync your first cohort:

1. In Amplitude, open the cohort you want to sync, then click **Sync**.
2. Select **Batch**, then click **Next**.
3. Choose the account you want to sync to.
4. Choose the sync cadence.
5. When finished, save your work.

## Locating your cohort in Batch

When the Cohort is synced to Batch, it appears in the “Audiences” tab of the dashboard. Select it in the targeting section of the campaign editor to use it in a Push, In-App, Email or SMS campaign. This is useful if you want to include or exclude a segment of users from your campaign.

### Use cases

- **Targeted Campaigns:** When you sync specific user cohorts from Amplitude to Batch, you can target those users more directly in push or In-App campaigns. For example, target a cohort of users who have abandoned their shopping carts with a notification that offers a discount to encourage completion of the purchase.
- **User Retention:** Identify cohorts of users who haven't engaged with the app or website for a set period in Amplitude and sync them to Batch. Re-engage these users with personalized content or updates relevant to their previous interactions, aiming to bring them back to the app or website.
- **Product Feedback and Updates:** For users who engage with certain features of an app or service (a cohort identified in Amplitude), syncing this information to Batch allows for sending specific notifications about updates, improvements, or requests for feedback on those features, ensuring that you reach the most relevant users.
