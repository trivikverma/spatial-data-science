# 🧐 Lectures

```{admonition} Table of Contents! 👇🏽
:class: dropdown

1. [Lecture 1: Spatial Data Science](L1)
2. [Lecture 2: Spatial and Urban Data](L2)
3. [Lecture 3: Data Grammar](L3)
4. [Lecture 4: Data Engineering](L4)
5. [Lecture 5 EDA and Visualisation:](L5)
6. [Lecture 6: Geo-Visualisation](L6)
7. [Lecture 7: Networks and Spatial Weights](L7)
8. [Lecture 8: Exploratory Spatial Data Analysis](L8)
9. [Lecture 9: Machine Learning for Everyone](L9)
10. [Lecture 10: Anatomy of a Learning Algorithm](L10)
11. [Lecture 11: Clustering](L11)
12. [Lecture 12: Dimensionality Reduction](L12)
13. [Lecture 13: Spatial Density Estimation](L13)
14. [Lecture 14: Responsible Data Science](L14)
```

```{tip}
*A GUIDE TO FOLLOW THIS PAGE*

- The slides will be updated latest a night before the lecture in **pdf** format.
- Lectures will not be recorded or delivered online.
- The section **To do before class** provides content that is useful for following the lectures. I expect you to follow it before every lecture. It will take about 1 hour of prep at home.
- Section **Extra Material** is exactly extra. It is **not required** for this course but can prove really helpful for gaining extra knowledge either during or after this course. Sometimes I use it to build the contents of the lecture and at others I find them helpful in my research related to the weekly topics but I will never question your knowledge on that.
```

***

# Let's begin

