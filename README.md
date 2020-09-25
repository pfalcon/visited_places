# Yet Another "Visited Places" Map

This is a simple local web application which allows to visualize countries
and places (cities, etc.) you have visited during travels.

There are gazillion of apps like that, here are the traits of this one:

* Standalone HTML+JavaScript webapp, no backend.
* Doesn't rely on 3rd-party web services like Google Maps, which change all
  the time and will break the app.
* Doesn't even pull any files from Internet, all dependencies
  ([D3](https://d3js.org/) and
  [D3 Datamaps](https://github.com/markmarkoh/datamaps)) are mirrored
  locally.
* Visited countries/cities info is stored in simple JSON-like files (which
  you edit with your text editor).

Missing features:

* No zoom (the webapp is based on D3 Datamaps which doesn't support
  interactive zoom as builtin feature; patches to add zoom support in
  a clean way (no bloat please!) are welcome).

How to use:

* Clone git repo.
* Edit `countries.js` and `cities.js` files following sample data they
  already have.
* Open `index.html` in a browser.
* Deploy all files to a webserver if you want a map to be accessible on
  Internet. (E.g., you can use Github Pages, example is here:
  https://pfalcon.github.io/visited_places/).

Customization:

* Refer to [D3 Datamaps](http://datamaps.github.io/) docs and samples.

Credits:

Based on D3 Datamaps examples. Put together by Paul Sokolovsky. MIT
license.
