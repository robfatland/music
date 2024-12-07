music? sure! See the **[tunes](https://github.com/robfatland/reorganiseduponthefloor/tree/main/tunes)** folder.


  
# [reorganised](https://github.com/robfatland/reorganiseduponthefloor/blob/main/sweeney.md)

map robfatland github repos, plus music

Reference: How to create a table in markdown:


| Activity | Amount |  Date | Notes |
| -------- | ------ | ---- | ---- |
| indicators |
| scale | roof |  03-AUG-2018 | 1.2 |




## [github.com/robfatland](https://github.com/robfatland), a dubious organization


### Research and Outreach

* Research folder -- consolidate to two (golive and ocean)
   * galleryclone: source material
   * cormorack: source material
   * chlorophyll: source material
   * notebooks: source material
   * rpy
   * golive is most advanced terrestrial cryosphere
   * ocean is most current, see?
* Outreach
   * mocean
   * othermathclub (consolidate with percival and boojum)
   * pythonbytes (consolidate with othermathclub / percival / boojum)
   * boojum (carry to othermathclub)
   * percival (carry to othermathclub)
   * genomics (delete after check on value)


### practical cloud


* cli: expand
* nlp: bring to usable state
* costnotify
* cloudsecurity
* cloud101102: check and delete
* Zero2API: update
* serverless: check
* greenandblack: catch-all, some material should go elsewhere
    * describes using gh-pages


### miscellaneous


* ops
    * Older version of organization effort.
    * Action: Integrate here, delete.
* flying bosun
    * notes on salmon fishing


- whither these?
    - cloudmaven
    - Port Cormorack
    - whaledr
    - research2cloud
    - escience-pangeo
    - eScience

### CloudBank

* [cb-resources](https://github.com/cloudbank-project/cb-resources) is resources **base**
    * [public view cb-resources](https://cloudbank-project.github.io/cb-resources/)
    * [markdown location for CloudBank Solutions](https://github.com/cloudbank-project/cb-resources/tree/main/docs/technical-resources/solutions)
    * [Template: **cbs-jupyter.md**](https://github.com/cloudbank-project/cb-resources/blob/main/docs/technical-resources/solutions/cbs-jupyter.md)
    * To inline images follow this procedure
        * Create `README.md` in a sub-folder called `cbs-topic-name-here-static` and copy contents in from `README.md` in `cbs-jupyter-static` 
        * Upload images to this folder
        * Create image inline markdown in `cbs-topic-name-here.md` as shown below

```
![Binder as sandbox Jupyter notebook server](cbs-jupyter-static/jupyter_binder_notebook_listing.png)
```

## More referentials

* [Oncorhynchus](http://github.com/robfatland/flyingbosun))
* [pangeo outreach education and training (POETs)](https://github.com/pangeo-data/education-material)
* NASA [Common Metadata Repository (CMR)](https://github.com/pangeo-data/cmr)
* [pangeo binder](http://binder.pangeo.io)
* [pangeo Jupyter Hub](https://nasa.pangeo.io)
* [jupyter-earth](https://github.com/pangeo-data/jupyter-earth)
* [my GOLIVE](https://github.com/robfatland/golive)
* [RCA](http://app-dev.ooica.net) and [Interactive Oceans](https://interactiveoceans.washington.edu)
    * Sort these...
        * [synoptic](https://github.com/robfatland/synoptic)
        * [cormorack](https://github.com/robfatland/cormorack)
        * [chlorophyll](https://github.com/robfatland/chlorophyll)
        * [notebooks](https://github.com/robfatland/notebooks)
        * [galleryclone](https://github.com/robfatland/galleryclone)
        * [a cormorack-organization version of the notebook gallery](http://github.com/cormorack/gallery) 
        * artifact work on [whalebooks](http://github.com/cormorack/whalebooks) (more below)
        * [megaptera](http://github.com/whaledr/whalebooks) Making whales -- specifically humpbacks -- accessible via broadband hydrophone
        * [the megaptera *game*](http://megaptera.swipesforscience.org/#/) 
        * [bio-acoustic transfer learning (batl)](https://github.com/pshivraj/batl)
* ***Medicine*** [aggregate material on secure digital research environments](https://github.com/robfatland/uwsdre) 
    * repo 'sce' should be folded into here ^
    * repo 'cloudsecurity' (for CB) also ^
* ***Data science, with emphasis on using the public cloud***
    * Lightweight data systems; we abbreviate with [Zero2API](https://github.com/robfatland/Zero2API)
    * A cost notification Lambda function called [costnotify](https://github.com/robfatland/costnotify)
    * [Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/)
    * [Apache Spark](https://spark.apache.org/documentation.html) 
        * Described at ([Wikipedia](https://en.wikipedia.org/wiki/Apache_Spark))
        * Also alternatives must arise, such as [BlazingSQL](https://docs.blazingdb.com)
    * [Transfer Learning (CNN)](https://github.com/pshivraj/batl)
    * [Cloud 101 / 102 work circa 2019](https://github.com/robfatland/cloud101102)
    * [Article of interest](https://hai.stanford.edu/news/the_intertwined_quest_for_understanding_biological_intelligence_and_creating_artificial_intelligence/)

* [PythonBytes, a middle-school coding club](https://github.com/robfatland/pythonbytes)
* [The Other Math Club](https://github.com/robfatland/othermathclub)
* [A snarky start on some number theory](https://github.com/robfatland/boojum)
* Can use `environment.yml` or `requirements.txt`
    * The latter is associated with `pip install` and can be made a sub-component of the former
    * `environment.yml` as follows
        * `conda env export` produces `environment.yml`
    * `requirements.txt` as follows
        * Create a virtual environment `python3 -m venv /path/to/new/virtual/env`
        * Install packages using `pip install <package>`
        * Save all packages `pip freeze > requirements.txt`
        * "Pin all the package versions"... not sure what the action is or what this means
        * Move `requirements.txt` to the root directory of the project

