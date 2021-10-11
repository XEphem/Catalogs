# XEphem Catalogs

The star catalogs in this repository are for the
[XEphem](https://xephem.github.io/XEphem/Site/xephem.html) serious
interactive astronomical software ephemeris.

## Official

* `GSC2201/` — The 1.3 GB Hubble Guide Star Catalog 2.2.0.1 which
  includes stars in the magnitude range 10.0–18.5.  Though traditionally
  installed at `/usr/local/xephem/catalogs/GSC2201`, you can install the
  catalog anywhere as long as you enter its path in the “GSC 2.2
  Directory” field in XEphem’s “Field Stars” window.  See the Reference
  Manual’s [Field
  Stars](https://xephem.github.io/XEphem/Site/help/xephem.html#mozTocId147305)
  section for more details.

* `Official/` — Large collection of catalogs (weighing a total 328 MB)
  that, in the old days, shipped with XEphem on its installation media.
  Most of the catalogs are in the `.edb` text format, though two are in
  the binary `.xe2` format.
  
* `usno/` — The USNO-SA2.0 catalog, a sub-sampled version of the
  USNO-A2.0 catalog. It contains only a tenth as many stars as the parent
  catalog (54,787,624 stars in 634 MB). The goal was to provide a spatially
  uniform distribution of stars in an intermediate range of magnitudes.
  There are about 1,300 stars per square degree of sky. Note that such a
  uniform distribution does not look much like the real sky, but is
  intended for use as a "reference grid" for comet or asteroid hunters, etc.
  Though traditionally installed at `/usr/local/xephem/catalogs/usno`, you
  can install the catalog anywhere as long as you enter its path in the
  “USNO A or SA catalogs - Root directory” field in XEphem’s “Field Stars”
  window. This is an updated version with the previously missing sky zones
  added.

## User contributed

Three catalogs have been contributed by Steve Mencinsky:

* `M31globulars.edb` — a list of principle globular clusters in galaxy M31.

* `SMC.edb` — a list of deep sky objects in the Magellanic Clouds.

* `recons100.edb` — is the complete census as of January 1, 2000, of
  objects outside our solar system known within 10 parsecs.
