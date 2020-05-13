
[![Netlify Status](https://api.netlify.com/api/v1/badges/d6a0ccf7-b5d1-4588-b628-84819681c478/deploy-status)](https://app.netlify.com/sites/at-lab-nuxt-prismic-i18n/deploys)

# Active talents lab - Prismic / Nuxt - i18n 

> [Demo](https://at-lab-nuxt-prismic-i18n.netlify.app/) 

# This demo is based on  

> [Phil Snows / Prsimic.io - Prismic Nuxt.js Multi-page website example ](https://github.com/prismicio/nuxtjs-website) 


## Launch this project in your local environment

Run the following commands:

``` bash
npm install
npm run dev
```
Then you can access it at [http://localhost:3000](http://localhost:3000).

## Compile and minify for production and launch the server
``` bash
npm run build
npm start
```

## Learn more about using Prismic with Nuxt.js

> [Prismic Nuxt.js Documentation](https://prismic.io/docs/vuejs/beyond-the-api/primsic-nuxt)

# nuxt-i18n Implementation

This was a quick POC according to the [nuxt-i18n documentation](https://nuxt-community.github.io/nuxt-i18n/).

### Prismic.io
I added two locales 'fr-fr' and 'sv-se', my deafult was 'en-us'.
And i added content for each page and locale. 
You can easaly [copy](https://user-guides.prismic.io/en/articles/2760541-copy-content-to-a-different-locale) your content form one locale to another in prismic. 

### nuxt-i18n

``` bash
npm i nuxt-i18n
```

### store/index.js
I had to fetch three menus, one for each language and add them to the [store](https://github.com/kennethillman/at-lab-nuxt-prismic-i18n/blob/master/store/index.js). 

### components/HeaderPrismic.js
Add language choice and navigation to the [header](https://github.com/kennethillman/at-lab-nuxt-prismic-i18n/blob/master/components/HeaderPrismic.vue) according to i18n.locale. _(Needs refinement)_ 

### pages
Updated async asyncData so prismic get data according to locale. [pages](https://github.com/kennethillman/at-lab-nuxt-prismic-i18n/tree/master/pages)  _(Needs refinement)_ 

### plugins/i18n.js
Added plugin [i18n]((https://github.com/kennethillman/at-lab-nuxt-prismic-i18n/blob/master/plugins/i18n.js)). 

### lang/*.json
Added the [languages](https://github.com/kennethillman/at-lab-nuxt-prismic-i18n/tree/master/lang).