Before starting the course, watch [this video](https://www.youtube.com/watch?v=8jqEj8XUPlk&t=80s) by Khalid Kadir about a reflection on poverty (an example of a social problem), expertise and equity. This representation is an example of how experts create boxes around their craft. As a data scientist or a future expert (consultant, data analyst, policymaker, etc.), it is our responsibility to step out of those boxes and engage with communities to strive for just outcomes. If you have seen this video, send me a meme about poverty, inequality and data. The best submission will win a prize at the end of the course.

<iframe width="560" height="315" <iframe width="560" height="315" src="https://www.youtube.com/embed/8jqEj8XUPlk" frameborder="0" allowfullscreen></iframe>

***

(L1)=
## Lecture 1 - Spatial Data Science

- [pdf](lectures/01-introduction.pdf)

### To do before class [Takes about 1 hour of prep at home]

As a way to whet your appetite about the content of the first class, I recommend you:

* Listen to [this interview](http://www.sciencefriday.com/segments/solving-lifes-everyday-problems-with-data/) with Hilary Mason, Max Shron, and Alex Pentland about the power of data.

* Watch [this video](https://www.youtube.com/watch?v=h1ImEQKSkUQ) by Mike Flowers, Chief Analytics Officer, at the City of New York about how data is used to influence policy decisions.

* Read [What New Yorkers are complaining about](https://www.wired.com/2010/11/ff_311_new_york/) and reflect on [if the cost of running such data systems worth the price of knowing?](https://www.governing.com/topics/urban/gov-311-systems-cost.html)

### Extra Material [Always to learn more but never needed for the course]

* "Chapter 1: Introduction" (Schutt & O’Neil, 2013). Free sampler of the book containing the chapter available online ([html](http://shop.oreilly.com/product/0636920028529.do), [pdf](http://cdn.oreillystatic.com/oreilly/booksamplers/9781449358655_sampler.pdf)).
* Read this critical argument about objectivity and positionality: [How Does Your Positionality Bias Your
Epistemology?](https://repository.uclawsf.edu/cgi/viewcontent.cgi?article=2260&context=faculty_scholarship)
* A Geographic take on Data Science, proposing a new field called [Geographic Data Science](https://doi.org/10.1111/gean.12194)
* Read this short critical piece called [Making Space in Geographical Analysis](https://doi.org/10.1111/gean.12325)

***

(L2)=
## Lecture 2 - Spatial and Urban Data

### Slides

- [pdf](lectures/02-data.pdf)

### To do before class [Takes about 1 hour of prep at home]

* Watch the [TED talk](https://www.youtube.com/watch?v=CijsvAGU6-c) by Carlo Rati about MIT's SENSEable City Lab projects: excellent set of examples
* Read the [New York Times piece](https://www.nytimes.com/interactive/2018/10/12/us/map-of-every-building-in-the-united-states.html) on US buildings map
* Explore the [Global Human Settlement Layer](https://ghsl.jrc.ec.europa.eu/index.php) Dataset, by the European Commission

### Extra Material [Always to learn more but never needed for the course]

* The part of the lecture on new sources of data relies on [Arribas-Bel, 2014](https://doi.org/10.1016/j.apgeog.2013.09.012) and [Lazer & Radford, 2017](https://doi.org/10.1146/annurev-soc-060116-053457).
* A classic on the rise of [volunteered geographic information](https://doi.org/10.1007/s10708-007-9111-y).

***

(L3)=
## Lecture 3 - Data Grammar

### Slides

- [pdf](lectures/03-grammar.pdf)

### To do before class [Takes about 1 hour of prep at home]

* Read a very influential pro-big data/data science article, [The End of Theory](https://www.wired.com/2008/06/pb-theory/) by Chris Anderson, the editor in chief of _Wired_.
* Read [A reflexive call of caution](https://science.sciencemag.org/content/343/6176/1203) on Big Data Analytics by David Lazer _et al._
* Read [Creating healthy and sustainable cities: what gets measured, gets done ](https://doi.org/10.1016/s2214-109x(22)00070-5).

### Extra Material [Always to learn more but never needed for the course]

* A cheatsheet (such a misnomer -- nobody is cheating and it is a helpful and beautiful resource) on [Data Wrangling with Pandas](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf) that you may want to stick to your wall or put as your screensaver to save time on finding useful and operational codes.

***

(L4)=
## Lecture 4 - Data Engineering

### Slides

- [pdf](lectures/04-engineering.pdf)

### To do before class [Takes about 1 hour of prep at home]

* Read a short blog on [Why, How and When to Scale your features](https://medium.com/greyatom/why-how-and-when-to-scale-your-features-4b30ab09db5e)

### Extra Material [Always to learn more but never needed for the course]

The contents of this lecture are loosely based on, and explored into further detail, in the following two references :

* Section 9.3.1 of [The Hundred-Page Machine Learning Book](https://leanpub.com/theMLbook) by Andriy Burkov.
* A more academically suited blog on [Feature Scaling](https://sebastianraschka.com/Articles/2014_about_feature_scaling.html)


***

(L5)=
## Lecture 5 - EDA and Visualisation

### Slides

- [pdf](lectures/05-visualisation.pdf)
- [Beautiful visualisations](lectures/AYearInGraphicDetail.zip)
- [Principles of Graphical Excellence and other things..](lectures/ExtraReading.zip)

### To do before class [Takes about 1 hour of prep at home]

* [Think about the grammar of graphics when improving your graphs](https://medium.com/tdebeus/think-about-the-grammar-of-graphics-when-improving-your-graphs-18e3744d8d18) - at _Colourful Facts_ – a Medium blog by Thomas de Beus. Ignore the reference to the **R** programming language as this course is based on **Python** (no offence intended to any community, R is the best for visualisation though).
* Learn about [Kernel Density Estimation](https://mathisonian.github.io/kde/)

### Extra Material [Always to learn more but never needed for the course]

* Berinato, S. [Visualisations That Really Work](https://hbr.org/2016/06/visualizations-that-really-work), Harvard Business Review, Jun 2016
* Alberto Cairo's weblog called [The Functional Art](http://www.thefunctionalart.com/) about information design, and visualisation is an excellent resource for improving your visualisations.
* (Yau, 2011)’s book ["Visualize this"](http://flowingdata.com/visualize-this/)
  is a good general introduction to visualisation.
* Check out [From Data to Vis](https://www.data-to-viz.com/) chart selector for selecting the right charts

***

(L6)=
## Lecture 6 - Geo-Visualisation

### Slides

- [pdf](lectures/06-geo-visualisation.pdf)

### To do before class [Takes about 1 hour of prep at home]

* Watch this lecture on  "Statistical maps" by Luc Anselin ([link](https://www.youtube.com/watch?v=6-weK5J6xRI) to 25min video).
* Read the Conversation [piece](http://theconversation.com/how-zip-codes-nearly-masked-the-lead-problem-in-flint-65626) on the Flint case, where the MAUP played a key role.
* Spend the rest of the prep hour browsing through Nathan Yau's excellent blog, [Flowing Data](http://flowingdata.com/).

### Extra Material [Always to learn more but never needed for the course]

* (Brewer, 2015)’s [Designing Better Maps](https://esripress.esri.com/display/index.cfm?fuseaction=display&websiteID=293&moduleID=0) covers several aspects of building compelling geo visualisations.
* [Choropleth chapter](https://geographicdata.science/book/notebooks/05_choropleth.html) from the GDS Book (in progress).
* Color palettes are important for maps. Find some in [ColorBrewer](http://colorbrewer2.org/).


***

(L7)=
## Lecture 7 - Networks and Spatial Weights

### Slides

- [pdf](lectures/07-space.pdf)

### To do before class [Takes about 1 hour of prep at home]

* Read Eli Knaap's blog on [Measuring Urban Segregation with Spatial Computation](https://knaaptime.com/posts/segregation_dynamics/)
* Watch this lecture on  "Spatial Weights" by Luc Anselin ([link](https://www.youtube.com/watch?v=ydFmI6ZGLQ8) to 34min video). Keep in mind the motivation, in this case, is focused on spatial regression.
* Lecture on "Spatial lag" by Luc Anselin ([link](https://www.youtube.com/watch?v=MQACCcfTpXc) to video, you can ignore the last five minutes as they are a bit more advanced).

### Extra Material [Always to learn more but never needed for the course]

* Check out Geoff Boeing's computational notebook showcasing the use of **OSMNX**- a python library for processing street networks as network objects- with a case of [Urban Street Network Analysis](https://escholarship.org/uc/item/6z9802kf.)
* For advanced and in-detail treatment, (Anselin & Rey, 2014) is an excellent reference.



***

(L8)=
## Lecture 8 - Exploratory Spatial Data Analysis

### Slides

- [pdf](lectures/08-esda.pdf)

### To do before class [Takes about 1 hour of prep at home]

* Watch this lecture on "Spatial Autocorrelation (Background)" by Luc Anselin. [[Part I](https://www.youtube.com/watch?v=EotbDebRnFg)][[Part II](https://www.youtube.com/watch?v=69CnasXK2pM)]

### Extra Material [Always to learn more but never needed for the course]

* [Reflections on spatial autocorrelation](https://doi.org/10.1016/j.regsciurbeco.2007.04.005) by a quantitative geographer.

***

(L9)=
## Lecture 9 - Machine Learning for Everyone

You may want to buy [The Hundred-Page Machine Learning Book](https://leanpub.com/theMLbook) as _some_ chapters will be used in _some_ topics from this point onwards and it is generally a fantastic book to have. If you cannot or do not want to spend $20.00 on the e-copy, email me, and we will figure something out. The author has invested a lot in writing this book, and it is an excellent resource on Machine Learning, even beyond this class.

### Slides

- [pdf](lectures/09-ml-for-everyone.pdf)

### To do before class [Takes about 1 hour of prep at home]

* [A Visual Introduction to Machine Learning by r2d3 - Part I: A Decision Tree](http://www.r2d3.us/visual-intro-to-machine-learning-part-1/)
* [A visual introduction to learning linear regression](https://mlu-explain.github.io/linear-regression/).

### Extra Material [Always to learn more but never needed for the course]

The contents of this lecture are loosely based on, and explored into further detail, in the following two references :

* Chapter 1 and section 3.1 of [The Hundred-Page Machine Learning Book](https://leanpub.com/theMLbook) by Andriy Burkov.
* [A Visual Introduction to Machine Learning by r2d3 - Part II: Model Tuning and the Bias-Variance Tradeoff](http://www.r2d3.us/visual-intro-to-machine-learning-part-2/)


***

(L10)=
## Lecture 10 - Anatomy of a Learning Algorithm

### Slides

- [pdf](lectures/10-ml-anatomy.pdf)

### To do before class [Takes about 1 hour of prep at home]

* Read [An accessible introduction to how machine learning is applied in urban design: a generative design tool](https://ui.kpf.com/smarter-city)
* Go through this medium post about [A first step toward the future of neighbourhood design](https://medium.com/sidewalk-talk/a-first-step-toward-the-future-of-neighborhood-design-a2777ad69550)
* Read this critique about neighbourhood design - [A visit to the smart-city-in-progress at Sidewalk Toronto prompts questions about what it means to “participate” in civic design.](https://placesjournal.org/article/post-it-note-city/?cn-reloaded=1&cn-reloaded=1&cn-reloaded=1#ref_17)

### Extra Material [Always to learn more but never needed for the course]

* [Explainable ML/AI: Why Are We Using Black Box Models in AI When We Don’t Need To?](https://hdsr.mitpress.mit.edu/pub/f9kuryi8/release/5)


***

(L11)=
## Lecture 11 - Clustering

### Slides

- [pdf](lectures/11-clustering.pdf)

### To do before class [Takes about 1 hour of prep at home]

* Talk on "Geodemographics and the Internal Structure of Cities" by Prof. Alex Singleton ([link](https://www.youtube.com/watch?v=lslLujtqGlw) to 50min. video).

### Extra Material [Always to learn more but never needed for the course]

* [Supervised Regionalization Methods: A Survey](https://doi.org/10.1177/0160017607301605) is an excellent review of regionalisation algorithms, but it is an excellent read.


***

(L12)=
## Lecture 12 - Dimensionality Reduction

### Slides

- [pdf](lectures/12-dimensionality-reduction.pdf)

### To do before class [Takes about 1 hour of prep at home]

* Read through this excellent step-wise example of [Principal Component Analysis](https://gmaclenn.github.io/articles/airport-pca-analysis/) using airport delay data
* Read this excellent community-driven explanation of [PCA](https://stats.stackexchange.com/questions/2691/making-sense-of-principal-component-analysis-eigenvectors-eigenvalues) on StackExchange.

### Extra Material [Always to learn more but never needed for the course]

* I recommend reading this amazing paper by Caitlin Robinson on [A spatial perspective of energy poverty](https://doi.org/10.1016/j.geoforum.2019.05.001).
* If you are feeling adventurous, you can read my work on [Inequalities in solar adoption in The Hague](https://doi.org/10.1016/j.erss.2023.103245).


***

(L13)=
## Lecture 13 - Spatial Density Estimation

### Slides

- [pdf](lectures/13-points.pdf)

### To do before class [Takes about 1 hour of prep at home]

* Lecture on  "Point Pattern Analysis Basics" by Luc Anselin ([link](https://www.youtube.com/watch?v=Z2iT4JpqGZg&list=PLzREt6r1NenlmAiF3ds5_WGVAG1rTYSK-&index=1) to 45min video, and [link](https://www.youtube.com/watch?v=BN94XXT6Io4) to a more recent 6 min intro).

### Extra Material [Always to learn more but never needed for the course]

* None...


***

(L14)=
## Lecture 14 - Responsible Data Science

### Slides

- [pdf](lectures/14-responsibility.pdf)

### To do before class [Takes about 1 hour of prep at home]

* Read [A city is not a computer](https://placesjournal.org/article/a-city-is-not-a-computer/?cn-reloaded=1), Shannon Mattern which carefully examines the limitations of computation in bettering the human condition.
* Explore the [Gender Shades](http://gendershades.org/overview.html) project by Joy Buolamwini and Timnit Gebru that uncovers the priorities, preferences and prejudices of influential organisations that develop automated systems.

### Extra Material [Always to learn more but never needed for the course]

* Watch [The unfortunate history of racial bias in photography.](https://www.youtube.com/watch?v=d16LNHIEJzs).
* Watch [Coded Bias](https://www.youtube.com/watch?v=jZl55PsfZJQ&feature=youtu.be) on how corporations are not held accountable for deploying algorithms that affect humans.
