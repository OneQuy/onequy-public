# Tips for Submitting Your App to the App Store (Minimize Rejection)

<img src="https://pbs.twimg.com/media/GqFN3cra8AAnqJE?format=jpg&name=medium" height="200">

* **If your app requires account creation**, you must include a **"Delete Account"** button within the app.

* **If your app collects device IDs, uses tracking/analytics, or displays ads**, you must:

  * Request **tracking permission** from the user.
  * Add the following to your `Info.plist`:

    ```xml
    <key>NSUserTrackingUsageDescription</key>
    <string>Your description for why you need this permission</string>
    ```

* **If your app uses push notifications**, include the following in your `Info.plist`:

  ```xml
  <key>NSUserNotificationsUsageDescription</key>
  <string>Allow notifications to get important updates and event reminders from our app.</string>
  ```

* **Avoid including any reference to Android** (words, logos, or related content) in your app or App Store description.

* **If your app offers subscriptions or in-app purchases**, include a **"Restore Purchase"** button in the app.
