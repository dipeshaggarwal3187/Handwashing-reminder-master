# Handwashing reminder

An app that reminds you smartly when you have to wash your hands 💦👏

## Features

Currently, the application supports:

+ Send notifications at specific time. This feature was developed using
  the Android's
  [WorkManager](https://developer.android.com/topic/libraries/architecture/workmanager)
  but because the notifications were not working as expected (they were almost
  always delayed) the app now uses AlarmManager for waking the device at
  specific time, even if it is in Doze mode.
+ Detect user activity and send a notification when ends an specific
  one. For example, if he gets out of a vehicle, or has just finished
  running, etc. This was developed using Google's [Activity Recognition
  API](https://developers.google.com/location-context/activity-recognition).

Obviously there are more features but the "important" ones (the ones
that reminds you to wash your hands) are those.

In addition, using the [WHO](https://who.int) as source, there are a
"diseases information" view in which some information about dangerous
diseases is displayed. This feature uses Firebase Remote Config, so the
list can always be updated and changed without updating the entire
application.

Another section is focused on **how to wash your hands**. This task,
that may seem simple, is crucial for having a good health and avoid some
practices that can compromise it. This section contains informative
videos and images for guiding you through the entire process.

Finally, there is a **news** section which is still under development.
In a future I expect having there recent news about any important
disease.

### Dynamic modules
By using
[dynamic delivery](https://developer.android.com/guide/app-bundle/dynamic-delivery)
this application downloads and installs modules on-demand. That is, it
downloads and installs new features keeping the app size as low as
possible.


