What is XSS Chef?
=================
XSS Chef is a small React.js application inspired by [CyberChef](https://gchq.github.io/CyberChef/), which provides users with a modular way to build JavaScript payloads to typically be used during penetration tests to demonstrate cross-site scripting vulnerabilities.

A live copy of the application can be found at [https://rastating.github.io/xss-chef](https://rastating.github.io/xss-chef)

What Can I Do with XSS Chef?
============================
The current set of recipes can be found below, along with a description of what they allow you to do:

* **Alert** - Display an alert in the user's browser
* **Body Replacer** - Replace the inner HTML of the document body with custom markup
* **Cookie Exfiltrator** - Exfiltrate one or more cookies to an external web server
* **Decimal Encoder** - Encode the payload into a comma separated array of decimal numbers
* **Link Hijacker** - Change the `href` attribute of all links on the page to point to a different URL
* **Keylogger** - Log all key presses on the page and submit them back to a web server
* **String Exfiltrator** - Request a resource from the target's browser and exfiltrate the data
* **WordPress: Create User** - Create a new WordPress user account on the target system

How to Build
============
* For a production build, run: `yarn build`
* For a development build, run: `yarn build-dev`

Running Unit Tests
==================
The unit tests can be run with jest: `yarn jest`

Want to Contribute?
===================
If you're interested in helping to improve XSS Chef, below are some of the key things that I'd like to add at some point:

* **More recipes!** - This can be application specific (like the existing WordPress payload) or generic recipes (such as the cookie exfiltrator)
* **Better mobile support** - Although there is probably minimal use case for people to use the application on their mobile devices, it would be cool to iron out the bugs with the responsive design at low resolutions.
* **A better way to browse recipes** - Currently, as there are limited recipes available, the existing approach works. As more are added, a categorised list would be better, to aid users in navigating the available recipes.
