# Credit Card Picker for iPhone

This is a Progressive Web App package. It can be added to an iPhone Home Screen after it is hosted at an HTTPS address and opened in Safari.

## Install on iPhone

1. Host all files in this folder at an HTTPS address.
2. Open that address in Safari on the iPhone.
3. Tap Share, then **Add to Home Screen**.
4. Tap **Add**.

The app shell and icons are cached for offline opening after the first successful visit. A live exchange-rate lookup needs an internet connection; the last fetched rate is retained on the device as a fallback.

## Privacy

The current `index.html` contains the card limits and statement-cycle days in its JavaScript data. Anyone who can access a hosted copy can inspect those values. Do not put this package on a public website or public repository unless you first remove those account-specific values or add access protection.

The exchange-rate lookup sends only the selected currency and PHP as the requested pair to Frankfurter. Purchase amounts are calculated on the device and are not sent by this app.

## Updating

Replace the hosted files with the updated package. If the app shell changes, increment `CACHE_NAME` in `sw.js` so installed devices refresh the cache.
