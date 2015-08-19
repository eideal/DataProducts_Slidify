---
title       : Developing Data Products Course Project
subtitle    : U.S. State Crime
author      : Emma Ideal
job         : 
framework   : revealjs        # {revealjs, io2012, html5slides, shower, dzslides, ...}
highlighter : prettify  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [shiny, interactive]  # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
runtime     : shiny
knit        : slidify::knit2slides
---

# In What U.S. State Should You Live?*

<font size="5">*if you want to base your decision on crime levels in 1973</font>

--- 

## Have a look at:

- <span style="color:green">Assault</span> (per 100k residents)  
- <span style="color:mediumblue">Murder</span> (per 100k residents)   
- <span style="color:darkmagenta">Rape</span> (per 100k residents)
- % <span style="color:chocolate">Urban</span> population

&nbsp;


For each U.S. state, and even...


--- &interactive

## Use Interactive Maps!
<!-- GeoChart generated in R 3.2.1 by googleVis 0.5.9 package -->
<!-- Wed Aug 19 22:21:17 2015 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataGeoChartID51507b4ad187 () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 "Alabama",
236 
],
[
 "Alaska",
263 
],
[
 "Arizona",
294 
],
[
 "Arkansas",
190 
],
[
 "California",
276 
],
[
 "Colorado",
204 
],
[
 "Connecticut",
110 
],
[
 "Delaware",
238 
],
[
 "Florida",
335 
],
[
 "Georgia",
211 
],
[
 "Hawaii",
46 
],
[
 "Idaho",
120 
],
[
 "Illinois",
249 
],
[
 "Indiana",
113 
],
[
 "Iowa",
56 
],
[
 "Kansas",
115 
],
[
 "Kentucky",
109 
],
[
 "Louisiana",
249 
],
[
 "Maine",
83 
],
[
 "Maryland",
300 
],
[
 "Massachusetts",
149 
],
[
 "Michigan",
255 
],
[
 "Minnesota",
72 
],
[
 "Mississippi",
259 
],
[
 "Missouri",
178 
],
[
 "Montana",
109 
],
[
 "Nebraska",
102 
],
[
 "Nevada",
252 
],
[
 "New Hampshire",
57 
],
[
 "New Jersey",
159 
],
[
 "New Mexico",
285 
],
[
 "New York",
254 
],
[
 "North Carolina",
337 
],
[
 "North Dakota",
45 
],
[
 "Ohio",
120 
],
[
 "Oklahoma",
151 
],
[
 "Oregon",
159 
],
[
 "Pennsylvania",
106 
],
[
 "Rhode Island",
174 
],
[
 "South Carolina",
279 
],
[
 "South Dakota",
86 
],
[
 "Tennessee",
188 
],
[
 "Texas",
201 
],
[
 "Utah",
120 
],
[
 "Vermont",
48 
],
[
 "Virginia",
156 
],
[
 "Washington",
145 
],
[
 "West Virginia",
81 
],
[
 "Wisconsin",
53 
],
[
 "Wyoming",
161 
] 
];
data.addColumn('string','state');
data.addColumn('number','Assault');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartGeoChartID51507b4ad187() {
var data = gvisDataGeoChartID51507b4ad187();
var options = {};
options["width"] =    600;
options["height"] =    400;
options["region"] = "US";
options["resolution"] = "provinces";
options["displayMode"] = "regions";
options["forceIFrame"] = "TRUE";
options["colorAxis"] = {colors:['#FFFFFF', '#0000FF']};

    var chart = new google.visualization.GeoChart(
    document.getElementById('GeoChartID51507b4ad187')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "geochart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartGeoChartID51507b4ad187);
})();
function displayChartGeoChartID51507b4ad187() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartGeoChartID51507b4ad187"></script>
 
<!-- divChart -->
  
<div id="GeoChartID51507b4ad187" 
  style="width: 600; height: 400;">
</div>

--- 
## Ever thought about moving to North Dakota?
<iframe src="https://eideal.shinyapps.io/DataProducts_AppforSlidify" width="100%" height="100" class="shiny-frame"></iframe>


--- 

## Interested?* Find out more:

- See the app on [shinyapps.io](https://eideal.shinyapps.io/DataProducts_CourseProject)  
- Source code on [Github](https://github.com/eideal/DataProducts_CourseProject)

&nbsp;


<font size="4">*I'm not surprised</font>





