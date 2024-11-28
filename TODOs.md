TODOs for the light mode theme:

- [x] Invert SVGs
- [x] Invert most images
- [x] Get body text legible
- [x] Get all text legible
- [x] Remove un-necessary `-inverted.svg` files
- [x] Fix images:
    - [x] Hamburger menu
    - [x] /404.html
    - [x] news
	      - [x] news/introducing-bevy/
        - [x] and other instances of `bevy_logo_dark.svg`.
        - [x] charts on ~~news/bevy-0-2/, 0-3/, 0-4/, 0-5/, 0-6/, 0-8/, 0-12/~~, 
        - [x] news/community-reflection-on-bevys-third-year/
   - [x] frontmatter
       - Rather than individually addressing each image, I simply changed the CSS
       - [ ] ~~bevy birthday~~
       - [ ] ~~scaling bevy~~
       - [ ] ~~webgpu.svg~~
       - [ ] ~~foundation~~
- [x] Give the colors another pass; make it look good!
    - [x] Donate page
    - [x] Error/Warn/Info boxes
    - [x] The rest!
- [x] Merge in from `main`
- [x] Check new pages:
    - [x] Bevy fourth birthday
    - [x] `contributing/`
    - [x] Generate assets and look through those, too
        - [x] generate_assets
        - [x] generate_examples
        - [x] generate_errors
- [ ] Update preview
- [ ] Theme toggle: https://css-tricks.com/a-complete-guide-to-dark-mode-on-the-web/
    - [ ] Make MVP as separate project: Three-state Javascript toggle, defaults to dark, except without JS, defaults to prefers-system color scheme
    - [ ] Retrofit into existing theme
- [ ] Ping BD103 on the PR once it's ready: