# GPX to Heatmap Overview

I needed a way to generate heatmap for all my rides
* This is a fork of https://github.com/TomCasavant/GPXtoHeatmap
* I modified the code to include the abiity to filter GPX files by year(s)
* Added Click command option for --year. Please see examples below






## Usage

**Install Dependencies**

```bash
$ python3 -m pip install -r requirements.txt
```

#### Command:

Show help:
```bash
$ python3 heatmap.py --help
Usage: heatmap.py [OPTIONS]

Options:
  --output TEXT                   Specify the name of the output file. Defaults to `map`.
  --input TEXT                    Specify an input folder - this is where all your GPX files should be. Defaults to `gpx`.
  --filter [running|cycling|walking]
                                  Specify a filter type. Defaults to no filter
  --help                          Show this message and exit.
  --year                          Specify a year to filter the GPX files. Defaults to no year. Multiple years can be accepted
```

Examples:
```bash
$ python3 heatmap.py
$ python3 heatmap.py --input gpx --output map
$ python3 heatmap.py --input gpx --output map2 --year 2019
$ python3 heatmap.py --input gpx --output map3 --year 2019 --year 2020
```

#### Retrieving GPX Files

- Garmin exports [garminexport](https://github.com/petergardfjall/garminexport)
- Strava exports [Strava's instructions](https://support.strava.com/hc/en-us/articles/216918437-Exporting-your-Data-and-Bulk-Export)
- Covert FIT files to GPX [fit2gpx](https://github.com/dodo-saba/fit2gpx) 

