# KONG Website

This folder is the source code for [Kong](https://github.com/Mashape/kong)'s website. It is a [Jekyll](http://jekyllrb.com/) website hosted on GitHub pages.

## Requirements

- [npm](https://www.npmjs.com/)
- [Bundler](http://bundler.io/)
- [Ruby](https://www.ruby-lang.org) (>= 2.0, < 2.3)
- [Python](https://www.python.org) (>= 2.7.X, < 3)

## Install

>
```bash
gem install bundler
npm install
```

## Running locally

>
```bash
npm start
```

## Generating Public Lua API from Kong

- Have a local clone of Kong.
- Checkout the desired branch/tag/release.
- Set an env variable `KONG_PATH` to point to your local clone.
- Run: `gulp docs`
- Module docs are generated into `./lua-reference`.
- Manually move to the desired location (appropriate version folder).

## Search

We are using Algolia [docsearch](https://www.algolia.com/docsearch) for our CE documentation search. The algolia index is maintained by Algolia through their docsearch service. Their scraper runs every 24hr. The config used by the scraper is open source getkong.org config can be found [here](https://github.com/algolia/docsearch-configs/blob/master/configs/getkong.json). 

## Deploying

This will deploy to GitHub pages:

>
```bash
npm run deploy
```
