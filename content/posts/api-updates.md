---
title: API and NPM Updates
date: 2021-05-24
published: true
tags: ['Infinity Bots', 'API', 'Updates', 'NPM Module']
series: false
cover_image: ./images/4E360AF5-121E-4012-A4DC-58AEB9C65EE3.png
canonical_url: false
description: "Updates Regarding the Infinity Bots API and NPM Module"
author: "Toxic Dev - Lead Developer"
author_image: ./images/ToxicGif2.gif
---

Hello everyone, we have recently published a few minor API changes that may or may not effect our Users and or their Bots,
A list of Changes will can be found below for those of you who are interested in what has and has not changed.

---

## Major Changes
- Implement a “absolute” 404 to fallback to if the route or bot doesn’t exist thus avoiding hanging and timeouts. 
- Same as above ^ but for 500 (Internal Error) prevents the API from hanging if an error occurs which would most likely result in a timeout 
- Updated the POST method errors to show a `400 (Client Error)` or `401 (Unauthorized)` for null, undefined, or invalid Auth Token

## Minor Changes
- Begin support and implementation of a `All Approved Bots` route for the Infinity Bots API

## NPM Changes
- Updated and Cleaned up the NPM Module.
- Implememt a `GET` bot method.
- Implement a `GET` user method.

---


