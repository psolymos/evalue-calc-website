# Website

Based on the [Minimal Mistakes Jekyll theme](https://mmistakes.github.io/minimal-mistakes/)
under and MIT license.

- edit `_config.yml` to update site metadata, Google Analytics etc
- edit `_data/navigation` to add more tabs to the top navigation

Adding apps:

Create new folder in the root, e.g. `app` and add `app/index.md` file
with the following content: change the app url

```
---
layout: app
app_url: http://www.evalue-calculator.com/
---
```

Important note: in the GitHub pages settings, do NOT force https if the shiny app is not served over https. Otherwise the iframe won't display the app. This is the case with the Heroku free tier. So use http protocol. Alternatively, set up SSL via [Cloudflare for Heroku](https://support.cloudflare.com/hc/en-us/articles/205893698-Configure-Cloudflare-and-Heroku-over-HTTPS) for free.
