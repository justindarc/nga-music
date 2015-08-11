music-nga
=========

Experiments in re-building the FxOS Music app using NGA

To set up development environment, clone this repo then run:
- `npm install`
- `bower install`

You may also occassionally need to run `bower update` to fetch the latest dependencies.

Running a local web server for development:
- Install [nws](https://www.npmjs.com/package/nws)
  + `npm install -g nws`
- From this repo's root directory, run `nws` (automatically serves up this app from HTTP port 3030)

To run on Firefox desktop (Developer Edition or Nightly):
- Check "Enable multi-process Firefox" in `about:preferences` > "General"
- Set `dom.webcomponents.enabled` to `true` in `about:config`
- Browse to `http://localhost:3030`

If you encounter any problems (e.g. HTTP 404 errors, crashes, etc.), try running Firefox with a fresh profile:
- [Use the Profile Manager to create and remove Firefox profiles](https://support.mozilla.org/en-US/kb/profile-manager-create-and-remove-firefox-profiles)

Note: You may occassionally need to clear your history to flush out the cache or go to `about:serviceworkers` to "Unregister" the Service Worker.
