
## Examples
Schema for CSV training data labels:
1. `id`: A unique sequential non-negative integer identifier for the data point.
2. `quadkey`: A zoom 15 [Bing Tile](https://learn.microsoft.com/en-us/bingmaps/articles/bing-maps-tile-system)
   quadkey containing the center of the image.
3. `latitude`: The latitude of the center of the image in the [WGS 84 datum](https://en.wikipedia.org/wiki/World_Geodetic_System).
4. `longitude`: The longitude of the center of the image in the [WGS 84 datum](https://en.wikipedia.org/wiki/World_Geodetic_System).
5. `num_true`: Number of true votes, i.e., votes that this image contains a building.
6. `num_false`: Number of false votes, i.e., votes that this image does not contain a building.
7. `num_unsure`: Number of unsure votes, i.e., votes that this image is unclear whether it contains a building.
8. `num_error`: Number of error votes, i.e., votes that this image has an error or image artifact.

## Requirements
HighResolutionSettlementLayer requires or works with
* Mac OS X or Linux
* and presently only requires Gzip to unpack and ability to access CSV (comma seperated value) files

## Building HighResolutionSettlementLayer
* CURRENTLY NOT APPLICABLE

## Installing HighResolutionSettlementLayer
* CURRENTLY NOT APPLICABLE

## How HighResolutionSettlementLayer works
*This repo contains a selection from the training, validation, and test data for
the [High Resolution Settlement Layer] (https://dataforgood.facebook.com/dfg/tools/high-resolution-population-density-maps)
dataset. The current data consists of 9869460 data points with location and rater scores.*

## Full documentation

The file `labels.csv.gz` is a Gzip compressed file; to uncompress on unix-like
systems run

```
$ gunzip labels.csv.gz
```

More information about Gzip, including how to decompress on other systems, can
be found at https://www.gnu.org/software/gzip/ .

This will produce a file `labels.csv`, which is a CSV file with header and the
schema provided in the Examples section above or in the README file in more detail.


## Join the HighResolutionSettlementLayer community
* Website: https://dataforgood.facebook.com/dfg/tools/high-resolution-population-density-maps
* Facebook page: NA 
* Mailing list: NA
* irc: NA 

See the [CONTRIBUTING](CONTRIBUTING.md) file for how to help out.

## License
HighResolutionSettlementLayer is MIT licensed, as found in the LICENSE file.