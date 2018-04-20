# Demonstration of Jupyter notebook deployed with Binder
## Smithsonian Volcanoes of the World (VOTW)


A while back (2014!) I made a [blog post](https://scottyhq.github.io/blog/2014/02/08/mapping-volcanic-eruptions/) that used a Jupyter Notebook to create a nice map of Volcanic Eruptions. There were some nice demonstrations, but the code was not reproducible because it used a csv file sitting on my computer. A lot has changed since I posted that notebook - there are great alternative Python libraries, and tools such as [Conda](https://conda.io/docs/), [Docker](https://www.docker.com/community-edition), and [Binder](https://mybinder.org), which enable others to reproduce and modify the analysis.

This repository contains a modernized reproducible blog post (hopefully it continues to be in 4 more years!) 

Launch an interactive jupyter notebook by clicking on the binder button
[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/scottyhq/votw/master)

Or clone this repository to run locally
```
git clone https://github.com/scottyhq/votw.git
cd votw
conda env create -f votw.yml
jupyter notebook
```

## Credit where credit is due
The Smithsonian Global Volcanism Program has released some great tools recently, including a GeoServer to query data programmatically:
http://volcano.si.edu/database/webservices.cfm 

Examples on how to do this with python are here:
http://geopython.github.io/OWSLib/#wfs

And a neat web viewer:
https://volcano.si.edu/E3/

But you can also select options online and download results in Excel format:
https://volcano.si.edu/search_eruption.cfm#

Compiling and curating databases is no small task! Here is the citation for the VOTW database:

```
Global Volcanism Program, 2013. Volcanoes of the World, v. 4.6.7. Venzke, E (ed.). Smithsonian Institution. Downloaded 18 Apr 2018. https://dx.doi.org/10.5479/si.GVP.VOTW4-2013
```
