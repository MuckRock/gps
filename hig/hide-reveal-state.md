# Maintaining state in hide/reveal UIs

Some parts of our interface let a user toggle visibility on parts of the page. For example, DocumentCloud uses navigation group components to hold related items. These can get unwieldy, so we let the user close them.

We can use `localStorage` to remember this state between page loads, so the user doesn’t have to reconfigure the page each time they visit. We generally only store this in the browser, not in a database, though it’s possible we could store settings like this in the future.
