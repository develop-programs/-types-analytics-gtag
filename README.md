# @types/analytics-gtag

## update

- 2019/06/24 0.0.1 Initial version

## How to use

Contains the following specifications.

https://developers.google.com/analytics/devguides/collection/gtagjs/pages
https://developers.google.com/analytics/devguides/collection/gtagjs/events
https://developers.google.com/analytics/devguides/collection/gtagjs/screens
https://developers.google.com/analytics/devguides/collection/gtagjs/user-timings
https://developers.google.com/analytics/devguides/collection/gtagjs/exceptions
https://developers.google.com/gtagjs/reference/api
https://developers.google.com/gtagjs/reference/event
https://developers.google.com/gtagjs/reference/parameter

```.ts
gtag("config", "GA_MEASUREMENT_ID", {
  page_title: "homepage",
  page_path: "/home"
});
gtag("config", "GA_MEASUREMENT_ID_1");
gtag("config", "GA_MEASUREMENT_ID_2");

gtag("event", "xyz");

gtag("event", "aaa", {
  event_category: "bbb",
  event_label: "ccc"
});

gtag("event", "login", { method: "Google" });

gtag("event", "video_auto_play_start", {
  event_label: "My promotional video",
  event_category: "video_auto_play",
  non_interaction: true
});

gtag("event", "screen_view", {
  app_name: "myAppName",
  screen_name: "Home"
});
gtag('config', 'GA_MEASUREMENT_ID', { 'app_name': 'myAppName' });
gtag('event', 'screen_view', { 'screen_name': 'Home'});


gtag('event', 'timing_complete', {
  'name' : 'load',
  'value' : 3549,
  'event_category' : 'JS Dependencies'
});
gtag('event', 'exception', {
  'description': 'error_description',
  'fatal': false
});
```

## license

- [MIT License](https://opensource.org/licenses/mit-license.php)
