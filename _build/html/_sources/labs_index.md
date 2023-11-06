# 💻 Labs

```{admonition} Table of Contents! 👇🏽
:class: dropdown
1. [Lab 0: Tools](lab-0)
2. [Lab 1: Tidy Data](lab-1)
3. [Lab 2: Data Engineering](lab-2)
4. [Lab 3: Geo-Visualisation](lab-3)
5. [Lab 4: Networks and Spatial Weights](lab-4)
6. [Lab 5: Linear Regression](lab-5)
7. [Lab 6: Clustering](lab-6)
8. [Lab 7: Points](lab-7)
```

```{tip}
*DOWNLOAD ALL THE LABS*

You can download all the labs, associated datasets, html files showing the output of the labs, and homework notebooks using the links below.
```

***

(lab-0)=
## Lab 0 - Tools

- [lab-0](labs/lab-00.zip)

**IMPORTANT** This is a supplementary notebook that covers many basics of the tools we will use in the course but does not explain anything directly related to Spatial Data Science.

Students are encouraged to read it before getting started with the other notebooks and then keep it as a reference throughout the rest of the course. There are some basic Python operations in there that act as a refresher, practice or learning material, if you may need it.

### Extra Material

If you want to explore further by yourself the contents presented in this tutorial, the following pointers are good places to start:

