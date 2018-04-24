# Documentation

The RAW Documentation is a [Hugo](https://gohugo.io/) site using the [Learn](https://learn.netlify.com/en/) theme. You can view the live version of the site at [http://docs.radio.warwick.ac.uk](http://docs.radio.warwick.ac.uk)

## Installation Instructions

1. Clone this repository `git clone --recursive https://github.com/radiowarwick/hugoDOS.git`
2. Install [Hugo](https://gohugo.io)

## Updating Version

To update the version online go to `/mnt/www/docs.radio.warwick.ac.uk` on the `raw` server. Pull the latest commit and then run `hugo` to build the changes.

## Testing & Building

- To build the site run `hugo` in the root directory. This creates the `public` directory.
- To run a local server run `hugo server` in the root directory. This will run on [http://localhost:1313](http://localhost:1313).
