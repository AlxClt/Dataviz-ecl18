## TP 1 - Data Visualization - Mosaic Chart

### 1) What is a mosaic chart exactly?

#### a) Definition 

A mosaic chart, also known under the name "Marimekko diagram" is a chart designed to vizualise the data of two or more qualitative variable  

The basic version of this chart plots the distribution of the data according to two variables, allowing to spot relationships between the variables. It ca be particulary usefull to infer statitical dependance/independance between two variables.

The following chart<sup>[1]</sup> shows the simplest mosaic plot. The 'answer' fild refers to the question "do you like sushis?":

<p align="center">
  <img src=https://github.com/AlxClt/dataviz_ecl18/blob/master/TP1/img/mosaic5.png/>
</p>

This chart is quite similar to a classic bar chart. We can see that more men thant women like sushis, which leads to the conclusion that 'liking sushis' is not independant from the biological gender. 

You would say, great but why not using a bar chart since it is the same?

#### b) Why is it widely different from a bar chart?

Well if you look closer you will see that the width of the columns is not the same, hence it carries more information than a simple bar chart. Indeed, the width represents the ration of genders participating in the study : there were more men than women. 

A famous usecase of this property is the analysis of the 1973 Berkeley admissions data. The goal was to study the differences in admission according to gender. The simplest mosaic chart is the following<sup>[2]</sup>:

<p align="center">
  <img src=https://github.com/AlxClt/dataviz_ecl18/blob/master/TP1/img/mosaic12.PNG />
</p>

The chart shows clearly that women tended to be less admitted than men. But it can show more.

 #### c) Plotting more than two variables

In order to better understand the difference, we can __increase the granularity__ and split the admissions by department. In the end, a mosaik plot allows to visualize the dependancies between more than two variables too. This plot shows indeed the relationship between admission, gender and department<sup>[3]</sup> :
  
<p align="center">
  <img src=https://github.com/AlxClt/dataviz_ecl18/blob/master/TP1/img/mosaic13.PNG />
</p>

And with this level of granularity we can see that the repartition varies a lot across departments. Visually talking, the spaces between departments columns is wider than between admission columns. This allows to 'group' the results by department first and then gender.

If we look at the results, we can see that despite having less women candidates departments A an B admits more women in proportion, whereas it is the contrary for the other. 


### 2) Mosaic plots examples

Let' study some mosaic plots that give information about various fields. Most of the mosaic plots are for two variables.

#### a) Song themes by decade

This plot<sup>[4]</sup> shows the top songs topic by decade (from  the Guardian's list of "1000 songs to hear before you die"):

<p align="center">
  <img src=https://github.com/AlxClt/dataviz_ecl18/blob/master/TP1/img/Mosaic1.png />
</p>

The width corresponds to the proportion of the list's songs that dates from the corresponding decade. We can see that :
* According to this list, the 60's and 70' have more great songs
* People from the 2000's enjoy mors songs about heartbreak and party than people from the 50's which prefered songs about people and places

#### b) Smartphone manufacturers and operating systems

<p align="center">
  <img src=https://github.com/AlxClt/dataviz_ecl18/blob/master/TP1/img/mosaic2.png />
</p>

This plot<sup>[5]</sup> gives us the following information :
* The share of each operating system
* The share of each manufacturer using which operating system

#### c) Data jobs

Data science and Bigs Data have been great buzzwords lately. What if a mosaic chart could help better defining the jobs in these fields?

The following plot<sup>[6]</sup> shows which skills to associate with which profile :

<p align="center">
  <img src=https://github.com/AlxClt/dataviz_ecl18/blob/master/TP1/img/mosaic4.png />
</p>

According to this analysis I would be more a 'data creative'. What about you?

#### d) Wine vs music

Statistical dependance can give us insight about a commercial strategy. This example <sup>[7]</sup> proves that the wine customer buy in a restaurant is influenced by the music :

<p align="center">
  <img src=https://github.com/AlxClt/dataviz_ecl18/blob/master/TP1/img/mosaic7.jpg />
</p>

French music leads to an increase in french wines sells and italian music to an increase in italian wines. Stucked with a stock of non selling french wines? Play some french music!

This plots alos shows that the musics were played in quite equal proportions (width)

#### e) Airplane crashes

What if a mosaic chart could infor us on the causes of airplane crashes? Indeed the following plot <sup>[8]</sup> shows that the origin of the crash and the flight phase are not independant : 

<p align="center">
  <img src=https://github.com/AlxClt/dataviz_ecl18/blob/master/TP1/img/mosaic10.png />
</p>

As an example, criminals strikes more in the 'en route' phase (flying) and human errors occurs more in the landing phase!

#### f) Votes

This chart<sup>[9]</sup> analyses the dependance between the neighborhood and the vote in the United States. Here again, we see that the variables are not independant. 

<p align="center">
  <img src=https://github.com/AlxClt/dataviz_ecl18/blob/master/TP1/img/mosaic9.png />
</p>

#### g) Titanic disaster : an exemple of a complex mosaik plot

Last but not least, the famous titanic disaster dataset is suitable for a mosaic plot. This plot<sup>[10]</sup> handles __four qualitative variables at the time__ : survived, age group, class, and gender.

<p align="center">
  <img src=https://github.com/AlxClt/dataviz_ecl18/blob/master/TP1/img/mosaic14.png />
</p>

The chart becomes however more complicated to read... Noticing that the color is dark when people died and light when they survuved helps a lot.

This plot show that if we can admit that 'children and women first' was a real thing, it is more accurate to say that it was 'women, children and rich first'! Indeed the ratios of surviving people (no matter the sex or age class) is way higher for the first class passengers and decrases with the class...

### 3) Conclusion

Mosaic charts are a good tool to visualize statistical dependances between two qualitative variables. As an examplethey can be useful to understand dependancies while constructing a bayesian network

They are also good tools to visualize dependancies beween three and four qualitative variables, which is uncommon for a 2D chart. However, given the last example, I wouldn't recommend to plot more than four variables because the resulting complexity would make the vizualisation hard to understand and hence lose the explanatory power of the vizualisation.

### 4) Sources

[1](https://steemit.com/programming/@dkmathstats/displaying-table-results-in-r)

[2](https://ncss-wpengine.netdna-ssl.com/wp-content/themes/ncss/pdf/Procedures/NCSS/Mosaic_Plots.pdf)

[3](https://ncss-wpengine.netdna-ssl.com/wp-content/themes/ncss/pdf/Procedures/NCSS/Mosaic_Plots.pdf)

[4](https://en.wikipedia.org/wiki/Mosaic_plot)

[5](http://www.actuarially.co.uk/post/27156208823/smartphone-operating-system-share-mosaic-plot)

[6](https://jeremiahstanghini.com/2017/07/30/what-is-data-science/)

[7](https://www.qimacros.com/quality-tools/mosaic-chart-marimekko/)

[8](http://proc-x.com/2015/03/visualizing-the-causes-of-airline-crashes/)

[9](https://blogs.sas.com/content/sastraining/2012/10/23/top-3-updates-to-categorical-data-analysis-using-sas/)

[10](http://www.grroups.com/blog/r-graphics-tutorial-series-part-4)
