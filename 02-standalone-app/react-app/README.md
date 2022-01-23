This is a video export-enabled version of the [TripsLayer example](https://deck.gl/examples/trips-layer/)
on [deck.gl](http://deck.gl) website.

### Purpose

Users can drag, zoom in and zoom out, change pitch and bearing from within the deckgl canvas. The camera will start at the last position (viewState) the user was at, improving the experience of exporting the camera movements.

![](./trips.gif)

### Usage

Copy the content of this folder to your project.

To see the base map, you need a [Mapbox access token](https://docs.mapbox.com/help/how-mapbox-works/access-tokens/). You can either set an environment variable:

#### file copy

```
cp .env.sample .env
```

### Set mapbox access token

```
MapboxAccessToken=pk.xxxxxxxxxxxxx
```

#### or change the style of the map

```
const MAP_STYLE = 'mapbox://styles/mapbox/dark-v9';
 ↓
const MAP_STYLE = 'https://basemaps.cartocdn.com/gl/dark-matter-nolabels-gl-style/style.json';
```

Or set `MAPBOX_TOKEN` directly in `app.js`.

Other options can be found at [using with Mapbox GL](https://deck.gl/docs/get-started/using-with-map).

### Installation

```bash
# do this once per example
yarn

# To run the example
yarn start
```
