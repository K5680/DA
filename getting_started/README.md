# Install Anaconda (Ubuntu 16.04)

The simplest way to have python and all the libraries installed, is to install Anaconda.

Download the [install script](https://www.anaconda.com/download/#linux)

run the script: bash Anaconda-3-5.0.1-Linux-x86_64.sh 


> If you get an error while creating a new Jupyter project, change ownership:

> sudo chown -R yourname:yourname ~/.local/share/jupyter/ 


Set path to your jupyter files:

1. jupyter notebook --generate-conf

2. nano /home/USER/.jupyter/jupyter_notebook_config.py

3. uncomment line and add path *c.NotebookApp.notebook_dir = '/DIRtoYOURfiles'*

4. Save and restart jupyter



***
# Start here

Alkuosassa hyvin sanastoa (suomi/englanti) ja luku 1 perustietoa koneoppimisesta ja algoritmeista:

[Johdatus tekoälyn taustalla olevaan matematiikkaan](https://tim.jyu.fi/view/kurssit/tie/tiep1000/tekoaly-mat/moniste)

Python & numpy -ohjeita suomeksi + linkkejä:

[https://mycourses.aalto.fi/mod/book/view.php?id=238495](https://mycourses.aalto.fi/mod/book/view.php?id=238495)


Pandas basic operations:

[Working with Dataframes](http://www.gregreda.com/2013/10/26/working-with-pandas-dataframes/)

[Pandas data manipulation](https://www.analyticsvidhya.com/blog/2016/01/12-pandas-techniques-python-data-manipulation/)


Esimerkkejä notebookeissa:

[example_notebooks/](example_notebooks/)



***

# More tutorials to get started

[Python for ecologists (get started with python/jupyter/csv files/pandas)](http://www.datacarpentry.org/python-ecology-lesson/)

[10 minutes to pandas](http://pandas.pydata.org/pandas-docs/stable/10min.html)

[Pandas Cookbook](https://pandas.pydata.org/pandas-docs/stable/tutorials.html)

[Dataquest - Python/Numpy/Pandas tutorials, a browser IDE](https://www.dataquest.io/)

[A Complete Tutorial to Learn Data Science with Python from Scratch](https://www.analyticsvidhya.com/blog/2016/01/complete-tutorial-learn-data-science-python-scratch-2/)

> 'ipython notebook --pylab=inline' has deprecated, use Jupyter with '%pylab inline' on the first row.
>

[Basics of Jupyter Notebook and Python](https://datahub.packtpub.com/tutorials/basics-jupyter-notebook-python/)

[Missing data basics](https://pandas.pydata.org/pandas-docs/stable/missing_data.html)

[Simple visualization examples](https://www.analyticsvidhya.com/blog/2015/05/data-visualization-python/)

---

[Johdatus tekoälyyn (Helsingin yliopisto)](https://www.cs.helsinki.fi/webfm_send/933)

[Data science lectures (pdf)](https://github.com/cs109/2015/tree/master/Lectures)

[Deep-learning -seminaari suomeksi. Erityisesti luku 5 "Machine learning basics". (TUT PLA-79100 course for the book Deep Learning (2016) by Goodfellow et al.)](https://github.com/karmus89/deep-learning-seminaari)

[Introduction to Deep Learning (MIT videos)](http://introtodeeplearning.com/)

[Beginning neural networks (video)](https://www.youtube.com/watch?v=ZzWaow1Rvho)

[GeoPandas / visualizing shapes/maps etc.](http://geopandas.org/)

[Matplotlib tutorial](http://www.scipy-lectures.org/intro/matplotlib/matplotlib.html)

***


# Cheat Sheets

[Matplotlib colormaps](https://matplotlib.org/examples/color/colormaps_reference.html)

[Cheat Sheet for Exploratory Data Analysis in Python](https://www.analyticsvidhya.com/blog/2015/06/infographic-cheat-sheet-data-exploration-python/)

[Cheatsheet – Python & R codes for common Machine Learning Algorithms](https://www.analyticsvidhya.com/blog/2015/09/full-cheatsheet-machine-learning-algorithms/)

[Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)


***

# Datasets & open data

[Kaggle, The Home of Data Science & Machine Learning](https://www.kaggle.com/)

[A list of dataset repos](https://www.kdnuggets.com/datasets/index.html)

[UCI machine learning repository](http://archive.ics.uci.edu/ml/index.php)

[Earthquake data](https://earthquake.usgs.gov/earthquakes/feed/v1.0/csv.php)

[Shape files (maps etc)](http://www.naturalearthdata.com/downloads/50m-physical-vectors/)

[Grouplens](https://grouplens.org/datasets/serendipity-2018/)

---

[Liikenneviraston avoin data (LAM)](https://www.liikennevirasto.fi/avoindata/tietoaineistot/lam-tiedot)

[Avoindata.fi](https://www.avoindata.fi/fi)

[Lounaistieto, Lounais-Suomen avoin data](http://www.lounaistieto.fi/tietopalvelut/avoimet-aineistot/)

[European data portal](https://www.europeandataportal.eu/)

[Linkki, linkki.jyvaskyla.fi/info/kehittajille](http://linkki.jyvaskyla.fi/info/kehittajille)

[HSL](https://www.hsl.fi/avoindata)


***

# Algorithms explained

[Top 10 Data Mining Algorithms Explained (KDnuggets)](https://www.kdnuggets.com/2015/05/top-10-data-mining-algorithms-explained.html/)

[A Tour of Machine Learning Algorithms](https://machinelearningmastery.com/a-tour-of-machine-learning-algorithms/)

[https://www.cs.usfca.edu/~galles/visualization/Algorithms.html](https://www.cs.usfca.edu/~galles/visualization/Algorithms.html)

[visualgo.net/en - visualising data structures and algorithms through animation](https://visualgo.net/en)

*** 

# Tilastotieteen / data-analytiikan / matematiikan sanastot

[Tilastotieteen sanakirja: suomi–englanti](https://math.aalto.fi/opetus/sovtoda/sanastot/fi2en.html)

[Tilastotieteen ja todennäköisyyslaskennan englantilais–suomalainen sanasto](http://www.math.helsinki.fi/petrin/sanasto/tilastosanasto.html)

[Tiedon louhinnan menetelmät, suomi-englanti-sanasto](https://www.cs.helsinki.fi/u/ronkaine/tilome/sanasto.html)

[Johdatus tekoälyn taustalla olevaan matematiikkaan, sanasto](https://tim.jyu.fi/view/kurssit/tie/tiep1000/tekoaly-mat/moniste)

[Matematiikan verkkosanakirja](https://matematiikkalehtisolmu.fi/sanakirja/s.html)

***

# Misc

[Deep Traffic - a fun challenge for traffic optimization](https://selfdrivingcars.mit.edu/deeptraffic/)

[What is batch size in neural networks](https://stats.stackexchange.com/questions/153531/what-is-batch-size-in-neural-network#153535)

[Comparing supervised learning algorithms (and scaling)](http://www.dataschool.io/comparing-supervised-learning-algorithms/)

[What algorithms need feature scaling](https://stats.stackexchange.com/questions/244507/what-algorithms-need-feature-scaling-beside-from-svm#253440)

