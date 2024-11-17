Astronomy Picture of the Day
============================

From 2007 until shortly into Musk's ownership of Twitter (as was) I created and ran the @apod Twitter feed as well as providing an [APOD Search](https://strudel.org.uk/apod/). To do this I created a database of the text explanations for every Astronomy Picture of the Day. These are parsed from the original web pages. At the same time I parsed the text to identify likely astronomical objects and piped those through ~[LookUp](http://www.strudel.org.uk/lookUP/)~ to find their Right Ascension/Declination and types (using the [AVM](http://www.virtualastronomy.org/avm_metadata.php) classification). The results go into a large [JSON-LD](http://json-ld.org/) file.

Contents
--------

For each entry you'll get:
* id - The URL
* date - A YYYY-MM-DD date string
* title - The title
* image - The URL of the image
* thumb - The URL of the thumbnail image
* media - [optional] The URL when the image isn't an image. This could be a link to YouTube, Vimeo, a Flash file etc.
* text - The escaped HTML for the description of the entry.
* credit - The escaped HTML for the credit line.
* objects - [optional] An array of extracted objects. Each one contains:
  * name - The name of the astronomical object
  * ra - The Right Ascension
  * dec - The Declination
  * category - An array of AVM (Astronomy Visualization Metadata) categories (see http://www.virtualastronomy.org/AVM_DRAFTVersion12_rlh02.pdf) for the object.


Credits
-------

All the explanations come from [APOD](http://apod.nasa.gov/) so please make sure you credit them if you use this (e.g. `APOD is created by Robert Nemiroff (MTU) & Jerry Bonnell (UMCP)`). If you can credit me too that would be wonderful.

~Note that the classification of objects and their coordinates comes from [LookUP](http://www.strudel.org.uk/lookUP/). LookUP gets data from [SIMBAD](http://simbad.u-strasbg.fr/simbad/) (operated at CDS, Strasbourg, France), the [NASA/IPAC Extragalactic Database](http://nedwww.ipac.caltech.edu/) (NED; operated by the Jet Propulsion Laboratory, California Institute of Technology, under contract with the National Aeronautics and Space Administration), the [SkyBoT project](http://www.imcce.fr/page.php?nav=webservices/skybot/) (set up under the auspice of the French Ministry for National Education and CNRS), the [Extrasolar Planets Encyclopedia](http://exoplanet.eu/) (Jean Schneider, CNRS/LUTH - Paris Observatory), the [Central Bureau for Astronomical Telegrams Supernovae List](http://www.cbat.eps.harvard.edu/lists/Supernovae.html) (IAU, Smithsonian Astrophysical Observatory), the [Royal Astronomical Society of Canada Constellation List](http://calgary.rasc.ca/constellation.htm) (Larry McNish), the [SDSS SkyServer](http://cas.sdss.org/astro/en/), the [Minor Planet & Comet Ephemeris Service](http://www.cfa.harvard.edu/iau/MPEph/MPEph.html) ([IAU Minor Planet Center](http://www.cfa.harvard.edu/iau/mpc.html)), and the excellent [WCSTools package](http://tdc-www.harvard.edu/software/wcstools/) ([Doug Mink](http://tdc-www.harvard.edu/mink/), Smithsonian Astrophysical Observatory).~