# About

This app reproduce a bug with Turbo and chromium based iOS navigators (Chrome and Brave at least).

This app is accessible on heroku : (https://tranquil-river-18127-f762de0e1a1d.herokuapp.com/)[https://tranquil-river-18127-f762de0e1a1d.herokuapp.com/]

## How to Reproduce bug

1. Go to `/products` with a Chromium based iOS navigator, (you need an iOS device)
2. Scroll down to card 40
3. Take care to not scroll up (bottom bar with back button should not appear)
4. Click on any card
5. See that scroll position is set to bottom of page

Notes :

- This bug does not happen if you click on top cards (until number 20). Don't know why, but maybe you have to scroll more than next page document height (my guess).
- This bug does not happen neither if after scrolled to card 40 for exemple, you scroll up until bottom bar (with back button) appears. If you click on link with visible bottom bar, the bug won't happen.

## Running locally

Just clone this repository, and run `bundle`, `yarn`, and `dev`. It'll be accessible on `localhost:3000`.