* Gallery of [interesting notebooks](https://github.com/jupyter/jupyter/wiki): a wealth of examples of Jupyter (formerly called IPython) notebooks.
* (Downey, 2012): very good general introduction to Python as a programming language and to the algorithmic way of thinking. The book is freely available in [HTML](http://www.greenteapress.com/thinkpython/html/index.html) and [PDF](http://www.greenteapress.com/thinkpython/thinkpython.pdf).

***

(lab-1)=
## Lab 1 - Tidy Data

- [lab-1](labs/lab-01.zip)

### Data

This session uses the **"Census socio-demographics"** dataset of The Hague, Netherlands and Liverpool, United Kingdom in two parts. The dataset for this lab is provided in the zipped lab files above.

1. Table of neighbourhoods called Buurten areas in The Hague with population counts by World region and Age groups. The table is derived from the denhaagcijfers dataset.
2. Table of LSOA areas in Liverpool with population counts by World region. The table is derived from the CDRC Census data pack.
3. Collection of socio-demographic characteristics from the 2011 Census for the city of Liverpool.

### Extra Material

* **[Visualization]** Python library `seaborn` [tutorial](http://stanford.edu/~mwaskom/software/seaborn/tutorial.html).
* [NY Times article](http://www.nytimes.com/2014/08/18/technology/for-big-data-scientists-hurdle-to-insights-is-janitor-work.html?_r=0) about the importance of cleaning data.


***

(lab-2)=
## Lab 2 - Data Engineering

- [lab-2](labs/lab-02.zip)

### Data

This session uses two datasets which are provided in the zipped lab files above.

1. A dataset about wines from different countries, download from **Kaggle**.
2. A dataset scraped and collected from **Goodreads**.


***

(lab-3)=
## Lab 3 - Geo-Visualisation

- [lab-3](labs/lab-03.zip)

The homework exercises are embedded within the lab files itself. You have to complete the exercises as you go along understanding the rest of the code. There are two files for this lab, ``geovis`` and ``eda``. Since this geocomputational lab is not as straightforward as other python code, a **solution set** is also provided for questions indicated in the lab.

### Data

This session uses multiple datasets which are provided in the zipped lab files above.

1. A **"Census socio-demographics"** dataset as well as the Ordnance Survey **(OS) Geodata Pack**.
2. An **"Index of Multiple Deprivation""** dataset as well as the Ordnance Survey **(OS) Geodata Pack**.
Scores, ranks, and components of the 2015 Index of Multiple Deprivation (IMD).
**Source**: [CDRC](http://cdrc.ac.uk/)'s English Indices of Deprivation 2015 Geodata Pack for the city of Liverpool (UK).
3. Additionally, you will need the raster file for the basemap of Liverpool. This has been assembled by [Dani Arribas-Bel](http://darribas.org) from the [OS VectorMap District (Backdrop Raster)](https://www.ordnancesurvey.co.uk/business-and-government/products/vectormap-district.html), and it is licensed as OpenData.
4. Simple datasets on ``heart diseases``, ``titanic`` and a ``mystery`` are also provided.

### Extra Material

* A good introduction to the `geopandas` project is provided by Kelsey Jordahl, the project's founder in this [set of slides](http://kjordahl.github.io/SciPy-Tutorial-2015/#1) from a 2015 talk and the companion [repository](https://github.com/kjordahl/SciPy-Tutorial-2015).
* An additional great resource is this 4h. [workshop](https://github.com/carsonfarmer/python_geospatial) by Carson Farmer.


***

(lab-4)=
## Lab 4 - Networks and Spatial Weights

- [lab-4](labs/lab-04.zip)

### Data

This session uses multiple datasets which are all provided in the zipped lab files above.

1. An **"Index of Multiple Deprivation""** dataset used in previous labs.
2. A **Brexit** dataset.

The Brexit dataset is of the results of the 2016 referendum vote to leave the EU, at the local authority level. All the necessary data have been assembled for convenience in a single file that contains geographic information about each local authority in England, Wales and Scotland, as well as the vote attributes. The file is in the modern geospatial format [GeoPackage](http://www.geopackage.org/), which presents several advantages over the more traditional shapefile (chief among them, the need of a single file instead of several).

The source data used to compile the file linked above include:

- Electoral Commission data on the EU referendum results ([`url`](https://www.electoralcommission.org.uk/find-information-by-subject/elections-and-referendums/past-elections-and-referendums/eu-referendum/electorate-and-count-information))
- Local Authority District boundaries (archived, not available online anymore)


***

(lab-5)=
## Lab 5 - Linear Regression

- [lab-5](labs/lab-05.zip)

Since this lab is not as straightforward as other python code, a **solution set** is provided for questions indicated in the lab and homework. It is better if you try yourself and get feedback from your peers, and then look at the solutions.

### Data

This session uses multiple data files.

1. A dataset downloaded from Kaggle on stats about the premiere league.
2. A Boston housing dataset and its training set companion.
3. An IMDB cast dataset.
4. A car dataset.
5. A cab dataset.

These sets are not that relevant to global urban issues but simple to work with on small regression practice sets.


***

(lab-6)=
## Lab 6 - Clustering

- [lab-6](labs/lab-06.zip)

### Data

This session uses the **"AirBnb listing for Inner London - MSOA level"** dataset.

This dataset contains information for [AirBnb](https://www.airbnb.com) properties for the area of Inner London aggregated at the MSOA level. It has been prepared by Dani Arribas-Bel using as the original source the full listing of AirBnb locations for London provided by [Inside AirBnb](http://insideairbnb.com/). Same as the source, the dataset is released under a [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) License.

For every polygon, the following variables are provided:

* `id`: MSOA unique identifier.
* `accommodates`: average property capacity in the MSOA.
* `bathrooms`: average number of bathrooms in the properties within the MSOA.
* `bedrooms`: average number of bedrooms in the properties within the MSOA.
* `beds`: average number of beds in the properties within the MSOA.
* `number_of_reviews`: average number of reviews received by the properties within the MSOA.
* `reviews_per_month`: average number of reviews per month received by the properties within the MSOA.
* `review_scores_ratings`: average rating score received by the properties within the MSOA.
* `review_scores_accuracy`: average accuracy score received by the properties within the MSOA.
* `review_scores_cleanliness`: average cleanliness score received by the properties within the MSOA.
* `review_scores_checkin`: average checkin score received by the properties within the MSOA.
* `review_scores_communication`: average communication score received by the properties within the MSOA.
* `review_scores_location`: average location score received by the properties within the MSOA.
* `review_scores_value`: average value score received by the properties within the MSOA.
* `property_count`: total number of AirBnb properties listed withing the MSOA.

The lab also uses an additional file that contains the boundary lines of the London boroughs provided in the data folder as well.

### Extra Material

* The documentation for [`scikit-learn`](http://scikit-learn.org), a world-class Python library for machine learning, is excellent and includes many examples that cover the entire functionality set of the library.

***

(lab-7)=
## Lab 7 - Points

- [lab-7](labs/lab-07.zip)

### Data

This lab uses a sample of geo-referenced locations of photographs taken in Tokyo.

### Extra Material

* A very good resource for kernel density estimation in Python is provided in [this blog post](https://jakevdp.github.io/blog/2013/12/01/kernel-density-estimation/) by Jake Vanderplas.
