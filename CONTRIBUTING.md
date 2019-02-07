# Contributing

There are two pieces to `og-image` that are worth noting before you begin development.

1. The backend image generator located in [/src/card.ts](https://github.com/styfle/og-image/blob/master/src/card.ts)
2. The frontend inputs located in [/src/browser.ts](https://github.com/styfle/og-image/blob/master/src/browser.ts)

The Now 2.0 platform handles [routing](https://github.com/styfle/og-image/blob/master/now.json#L12) in an elegate way for us so deployment is easy.

However, local development requires a few steps.

1. Run `npm run develop` to get 
   1. TS to JS compilation file watch running (compiles on save)
   2. Run the backend (you can try it by visiting http://localhost:13463/Nice.png)
   3. Run the frontend and visit http://localhost:8080/public/index.html
2. If necessary, edit the `exePath` in [options.ts](https://github.com/styfle/og-image/blob/master/src/options.ts) to point to your local Chrome executable

Now you're ready to start local development!
