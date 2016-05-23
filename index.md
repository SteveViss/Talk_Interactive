---
title       : New avenues on visualization with R
subtitle    : R is more than statistics...
author      : Steve Vissault
job         : Research professional at UdS
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      #
widgets     : [mathjax, quiz, bootstrap, interactive] # {mathjax, quiz, bootstrap}
ext_widgets : {rCharts: [libraries/nvd3, libraries/leaflet, libraries/dygraphs]}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
biglogo     : qcbs.png
assets      : {assets: ../../assets}

---

## R and the Web languages

RMarkdown + knitr = HTML + CSS + Javascript

[http://slidify.org/](http://slidify.org/)

Allow to generate slides in HTML/CSS/Javascript (Web lamguages)
which is the new avenue for dynamic and interactive visualization

--- .segue bg:white

## Interactivity

---

## Hans Rosling and R

<div align="center">


</div>

--- .segue bg:white

## HTML widgets

---

## HTML widget library

HTML widgets are interactive graphics made for the web. These are the main libraries available:

- [rCharts](http://rcharts.io/): interactive javascript visualizations from R
- [leaflet](https://rstudio.github.io/leaflet/): interactive maps
- [dygraphs](https://rstudio.github.io/dygraphs/): charting time series data
- [metricsgraphics](http://www.htmlwidgets.org/showcase_metricsgraphics.html): scatterplots, linegraphs and histograms
- [networkD3](http://christophergandrud.github.io/networkD3/): network graphs
- [DT](https://rstudio.github.io/DT/): print dataframes as html
- [threejs](http://www.htmlwidgets.org/showcase_threejs.html): 3d scatterplots and [globes](https://www.chromeexperiments.com/globe)
- [DiagrammeR](http://rich-iannone.github.io/DiagrammeR/): pretty diagrams

--- &radio2

## Quizz

Which of these two plots have a higher correlation?

1. A
2. B

*** =image

<img src=https://oli.cmu.edu/repository/webcontent/470835bf80020ca60018d5a6c359d34c/_u2_summarizing_data/_m2_examining_relationships/webcontent/linear1.gif>

*** .explanation

Both have the same correlation.

---
## rCharts


<div id = 'chart61022929650d' class = 'rChart nvd3'></div>
<script type='text/javascript'>
 $(document).ready(function(){
      drawchart61022929650d()
    });
    function drawchart61022929650d(){  
      var opts = {
 "dom": "chart61022929650d",
"width":    800,
"height":    400,
"x": "wt",
"y": "mpg",
"type": "scatterChart",
"id": "chart61022929650d" 
},
        data = [
 {
 "mpg":             21,
"cyl":              6,
"disp":            160,
"hp":            110,
"drat":            3.9,
"wt":           2.62,
"qsec":          16.46,
"vs":              0,
"am":              1,
"gear":              4,
"carb":              4 
},
{
 "mpg":             21,
"cyl":              6,
"disp":            160,
"hp":            110,
"drat":            3.9,
"wt":          2.875,
"qsec":          17.02,
"vs":              0,
"am":              1,
"gear":              4,
"carb":              4 
},
{
 "mpg":           22.8,
"cyl":              4,
"disp":            108,
"hp":             93,
"drat":           3.85,
"wt":           2.32,
"qsec":          18.61,
"vs":              1,
"am":              1,
"gear":              4,
"carb":              1 
},
{
 "mpg":           21.4,
"cyl":              6,
"disp":            258,
"hp":            110,
"drat":           3.08,
"wt":          3.215,
"qsec":          19.44,
"vs":              1,
"am":              0,
"gear":              3,
"carb":              1 
},
{
 "mpg":           18.7,
"cyl":              8,
"disp":            360,
"hp":            175,
"drat":           3.15,
"wt":           3.44,
"qsec":          17.02,
"vs":              0,
"am":              0,
"gear":              3,
"carb":              2 
},
{
 "mpg":           18.1,
"cyl":              6,
"disp":            225,
"hp":            105,
"drat":           2.76,
"wt":           3.46,
"qsec":          20.22,
"vs":              1,
"am":              0,
"gear":              3,
"carb":              1 
},
{
 "mpg":           14.3,
"cyl":              8,
"disp":            360,
"hp":            245,
"drat":           3.21,
"wt":           3.57,
"qsec":          15.84,
"vs":              0,
"am":              0,
"gear":              3,
"carb":              4 
},
{
 "mpg":           24.4,
"cyl":              4,
"disp":          146.7,
"hp":             62,
"drat":           3.69,
"wt":           3.19,
"qsec":             20,
"vs":              1,
"am":              0,
"gear":              4,
"carb":              2 
},
{
 "mpg":           22.8,
"cyl":              4,
"disp":          140.8,
"hp":             95,
"drat":           3.92,
"wt":           3.15,
"qsec":           22.9,
"vs":              1,
"am":              0,
"gear":              4,
"carb":              2 
},
{
 "mpg":           19.2,
"cyl":              6,
"disp":          167.6,
"hp":            123,
"drat":           3.92,
"wt":           3.44,
"qsec":           18.3,
"vs":              1,
"am":              0,
"gear":              4,
"carb":              4 
},
{
 "mpg":           17.8,
"cyl":              6,
"disp":          167.6,
"hp":            123,
"drat":           3.92,
"wt":           3.44,
"qsec":           18.9,
"vs":              1,
"am":              0,
"gear":              4,
"carb":              4 
},
{
 "mpg":           16.4,
"cyl":              8,
"disp":          275.8,
"hp":            180,
"drat":           3.07,
"wt":           4.07,
"qsec":           17.4,
"vs":              0,
"am":              0,
"gear":              3,
"carb":              3 
},
{
 "mpg":           17.3,
"cyl":              8,
"disp":          275.8,
"hp":            180,
"drat":           3.07,
"wt":           3.73,
"qsec":           17.6,
"vs":              0,
"am":              0,
"gear":              3,
"carb":              3 
},
{
 "mpg":           15.2,
"cyl":              8,
"disp":          275.8,
"hp":            180,
"drat":           3.07,
"wt":           3.78,
"qsec":             18,
"vs":              0,
"am":              0,
"gear":              3,
"carb":              3 
},
{
 "mpg":           10.4,
"cyl":              8,
"disp":            472,
"hp":            205,
"drat":           2.93,
"wt":           5.25,
"qsec":          17.98,
"vs":              0,
"am":              0,
"gear":              3,
"carb":              4 
},
{
 "mpg":           10.4,
"cyl":              8,
"disp":            460,
"hp":            215,
"drat":              3,
"wt":          5.424,
"qsec":          17.82,
"vs":              0,
"am":              0,
"gear":              3,
"carb":              4 
},
{
 "mpg":           14.7,
"cyl":              8,
"disp":            440,
"hp":            230,
"drat":           3.23,
"wt":          5.345,
"qsec":          17.42,
"vs":              0,
"am":              0,
"gear":              3,
"carb":              4 
},
{
 "mpg":           32.4,
"cyl":              4,
"disp":           78.7,
"hp":             66,
"drat":           4.08,
"wt":            2.2,
"qsec":          19.47,
"vs":              1,
"am":              1,
"gear":              4,
"carb":              1 
},
{
 "mpg":           30.4,
"cyl":              4,
"disp":           75.7,
"hp":             52,
"drat":           4.93,
"wt":          1.615,
"qsec":          18.52,
"vs":              1,
"am":              1,
"gear":              4,
"carb":              2 
},
{
 "mpg":           33.9,
"cyl":              4,
"disp":           71.1,
"hp":             65,
"drat":           4.22,
"wt":          1.835,
"qsec":           19.9,
"vs":              1,
"am":              1,
"gear":              4,
"carb":              1 
},
{
 "mpg":           21.5,
"cyl":              4,
"disp":          120.1,
"hp":             97,
"drat":            3.7,
"wt":          2.465,
"qsec":          20.01,
"vs":              1,
"am":              0,
"gear":              3,
"carb":              1 
},
{
 "mpg":           15.5,
"cyl":              8,
"disp":            318,
"hp":            150,
"drat":           2.76,
"wt":           3.52,
"qsec":          16.87,
"vs":              0,
"am":              0,
"gear":              3,
"carb":              2 
},
{
 "mpg":           15.2,
"cyl":              8,
"disp":            304,
"hp":            150,
"drat":           3.15,
"wt":          3.435,
"qsec":           17.3,
"vs":              0,
"am":              0,
"gear":              3,
"carb":              2 
},
{
 "mpg":           13.3,
"cyl":              8,
"disp":            350,
"hp":            245,
"drat":           3.73,
"wt":           3.84,
"qsec":          15.41,
"vs":              0,
"am":              0,
"gear":              3,
"carb":              4 
},
{
 "mpg":           19.2,
"cyl":              8,
"disp":            400,
"hp":            175,
"drat":           3.08,
"wt":          3.845,
"qsec":          17.05,
"vs":              0,
"am":              0,
"gear":              3,
"carb":              2 
},
{
 "mpg":           27.3,
"cyl":              4,
"disp":             79,
"hp":             66,
"drat":           4.08,
"wt":          1.935,
"qsec":           18.9,
"vs":              1,
"am":              1,
"gear":              4,
"carb":              1 
},
{
 "mpg":             26,
"cyl":              4,
"disp":          120.3,
"hp":             91,
"drat":           4.43,
"wt":           2.14,
"qsec":           16.7,
"vs":              0,
"am":              1,
"gear":              5,
"carb":              2 
},
{
 "mpg":           30.4,
"cyl":              4,
"disp":           95.1,
"hp":            113,
"drat":           3.77,
"wt":          1.513,
"qsec":           16.9,
"vs":              1,
"am":              1,
"gear":              5,
"carb":              2 
},
{
 "mpg":           15.8,
"cyl":              8,
"disp":            351,
"hp":            264,
"drat":           4.22,
"wt":           3.17,
"qsec":           14.5,
"vs":              0,
"am":              1,
"gear":              5,
"carb":              4 
},
{
 "mpg":           19.7,
"cyl":              6,
"disp":            145,
"hp":            175,
"drat":           3.62,
"wt":           2.77,
"qsec":           15.5,
"vs":              0,
"am":              1,
"gear":              5,
"carb":              6 
},
{
 "mpg":             15,
"cyl":              8,
"disp":            301,
"hp":            335,
"drat":           3.54,
"wt":           3.57,
"qsec":           14.6,
"vs":              0,
"am":              1,
"gear":              5,
"carb":              8 
},
{
 "mpg":           21.4,
"cyl":              4,
"disp":            121,
"hp":            109,
"drat":           4.11,
"wt":           2.78,
"qsec":           18.6,
"vs":              1,
"am":              1,
"gear":              4,
"carb":              2 
} 
]
  
      if(!(opts.type==="pieChart" || opts.type==="sparklinePlus" || opts.type==="bulletChart")) {
        var data = d3.nest()
          .key(function(d){
            //return opts.group === undefined ? 'main' : d[opts.group]
            //instead of main would think a better default is opts.x
            return opts.group === undefined ? opts.y : d[opts.group];
          })
          .entries(data);
      }
      
      if (opts.disabled != undefined){
        data.map(function(d, i){
          d.disabled = opts.disabled[i]
        })
      }
      
      nv.addGraph(function() {
        var chart = nv.models[opts.type]()
          .width(opts.width)
          .height(opts.height)
          
        if (opts.type != "bulletChart"){
          chart
            .x(function(d) { return d[opts.x] })
            .y(function(d) { return d[opts.y] })
        }
          
         
        
          
        

        
        
        
      
       d3.select("#" + opts.id)
        .append('svg')
        .datum(data)
        .transition().duration(500)
        .call(chart);

       nv.utils.windowResize(chart.update);
       return chart;
      });
    };
</script>

Gallery: [http://rcharts.io/gallery/](http://rcharts.io/gallery/)

---

## leaflet



<iframe src="./assets/widgets/leaflet1.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## dygraphs

<iframe src="./assets/widgets/dygraphs1.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## dygraphs (cont)

<iframe src="./assets/widgets/dygraphs2.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## dygraphs (cont)

<iframe src="./assets/widgets/dygraphs3.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## dygraphs (cont)

<iframe src="./assets/widgets/dygraphs4.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## metricsgraphics

<iframe src="./assets/widgets/metricsgraphics1.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## metricsgraphics (cont)

<iframe src="./assets/widgets/metricsgraphics2.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## metricsgraphics (cont)

<iframe src="./assets/widgets/metricsgraphics3.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## metricsgraphics (cont)

<iframe src="./assets/widgets/metricsgraphics4.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## metricsgraphics (cont)

<iframe src="./assets/widgets/metricsgraphics5.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## metricsgraphics (cont)

<iframe src="./assets/widgets/metricsgraphics6.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## networkD3

<iframe src="./assets/widgets/networkD31.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## networkD3 (cont)

<iframe src="./assets/widgets/networkD32.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## DT

<iframe src="./assets/widgets/dt1.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## threejs

<iframe src="./assets/widgets/threejs1.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## threejs (cont)

<iframe src="./assets/widgets/threejs2.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## DiagrammeR

<iframe src="./assets/widgets/diagrammer1.html" width=100% height=100% allowtransparency="true"> </iframe>

---

## DiagrammeR (cont)

<iframe src="./assets/widgets/diagrammer2.html" width=100% height=100% allowtransparency="true"> </iframe>
