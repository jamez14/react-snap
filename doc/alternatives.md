# Alternatives

## Prerendering, snapshoting

|                               | react-snap | [prerender-spa-plugin][prerender-spa-plugin] | [react-snapshot][react-snapshot] | [prep][prep] | [snapshotify][snapshotify] |
|-------------------------------|------------|----------------------------------------------|----------------------------------|--------------|----------------------------|
| State                         | supported  | looking for maintainer                       | unsupported                      | unsupported  | experimental               |
| DOM implementation            | puppeteer  | phantomjs-prebuilt                           | jsdom                            | nightmare    | puppeteer                  |
| Doesn't depend on Webpack     | +          | -                                            | +                                | +            | +                          |
| Doesn't depend on React       | +          | +                                            | -                                | +            | -                          |
| Load performance optimisation | +          | -                                            | -                                | -            | +                          |
| Zero-configuration            | +          | -                                            | +                                | -            | +                          |
| Redux                         | +          | -                                            | +                                | -            | -                          |
| Assync components             | +          | -                                            | -                                | -            | +                          |
| Webpack code splitting        | +          | [+][code-splitting]                          | -                                | -            | +                          |
| `CSSStyleSheet.insertRule`    | +          | -                                            | -                                | -            | +                          |
| blob urls                     | +          | ?                                            | -                                | -            | -                          |
| All browser features          | +          | -                                            | -                                | ?            | +                          |

[prerender-spa-plugin]: https://github.com/chrisvfritz/prerender-spa-plugin
[react-snapshot]: https://github.com/geelen/react-snapshot
[prep]: https://github.com/graphcool/prep
[snapshotify]: https://github.com/errorception/snapshotify
[code-splitting]: https://github.com/chrisvfritz/prerender-spa-plugin#code-splitting

- Load performancs optimisation - something beyond rendering HTML, like critical CSS
- Zero-configuration - provides sensible defaults
- **Redux** - can save state at the end of redering
- **assync components** - can save state of async componets to prevent flash on the client side
- `insertRule` - Works with CSS-in-JS solutions which use `CSSStyleSheet.insertRule`
- **blob urls** - removes blob urls from generated HTML

### Less popular options

- [prerenderer](https://github.com/tribex/prerenderer), experimental, jsdom, cheerio, chrome-remote-interface
- [prerender-chrome-headless](https://github.com/en-japan-air/prerender-chrome-headless), puppeteer
- [chrome-render](https://github.com/gwuhaolin/chrome-render), chrome-pool (chrome-remote-interface, chrome-runner)
- [react-prerender](https://github.com/Robert-W/react-prerender), react, cheerio
- [simple-react-prerender](https://github.com/beac0n/simple-react-prerender), react, jsdom, mock-browser, isomorphic-fetch
- [vue-prerender](https://github.com/eldarc/vue-prerender), experimental, vue, puppeteer
- [prerender-seo](https://github.com/posrix/prerender-seo), phantomjs-prebuilt
- [puppeteer-prerender](https://github.com/fenivana/puppeteer-prerender), puppeteer, request
- [puppeteer-prerenderer](https://github.com/GoodeUser/puppeteer-prerenderer), puppeteer
- [pre-render](https://github.com/kriasoft/pre-render), chrome-remote-interface, chrome-launcher, lighthouse-logger
- [prerender-plugin](https://github.com/mubaidr/prerender-plugin), webpack, puppeteer

## SEO-only server prerenderers

- [rendertron](https://github.com/GoogleChrome/rendertron), chrome-remote-interface, chrome-launcher
- [prerender](https://github.com/prerender/prerender), chrome-remote-interface
- [puppetron](https://github.com/cheeaun/puppetron), puppeteer
- [pupperender](https://github.com/LasaleFamine/pupperender), puppeteer
- [spiderable-middleware](https://github.com/VeliovGroup/spiderable-middleware), request

## Other

- [usus](https://github.com/gajus/usus), chrome-remote-interface, chrome-launcher
- [hypernova](https://github.com/airbnb/hypernova)
- [static-site-generator-webpack-plugin](https://github.com/markdalgleish/static-site-generator-webpack-plugin), webpack
- [Sitepack: A toolkit for building lazymorphic applications](https://github.com/sitepack/sitepack)

## React static site generators

- [gatsby](https://github.com/gatsbyjs/gatsby)
- [phenomic](https://github.com/phenomic/phenomic)
- [react-static](https://github.com/nozzle/react-static)

## SSR

- [razzle](https://github.com/jaredpalmer/razzle), react
- [next.js](https://github.com/zeit/next.js/), react
- [nuxtjs](https://nuxtjs.org/), vue
- [Create React App Universal CLI](https://github.com/antonybudianto/cra-universal), react

## WebComponents

- [talk: WebComponents SSR](https://youtu.be/yT-EsESAmgA)
- [skatejs/ssr](https://github.com/skatejs/ssr)
- [rendertron#web-components](https://github.com/GoogleChrome/rendertron#web-components)
- [shadydom](https://github.com/webcomponents/shadydom)

## Headless browsers

- Puppeteer vs chrome-launcher - [WIP: use chrome-launcher for handling the browser](https://github.com/GoogleChrome/puppeteer/pull/23)
- [HeadlessBrowsers](https://github.com/dhamaniasad/HeadlessBrowsers)
- [Puppeteer for Firefox](https://github.com/autonome/puppeteer-fx)
