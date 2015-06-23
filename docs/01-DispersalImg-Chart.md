---
title: Dispersal Img Chart

---
###Introduction
A Dispersal Img chart is a way of plotting Img points in  x and y.

Often, it is used to show trend data, and the comparison of two data sets.

<div class="canvas-holder">
	<canvas width="250" height="125"></canvas>
</div>

###Example usage
```javascript
var myDispersalImg=new Chart(ctx).DispersalImg(data, options);
```
###Data structure

```javascript
var dispersalData = {
		labels : ["Mercantil","Banesco","uniseguro","Manfre","catatumbo","seguritas"],
                labelX :"Prima Asegurada",
                labelY :"Suma Asegurada",
                labelProm:"Promedio",
		datasets : [
			{
                                fillColor : "rgba(220,220,220,0.5)",
				strokeColor : "rgba(220,220,220,0.8)",
				highlightFill: "rgba(220,220,220,0.75)",
				highlightStroke: "rgba(220,220,220,1)",
                                
                                fillColorProm : "rgba(220,220,220,0.5)",
				strokeColorProm : "rgba(220,220,220,0.8)",
				highlightFillProm: "rgba(220,220,220,0.75)",
				highlightStrokeProm: "rgba(220,220,220,1)",
                                dataXY:[
                                         {x:10,y:20,imgSrc:"../images/banesco.png"},
                                         {x:20,y:40,imgSrc:"../images/constitucion.png"},
                                         {x:30,y:60,imgSrc:"../images/ibero.png"},
                                         {x:40,y:80,imgSrc:"../images/mapfre.png"},
                                         {x:50,y:100,imgSrc:"../images/mercantil.png"},
                                         {x:60,y:110,imgSrc:"../images/multinacional.png"}
                                     ]
			}
		]

	}
```




### Chart options

These are the customisation options specific to Line charts. These options are merged with the [global chart configuration options](#getting-started-global-chart-configuration), and form the options of the chart.

```javascript
{

	///Boolean - Whether grid lines are shown across the chart
	scaleShowGridLines : true,

	//String - Colour of the grid lines
	scaleGridLineColor : "rgba(0,0,0,.05)",

	//Number - Width of the grid lines
	scaleGridLineWidth : 1,

	//Boolean - Whether to show horizontal lines (except X axis)
	scaleShowHorizontalLines: true,

	//Boolean - Whether to show vertical lines (except Y axis)
	scaleShowVerticalLines: true,

	//Boolean - Whether the line is curved between points
	bezierCurve : true,

	//Boolean - Whether to show a dot for each point
	pointDot : true,

	//Number - Pixel width of point dot stroke
	pointDotStrokeWidth : 1,

        scaleBeginAtZero : true,

	
	
};
```
