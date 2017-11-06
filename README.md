# DRILSDOWN
#### _Drawing Rich Integrated Lat-lon-time Samples from Datasets Online into Working Notebooks_
https://brianmapes.github.io/EarthCube-DRILSDOWN/

[(image: 4 panels Explaining DRILSDOWN concept)](https://raw.githubusercontent.com/brianmapes/EarthCube-DRILSDOWN/master/DRILSDOWN.strategy.2017-06-01.why.jpg)

# Get DRILSDOWN capabilities in **three tiers** of increasing complexity 

## 1. IDV only. Install The IDV on your screen machine, then use idv_teleport a template bundle to any place+time.
## 2. IDV *plus* install Jupyter, and have Notebooks interact with your IDV session. 
## 3. IDV+Jupyter, *plus* install RAMADDA on a server to curate the results of 1. & 2., and share out to the world.

----------------

### Tier 1. Teleporting the IDV to any place and time:
**Install** [The IDV](http://www.unidata.ucar.edu/downloads/idv/nightly/index.jsp){:target="_blank"} [and our recommended Plugin](https://www.rsmas.miami.edu/users/bmapes/MapesIDVcollection.html){:target="_blank"} on your screen machine. Learn the basics of interacting with The IDV, e.g. from [this ppt](http://weather.rsmas.miami.edu/repository/entry/get/IDV_intro_LMTmanual.pptx?entryid=dd95b65c-09a5-43a5-9f44-da5243e302f4){:target="_blank"}. 

- 1a. **Obtain** a template IDV bundle, with displays you like, drawn from a big aggregated dataset, [like this one](http://weather.rsmas.miami.edu/repository/entry/show/Reanalyses-satellite_forWikipedia.isl/RSMAS-UM+Repository+for+atm-ocean+data+and+its+science/The+Mapes+IDV+collection/IDV+Bundles/Case+study+templates/Reanalyses-satellite_forWikipedia?entryid=ec12b8ce-3ea2-4de9-a833-3f4f13aca23b&output=idv.islform){:target="_blank"}. It can then be teleported to your places & cases. For instance, to try out The IDV for some atmospheric data around heavy rain events, you can select a case from [this online atlas](http://www.rsmas.miami.edu/users/bmapes/HeavyRains_clickmaps/index.html){:target="_blank"}. 

- 1b. **Teleport by command line:** To use a command-line call to teleport your IDV bundle, you could clone a copy of [IDV_teleport.py](https://github.com/suvarchal/IDV_teleport). Follow the directions there, or type _python idv_teleport.py -h_ to get help. **Even easier:** run _pip install drilsdown_, and then _idv_teleport -h_ will be a direct command. 

### Tier 2. Add Jupyter notebooks to the mix
**Install** Jupyter notebooks on your screen machine, starting [here](https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/). You can learn more about Notebook technology from [Unidata](https://github.com/Unidata/unidata-python-workshop/blob/master/presentations/jupyter_notebook_2016.pdf){:target="_blank"}. 

- 2a. To use The IDV within iPython notebooks, follow the 4 steps [here](https://github.com/Unidata/ipython-IDV/blob/master/README.md#ipython-idv){:target="_blank"}. From the Notebook, you will launch an IDV instance and communicate with it from within the Notebook environment, capturing images and animations into the Notebook, and connecting The IDV's data and display capabilities to your other Python computations. It is clearest to start from an example .ipynb file, like this one.  

- 2b. To work with The IDV from a Jupyter notebook with a Jython kernel (one of IDV's native languages), install [JyIDV](https://github.com/suvarchal/JyIDV), culminating in the command line call of _python setup.py install_. Follow and extend the example notebooks you can find there. 


### Tier 3. Run your own RAMADDA server
#### Perhaps you see the power of RAMADDA from Tiers 1 and 2 and want to operate your own RAMADDA, so you can publish to it, and with it, moving beyond just fetching goodies from someone else's. 

**Install** [RAMADDA](http://geodesystems.com/repository/entry/show?entryid=2e485e95-eb29-44fc-8987-76e6ac74365a){:target="_blank"} on your networked server (or in fact, it can run on your laptop or screen machine too). Among its many other functions, RAMADDA can be used to serve out gridded numerical datasets suitable for IDV access from anywhere. It can also publish and curate [IDV bundles](http://weather.rsmas.miami.edu/repository/entry/show?entryid=115a4ff0-10de-4fba-86d7-66cd42d6d8de){:target="_blank"}, and publish and render [Jupyter notebooks](http://dataloggia.com/repository/entry/show?entryid=3552f8c0-a3af-4531-9339-9d420a437835){:target="_blank"}.

Obtain the DRILSDOWN [plugin for RAMADDA](https://github.com/Unidata/ipython-IDV/blob/master/README.md#setting-up-your-own-ramadda-to-handle-drilsdown-case-study-objects){:target="_blank"} to gain extra services. Special for DRILSDOWN is an entry type called a [_case study_ like this](http://geodesystems.com/repository/entry/show?entryid=12704a38-9a06-4989-aac4-dafbbe13a675){:target="_blank"}. This digital object (symbolized by a briefcase icon) can contain meaningfully linked-together sets of notebooks, IDV bundles, and pre-made images, as well as metadata tags. Your content can be accessed from anywhere, and new services can be developed within RAMADDA to operate on whatever sorts of materials and data you may store in sufficiently-similar Case Studies. 
