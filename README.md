## Your First Progressive Web App
Open West 2018

### Getting Started
1. 

### PWA Support

### Developer Tools

![Lighthouse Logo](/assets/images/pwa-lighthouse.png)
#### [Lighthouse](https://developers.google.com/web/tools/lighthouse/)

Lighthouse is an open-source tool from Google that audits a web app for PWA features

![Lighthouse example report](/assets/images/pwa-lighthouse-example.png)

### Resources

- [Hacker News readers as Progressive Web Apps](https://hnpwa.com/)
- [Production Progressive Web Apps With JavaScript Frameworks](https://www.youtube.com/watch?v=aCMbSyngXB4)

#### Offline
- [Offline Web Apps - Udacity Course](https://www.udacity.com/course/offline-web-applications--ud899)
  - IndexedDB & Service Worker
- [Service Worker Cookbok](https://serviceworke.rs/)

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
- [IndexedDB, but with promises](https://github.com/jakearchibald/idb)

## Frameworks

{:.center}
![Polymer Logo](/assets/images/p-logo.png)

### Polymer
#### [Polymer PWA Starter Kit](https://github.com/Polymer/pwa-starter-kit)
[Demo](https://pwa-starter-kit.appspot.com/)
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

{:.center}
![Vue.js Logo](/assets/images/vuejs-logo.png)

### Vue.js
#### [PWA Starter Template](https://github.com/vuejs-templates/pwa)
`vue init pwa my-project`
##### What is Included
- Service Worker precaching of application shell + static assets (prod)
- Script (async chunk) preloading using <link rel="preload">
- Web Application Manifest + favicons
- Mobile-friendly meta-viewport
- Lighthouse score of 90+/100
