# RingCentral CRM Extension Client

It is to work with the server code: https://github.com/ringcentral/rc-unified-crm-extension

## Quick start

Assuming you have already setup your local server, let's then start setting up your client app. Here are the steps:

1. `npm i`
2. In `src`, there's a `manifest.sample.json`, rename it to `manifest.json` and fill in. As at development stage, the only required field is `defaultCrmManifestUrl`.
3. `npm run build`
4. The build will be in `dist` folder
5. To install it, go to chrome://extensions/ and toggle on "Developer mode" and click "Load unpacked"

## Add your CRM

This client app is a Chrome extension which has url matcher to control its accessibilities. To add your CRM urls:

1. Open `public/manifest.json`
2. Under `content_scripts.matches`, add your CRM's url
3. Under `web_accessible_resources/matches`, add your CRM's url