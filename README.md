# GPX to Heatmap Overview
I modified the code to include the ability to filter GPX files by years. 
Click command option to include --year. Please see examples below.

This is a fork of https://github.com/TomCasavant/GPXtoHeatmap



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
  --output TEXT                   Specify the name of the output file.
                                  Defaults to `map`
  --input TEXT                    Specify an input folder. Defaults to `gpx`
  --filter [running|cycling|walking]
                                  Specify a filter type. Defaults to no filter
  --help                          Show this message and exit.
  --year                          Specify y a filter type. Defaults to no year. Multiple years can be accepted
```

Examples:
```bash
$ python3 heatmap.py
$ python3 heatmap.py --input gpx --output map
$ python3 heatmap.py --input gpx --output map2 --year 2019
$ python3 heatmap.py --input gpx --output map3 --year 2019 --year 2020
```

#### Retrieving GPX Files

- Garmin users can use [garminexport](https://github.com/petergardfjall/garminexport) to export GPX data.
- Strava users can follow [Strava's instructions](https://support.strava.com/hc/en-us/articles/216918437-Exporting-your-Data-and-Bulk-Export) to export GPX data
- Convert Fit files into GPX [fit2gpx](https://github.com/dodo-saba/fit2gpx) 

