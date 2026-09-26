# Desk Widgets: Website

The public home page, privacy policy and terms of service for [Desk Widgets](https://github.com/sevensixteeeen/desk-widgets), a personal Windows desktop widgets app.

Google requires these pages before an app that uses Google sign-in can be published. They're linked from the app's Google sign-in screen and shown to anyone who connects their Google Calendar.

## Live pages

| Page | URL |
|---|---|
| Home | https://sevensixteeeen.github.io/desk-widgets-site/ |
| Privacy policy | https://sevensixteeeen.github.io/desk-widgets-site/privacy.html |
| Terms of service | https://sevensixteeeen.github.io/desk-widgets-site/terms.html |

## Files

```
index.html     Home page: what the app is
privacy.html   What data the app accesses, how it's used, and how to remove access
terms.html     Terms of use
```

Plain HTML with inline CSS. No build step, no dependencies, no tracking.

## Hosting

Served by **GitHub Pages** from the `main` branch, root folder (**Settings → Pages**). Changes go live about a minute after pushing.

## Connected Google settings

These pages are used in **Google Cloud → Google Auth Platform → Branding**:

| Branding field | Value |
|---|---|
| Application home page | `https://sevensixteeeen.github.io/desk-widgets-site/` |
| Privacy policy link | `https://sevensixteeeen.github.io/desk-widgets-site/privacy.html` |
| Terms of service link | `https://sevensixteeeen.github.io/desk-widgets-site/terms.html` |
| Authorized domain | `sevensixteeeen.github.io` |

> **Don't rename, move or delete these files, and don't make this repo private.** Google checks these URLs. If they stop loading, the app can be flagged and Google Calendar sign-in may stop working.

## Keeping it accurate

The privacy policy must describe what the app **actually** does. Update `privacy.html` and its "Last updated" date whenever the app changes how it uses Google data, for example when a new Google permission (scope) is added.

Current Google permissions:

| Scope | Used for |
|---|---|
| `calendar.readonly` | Seeing the list of calendars and reading their events |
| `calendar.events` | Adding events the user creates in the calendar widget |

The app never changes or deletes existing events, and it has no server. Everything stays on the user's PC.

## Related

- App source code: [sevensixteeeen/desk-widgets](https://github.com/sevensixteeeen/desk-widgets)
