# att-website

Welcome to my personal website repo 👨‍💻

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

# Files missing are:
`.firebaserc`
```json
{
  "projects": {
    "default": "***-*******-*****"
  }
}
```

`firestore.rules`
```
rules_version = '1';
service cloud.firestore {
  **************
}
```

`nuxt.config.js`
```js
export default {
  target: 'static',
  head: {
    title: 'Artur Teixeira - Freelance Software Engineer',
    meta: [
      { charset: 'utf-8' },
      { name: 'viewport', content: 'width=device-width, initial-scale=1' },
      { hid: 'description', name: 'description', content: '' },
    ],
    link: [{ rel: 'icon', type: 'image/x-icon', href: '/favicon.ico' }],

    // Global site tag (gtag.js) - Google Analytics
    __dangerouslyDisableSanitizers: ['script'],
    script: [
      { src: 'https://www.googletagmanager.com/gtag/js?id=G-**********', async: true },
      {
        innerHTML: `window.dataLayer = window.dataLayer || [];
        function gtag(){dataLayer.push(arguments);}
        gtag('js', new Date());
        gtag('config', 'G-**********');`
      }],
  },

  // Smooth Scrolling
  router: {
    scrollBehavior(to) {
      if (to.hash) {
        return window.scrollTo({
          top: document.querySelector(to.hash).offsetTop - 32,
          behavior: 'smooth'
        })
      }
      return window.scrollTo({ top: 0, behavior: 'smooth' })
    }
  },

  css: [],
  plugins: [],
  components: true,
  buildModules: [
    '@nuxt/typescript-build',
    '@nuxtjs/tailwindcss',
  ],

  modules: [
    [
      '@nuxtjs/firebase',
      {
        config: {
          apiKey: '***************************************',
          authDomain: '***-*******-*****.firebaseapp.com',
          projectId: '***-*******-*****',
          storageBucket: '***-*******-*****.appspot.com',
          messagingSenderId: '************',
          appId: '*:************:web:**********************',
          measurementId: 'G-**********'
        },
        services: {
          firestore: true
        }
      }
    ],
  ],

  build: {},
}
```
