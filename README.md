# Firefox favicon .ico size bug (retina)

Example code showing a Firefox favicon bug for .ico files with multiple embedded sizes on retina displays

## Instructions

- `npx serve src`

- Open <http://localhost:3000> in Firefox

- Move the Firefox window between a retina screen and a non-retina screen

- Observe that on the retina screen, Firefox chooses the 96px favicon instead of the 32px, resulting in a difficult to read icon

- I expect that the favicon will choose either the 16px or 32px version depending on whether the screen is retina or not. It doesn't seem correct to downscale a drastically larger icon since favicons have very limited real estate, and the smaller designs will typically look better scaled up.
