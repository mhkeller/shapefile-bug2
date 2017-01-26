Shapefile bug 2
===

## What's the problem

When reading in the dbf file `us-states/us-states.dbf`, the json has an extra item that shows up as:

```json
{
  "name": null,
  "fid": null
}
```

## How to reproduce

```sh
npm install
npm start
```

This will run `shp2json` and `dbf2json` and output the files. The shapefile output doesn't contain any extra or empty feature, as expected.
