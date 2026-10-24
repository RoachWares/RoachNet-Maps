<p align="center">
  <img src="https://roachnet.org/assets/readme/roachnet-maps.png" width="100%" alt="RoachNet Maps: offline map packs for the Maps pane, with no tile server.">
</p>

# RoachNet Maps

The offline map packs RoachNet's Maps pane draws: vector tiles in the PMTiles format, drawn on your Mac with no tile server and no web view. Once a pack is on your Mac, the map works without a connection.

**Maps 2026-10** · 57 packs, about 18 GB in all · [Maps guide](https://roachnet.org/docs/guides/maps/)

## What's here

The [2026-10 release](https://github.com/RoachWares/RoachNet-Maps/releases/tag/maps-2026-10) holds the packs:

- the 50 states and the District of Columbia;
- five territories: American Samoa, Guam, the Northern Mariana Islands, Puerto Rico and the U.S. Virgin Islands;
- a world overview (`global-min`).

`packs-inventory-2026-10.json` lists every pack with its size in bytes and its SHA-256, so you can check a download.

## Get a pack

You don't need to download packs by hand. In RoachNet, install the ones you want from [RoachNet Apps](https://roachnet.org/docs/guides/apps-and-packs/); **Install base maps** also queues the World Atlas. Downloads resume after a stall instead of starting over, and the packs are kept in `~/RoachNet/storage/maps/pmtiles`.

To check a pack you downloaded yourself:

```sh
shasum -a 256 delaware_2026-10.pmtiles
```

and compare the result with the pack's `sha256` in the inventory.

## Credit

Map data © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright), built with [Protomaps](https://protomaps.com/). RoachNet shows this credit on the map.

## Help

- **Documentation:** [roachnet.org/docs](https://roachnet.org/docs/)
- **Something wrong with a pack?** Email [support@roachwares.org](mailto:support@roachwares.org).

---

<sub>Made by RoachWares LLC. RoachNet · offline on purpose.</sub>
