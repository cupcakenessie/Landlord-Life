# LANDLORD LIFE — Mobile Edition

A phone-first playable prototype designed for Android/iPhone/iPad testing through a browser/PWA. It is offline-first and uses localStorage for the current prototype save.

## Run on Android
1. Put the `LandlordLife` folder on a static web host (GitHub Pages, Netlify, Cloudflare Pages, etc.) or serve it from a local development server.
2. Open the URL in Chrome on Android.
3. Use the browser menu → **Add to Home screen** / **Install app** where available.
4. The service worker caches the core files after the first successful load, enabling offline play.

Opening `index.html` directly with `file://` may prevent service-worker installation; use a normal web server for install/offline behavior.

## Current playable systems
- First rental home
- Hourly rent simulation (1 in-game hour = 30 seconds for prototype testing)
- Tenant applicants and affordability
- Tenant satisfaction/reliability/lifestyle data
- Tenant life event decisions
- Furniture upgrades with compounding +5% rent
- Property value/rating
- Second property at Level 2
- XP and level progression
- Daily rewards/streak
- Missions
- City unlock map
- Offline income cap (8 in-game hours)
- Farm mini-loop (Level 10)
- Business mini-loop (Level 15)
- Hotel mini-loop (Level 20)
- Banking/credit/loan foundation
- Online/offline indicator
- Local save
- Responsive portrait mobile UI

## Future production integrations
- Unity/native packaging
- Apple/Google account authentication
- Cloud save with version conflict resolution
- Server-authoritative online economy
- Google Play Billing
- Apple StoreKit
- AdMob rewarded ads
- Leaderboards/tournaments
- Push notifications
- Analytics/remote configuration
- Production art, animation, audio and localization

This prototype deliberately keeps core gameplay independent from network services.
