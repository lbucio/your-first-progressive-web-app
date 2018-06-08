## Your First Progressive Web App
Open West 2018

## Getting Started

### Reliable
- [Background Sync](https://developers.google.com/web/updates/2015/12/background-sync)

### Secure
- Served over HTTPS

### Fast
- [App Shell Model](https://developers.google.com/web/fundamentals/architecture/app-shell)

### Engaging
- [Configured Web App Manifest](https://developers.google.com/web/fundamentals/web-app-manifest/)
- [Installable](https://developers.google.com/web/fundamentals/app-install-banners/#criteria)
- [Push Notifications](https://developers.google.com/web/fundamentals/push-notifications/)
  - [Push API](https://developer.mozilla.org/en-US/docs/Web/API/Push_API)
  - [Notification API](https://developer.mozilla.org/en-US/docs/Web/API/Notifications_API)

1. App Shell Model
3. Service Worker
4. Cache Strategy

## PWA Support
- [Is Service Worker Ready](https://jakearchibald.github.io/isserviceworkerready/index.html#moar)

## Push Notifications
Two API's

### [Push API](https://developer.mozilla.org/en-US/docs/Web/API/Push_API)
The Push API gives web applications the ability to receive messages pushed to them from a server, whether or not the web app is in the foreground, or even currently loaded.

### [Notification API](https://developer.mozilla.org/en-US/docs/Web/API/Notifications_API)
The Notifications API allows web pages to control the display of system notifications to the end user.

## App Shell 
🎥[Instant Loading with the App Shell Model](https://www.youtube.com/watch?v=QhUzmR8eZAo)

The app shell should ideally:

- Load fast
- Use as little data as possible
- Use static assets from a local cache
- Separate content from navigation
- Retrieve and display page-specific content (HTML, JSON, etc.)
- Optionally, cache dynamic content

Reliable performance that is consistently fast. Repeat visits are extremely quick. Static assets and the UI (e.g. HTML, JavaScript, images and CSS) are cached on the first visit so that they load instantly on repeat visits. Content may be cached on the first visit, but is typically loaded when it is needed.

Native-like interactions. By adopting the app shell model, you can create experiences with instant, native-application-like navigation and interactions.

Economical use of data. Design for minimal data usage and be judicious in what you cache because listing files that are non-essential (large images that are not shown on every page, for instance) result in browsers downloading more data than is strictly necessary. Even though data is relatively cheap in western countries, this is not the case in emerging markets where connectivity is expensive and data is costly.

## Service Worker

- [Service Worker Demos](https://github.com/GoogleChrome/samples/tree/gh-pages/service-worker)
- [Service Worker, What are you?](https://kosamari.com/notes/Service-Worker-what-are-you)

## Web App Manifest
- [Browser Support](https://caniuse.com/#search=web%20app%20manifest)
  - Chrome **Enabled by Default**
  - Edge **Shipped**
  - [Firefox](https://platform-status.mozilla.org/#app-manifest) **In Development**
  - [Webkit](https://webkit.org/status/#specification-web-app-manifest) **In Development**
  
### Safari
- [Configuring Web Applications](https://developer.apple.com/library/archive/documentation/AppleApplications/Reference/SafariWebContent/ConfiguringWebApplications/ConfiguringWebApplications.html)
- [Add to Homescreen elements for Safari on iOS](https://developers.google.com/web/fundamentals/codelabs/your-first-pwapp/#add_to_homescreen_elements_for_safari_on_ios)

### Developer Tools

![Lighthouse Logo](/assets/images/pwa-lighthouse.png)

#### [Lighthouse](https://developers.google.com/web/tools/lighthouse/)

Lighthouse is an open-source tool from Google that audits a web app for PWA features

![Lighthouse example report](/assets/images/pwa-lighthouse-example.png)

## Resources
- [PWA Checklist](https://developers.google.com/web/progressive-web-apps/checklist)
- [Updates to Add to Home Screen Behaviour](https://developers.google.com/web/updates/2018/06/a2hs-updates)
- [Hacker News readers as Progressive Web Apps](https://hnpwa.com/)
- [PWA Rocks](https://pwa.rocks/)
- 🎥[Production Progressive Web Apps With JavaScript Frameworks](https://www.youtube.com/watch?v=aCMbSyngXB4)
- 🎥[PWA Roadshow](https://www.youtube.com/watch?v=z2JgN6Ae-Bo&list=PLNYkxOF6rcICnIOm4cfylT0-cEfytBtYt)

#### Offline
- 📚[Offline Web Apps - Udacity Course](https://www.udacity.com/course/offline-web-applications--ud899)
  - IndexedDB & Service Worker
- [Service Worker Cookbok](https://serviceworke.rs/)
- [Offline Cookbook](https://developers.google.com/web/fundamentals/instant-and-offline/offline-cookbook/)

#### Animations
- [CSS Triggers](https://csstriggers.com/)
- [FLIP](https://aerotwist.com/blog/flip-your-animations/)
- [Performant Expand and Collapse](https://developers.google.com/web/updates/2017/03/performant-expand-and-collapse)
- [Pull to Refresh - Overscroll Behaviour](https://developers.google.com/web/updates/2017/11/overscroll-behavior#disablp2r)

#### Push Notifications
- [Google Fundamentals](https://developers.google.com/web/fundamentals/push-notifications/)
- [Push Payload Demo](https://serviceworke.rs/push-payload_demo.html)

#### Performance
- [Why Mobile Speed Matters](https://www.doubleclickbygoogle.com/articles/mobile-speed-matters/)


### Helpful Libraries
- [Workbox](https://developers.google.com/web/tools/workbox/)
  - JavaScript Libraries for adding offline support to web apps
- [IndexedDB, but with promises](https://github.com/jakearchibald/idb)

## Frameworks

🎥[Production PWA with Frameworks](https://www.youtube.com/watch?v=aCMbSyngXB4)

{:.center.framework__logo}
![React Logo](/assets/images/react-logo.png)

{:.center}
### React

#### [React PWA Starter Kit](https://github.com/facebookincubator/create-react-app)
`create-react-app my-great-app`
##### What is Included
- By default, the production build is a fully functional, offline-first Progressive Web App
- An offline-first service worker and a web app manifest, meeting all the Progressive Web App criteria.
- All static site assets are cached so that your page loads fast on subsequent visits, regardless of network connectivity 
- Add to Homescreen capable

---

{:.center.framework__logo}
![Preact Logo](/assets/images/preact-logo.png)

{:.center}
### Preact

#### [Preact PWA Starter Kit](https://github.com/developit/preact-cli)

`preact create my-great-app`

##### What is Included
- 100/100 Lighthouse score, right out of the box
- Fully automatic code splitting for routes
- Auto-generated Service Workers for offline caching powered by sw-precache
- PRPL pattern support for efficient loading

---

{:.center.framework__logo}
![Polymer Logo](/assets/images/p-logo.png)

{:.center}
### Polymer

#### [Polymer PWA Starter Kit](https://github.com/Polymer/pwa-starter-kit)

[Demo](https://pwa-starter-kit.appspot.com/)

🎥[Google I/O Video](https://www.youtube.com/watch?v=we3lLo-UFtk)

##### What is Included
- All the PWA goodness (manifest, service worker)
- Responsive layout
- Application theming
- Example of using Redux for state management
- Offline UI
- Simple routing solution
- Fast time-to-interactive and first-paint through the PRPL pattern
- Easy deployment to prpl-server or static hosting
- Unit and integrating testing starting points
- Documentation about other advanced patterns.

---

{:.center.framework__logo}
![Vue.js Logo](/assets/images/vuejs-logo.png)

{:.center}
### Vue.js

#### [PWA Starter Template](https://github.com/vuejs-templates/pwa)

`vue init pwa my-project`

##### What is Included
- Service Worker precaching of application shell + static assets (prod)
- Script (async chunk) preloading using <link rel="preload">
- Web Application Manifest + favicons
- Mobile-friendly meta-viewport
- Lighthouse score of 90+/100

---

{:.center}
### Angular
### [Service Worker Support](https://angular.io/guide/service-worker-getting-started)

`ng add  @angular/pwa --project *project-name*`

[Angular Service Worker Intro](https://angular.io/guide/service-worker-intro)
