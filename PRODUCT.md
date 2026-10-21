# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Static HTML, CSS and JavaScript, chosen to keep GitHub Pages deployment simple and NAS migration straightforward.

## Users

Primary user: the owner of a personal music library, using the site on both phone and desktop to find, play, collect, organize and download music.

## Product Purpose

Provide one fast personal music space for searching public music sources, playing tracks with synchronized lyrics, saving favorites and playlists, importing local audio and downloading available files.

## Positioning

Orbit is a personal listening workspace rather than a promotional music landing page: search, playback, lyrics and library management are visible and usable immediately.

## Operating Context

Used in a browser, often on a phone. Search results come from the existing Orbit API. Favorites, playlists and download history are saved in the current browser. The project will be hosted on GitHub Pages first and may later move to a local NAS.

## Capabilities and Constraints

- Search by song, artist or album across the existing aggregate sources.
- Play a selected result and show synchronized lyrics.
- Favorite tracks, create playlists, manage the library and record downloads.
- Import local audio files for the current browser session.
- Responsive desktop, tablet and phone layouts.
- Must not overwrite either existing Orbit repository.
- The upstream public music sources may require network access available in the user's region.

## Brand Commitments

The working product name is Orbit Music. The interface should feel professional and contemporary, not like a promotional poster, decorative equalizer, cassette illustration or generic AI landing page.

## Evidence on Hand

- Existing working search/playback/library behavior in the preceding Orbit Music build.
- Existing Orbit API endpoint and response handling in `app.js`.
- No testimonials, audience metrics or licensed editorial photography; none should be fabricated.

## Product Principles

- Playback is always one obvious action away.
- Music content, cover art and lyrics carry the visual identity.
- The phone layout is a first-class composition, not a compressed desktop page.
- Empty, loading and error states explain the next action plainly.
- Personal library data remains local and transparent to the user.

