# Lightroom PhotoTagger Import Plugin

This Lightroom Classic Plug-In allows importing keywords as well as title, headline and description to photos from a CSV file which is e. g. written by the PhotoTagger app.

## Installation

- Download the latest release version
- Unzip it
- In Lightroom Classic, choose File -> _Plug-in Manager_
- Select _Add_ in the lower left.
- Choose the plugin directory and click _Add Plug-in_.

## Usage

Use the PhotoTagger app to tag photos and export the CSV File to your machine running Lightroom Classic.

- In Lightroom Classic, choose Library -> Plug-in Extras -> Import CSV (Photo Tagger)
- Select the file exported from PhotoTagger.
- See how the the plug-in imports metadata in the progress bar in the upper left.

## Documentation

See the [PhotoTagger homepage](https://www.kluks.de/apps/phototagger) for detailed information about the app and the plug-in, as well as further information, privacy policy and legal information.

# Development

First clone the repo:

    git clone kassi/phototagger.lrdevplugin

Next, add it to lightroom as mentioned in the usage above.

## Building

Bump the version by tagging with the next version number according to semver and push the commits and tags. The github action will create a new release and upload it to this and the public companion repo.

### Manually

Simply running

    make

will compile lua and create a `dist/PhotoTagger.x.y.z.zip` file, according to the current version number.

This file can be distributed.
