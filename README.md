# wled-hyperion-ledfx
A simple implementation of the "missing" features from the WLED integration for Home Assistant,
including overriding Hyperion and LedFx, for users of each.

## Requirements
You will need a light integrated by the WLED integration (`light.wled` in these files).
This should work with segments or multiple lights, but the packages will need to be duplicated and updated for each light.

## Usage
 * Download all the `.yaml` files from this repository.
 * Place `wled.yaml` in your Home Assistant `/config` directory.
 * Copy the contents of `secrets.yaml` into your existing file (or the whole file if you don't already have them).
 * Update the paths in `secrets.yaml` to match your WLED instance. //i.e. your URL.
 * Add the `package` lines from `configuration.yaml` into your existing file.
 * Restart Home Assistant.

### Lovelace
*  Copy the contents of `lovelace.yaml` into a "Manual" Lovelace card, update the address for the "peek" bar, and save the card.
