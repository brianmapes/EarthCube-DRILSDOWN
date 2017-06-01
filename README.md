# DRILSDOWN
#### _Drawing Rich Integrated Lat-lon-time Samples from Datasets Online into Working Notebooks_

![4 panels Explaining DRILSDOWN concept](https://raw.githubusercontent.com/brianmapes/EarthCube-DRILSDOWN/master/DRILSDOWN.strategy.2017-06-01.why.jpg)

# Get DRILSDOWN capabilities in **three tiers**, of increasing complexity 

## 1. Install The IDV on screen machine, teleport a template, study visualizations.
## 2. As above, plus install Jupyter Notebooks to interact with your IDV sessions. 
## 3. As above, plus install RAMADDA on a server, to curate the results of 1. & 2. and to serve out datasets.

----------------

### Tier 1. Teleporting with the IDV
**Install** [The IDV and a Plugin](https://www.rsmas.miami.edu/users/bmapes/MapesIDVcollection.html) on your screen machine, and learn the basics of interacting with it, e.g. from [this ppt](http://weather.rsmas.miami.edu/repository/entry/get/IDV_intro_LMTmanual.pptx?entryid=dd95b65c-09a5-43a5-9f44-da5243e302f4). 

- 1a. To try out The IDV for some atmospheric data around heavy rain events, you can select a case from [this online atlas](http://www.rsmas.miami.edu/users/bmapes/HeavyRains_clickmaps/index.html). 

- 1b To teleport one of our RAMADDA-stored templates [like this one](http://weather.rsmas.miami.edu/repository/entry/show?entryid=ec12b8ce-3ea2-4de9-a833-3f4f13aca23b) to your places & cases. To constuct Python command-line calls that will teleport an IDV bundle, clone a copy of [IDV_teleport.py](https://github.com/suvarchal/IDV_teleport) and follow the directions.  

### Tier 2. Add Jupyter notebooks
**Install** Jupyter, part of [Anaconda](https://www.continuum.io/downloads), on your screen machine, and learn the basics of interacting with notebooks. 

- 2a. To use iPython notebooks, get a copy of [drilsdown.py](https://raw.githubusercontent.com/Unidata/ipython-IDV/master/drilsdown.py) and put it in your _.ipython/extensions_ file in your home directory. Then within a notebook, invoking the magic _%reload_ext drilsdown_ will unlock tha ability to launch and communicate with The IDV from within the Notebook environment. See one of our template notebooks like [this one](http://geodesystems.com/repository/entry/show?entryid=8f7cfb7e-aba1-4b8f-878c-65b525aee169) for examples of the available commands.  

- 2b. Alternately, install the Jython kernel for JuPyter, [JyIDV](https://github.com/suvarchal/JyIDV), culminating in the command _python setup.py install_. Follow and extend the example notebooks there. 


### Tier 3. Add your own RAMADDA server
**Install** [RAMADDA](http://geodesystems.com/repository/entry/show?entryid=2e485e95-eb29-44fc-8987-76e6ac74365a) on your networked server (or in fact, it can run on your laptop or screen machine too). Among its many other functions, RAMADDA can be used to serve out gridded numerical datasets suitable for IDV access from anywhere. It can also publish and curate [IDV bundles](http://weather.rsmas.miami.edu/repository/entry/show?entryid=115a4ff0-10de-4fba-86d7-66cd42d6d8de), and publish and render [Jupyter notebooks](http://dataloggia.com/repository/entry/show?entryid=3552f8c0-a3af-4531-9339-9d420a437835).

Obtain the DRILSDOWN [plugin for RAMADDA](https://github.com/Unidata/drilsdown) to gain extra services. Special for DRILSDOWN is an entry type called a [_case study_](http://geodesystems.com/repository/entry/show?entryid=12704a38-9a06-4989-aac4-dafbbe13a675), which can contain meaningfully linked-together groups of notebooks, IDV bundles, and pre-made images. Your content can be accessed from anywhere, and new services can be integrated within RAMADDA to operate on whatever sorts of materials and data you store there. 
