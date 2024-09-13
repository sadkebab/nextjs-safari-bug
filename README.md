# About

This repository was created for the reproduction of the bug reported in [this issue](https://github.com/vercel/next.js/issues/70079).

## The issue

Next.js in development mode throws a client-side exception on Safari 16.3 in version 14.2.11.

## How to reproduce

1. `pnpm dev`
2. Open localhost:3000 on safari 16.3, it will always show a black screen with the "Application error: a client-side exception has occurred (see the browser console for more information)." message if you are using the App Router or a blank white screen if you are using the Pages Directory
3. Change version of next to 14.2.10 in package.json
4. `pnpm i`
5. `pnpm dev`
6. Open localhost:3000 on safari 16.3, it will show the default home page for a new next.js project
