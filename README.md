## Find Habitable Exoplanets

We have used data from NASA Exoplanet Archive and more specifically the Kepler's KOI Table.

The node script:

- Creates a read stream using fs module.
- Parses the data from the stream using csv-parse library.
- Filters out non habitable exoplanets given certain criteria.

Planet habitability criteria:

- Exoplanet Archive Disposition is confirmed
- Insolation Flux > 0.36
- Insolation Flux < 1.11
- Planetary Radius < 1.6
