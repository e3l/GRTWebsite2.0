# GRTWebsite2.0
A Next.js port of the GRT website, with the aims of keeping the theme the same but improving code readability and 
maintainability, as well as modernizing the CSS and JS logic.

### Changelog
The following is an incomplete changelog of differences from the old PHP website. I may move this to an issue or remove
this entirely at some point, perhaps after the port is finished.

#### Fundamental changes
- Next.js as a framework, instead of PHP and vanilla JS
- `tailwindcss` instead of raw CSS and style tags
- React instead of raw HTML
- PWA capabilities with `next-pwa` (this isn't strictly necessary, but we had the manifest already so I thought "why not?")

#### Bug fixes
- Fixed navbar wrapping and disappearing issues with `display: flex`
- Fixed subnavbar wrapping and expanding issues with `display: flex`
- Fixed navbar caret off centering the navlinks with `position: absolute`
- Fixed footer not staying at the bottom of the page when the content doesn't fill the whole screen
- Fixed page title saying "GRT | FIRST" on `/join`
- Fixed favicon on non-index pages

#### UI changes / improvements
- Added block quote for `firstinspires.org` quotes in `/FIRST` instead of having them be separate sections
- Made 2019 and 2018 in `/FIRST/accolades` obey the same award formatting as the other years
- Added jumbotron for "teach a man to fish" quote in `/mentors`
- Added captions to images in `/mentors/*`
- Used block quote for interview responses in `/mentors/*`
- Redid list styling, expanded on list items in `/join`
- Used disclosures for Q&A in `/summer`
- Added "elevator pitch" blurb section in `/summer`
- Added alert-ish box for the "sign-ups available" text in `/summer`
- Removed unnecessary one-item subnav for pages with no subpages
- Added a black overlay for text contrast on the home page slideshow
- Generally more semantic HTML; `<footer>` for the footer, `<header>` and `<nav>` for the navbar, etc.
