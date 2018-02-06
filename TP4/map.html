<!DOCTYPE html>
<head>
  <meta charset="utf-8">
  <script src="https://d3js.org/d3.v4.min.js"></script>
  <style>
    body { margin:0;position:fixed;top:0;right:0;bottom:0;left:0; }
  </style>
</head>

<style>
    .hidden {
        display: none;
    }
    div.tooltip {
        color: #222;
        background-color: #fff;
        padding: .5em;
        text-shadow: #f5f5f5 0 1px 0;
        border-radius: 2px;
        opacity: 0.9;
        position: absolute;
    }
</style>



<body>
  <script>
		var width = 960,
  		  height = 500;

		var svg = d3.select( "body" )
  		.append( "svg" )
		  .attr( "width", width )
		  .attr( "height", height );

    var projection = d3.geoConicConformal().center([2.454071, 46.279229]).scale(2800)
    			.translate([width/2, height/2])

    var path = d3.geoPath()
                 .projection(projection);
    
    var color = d3.scaleLinear()
      						.interpolate(d3.interpolateHcl)
      						.range(['white','green']);
    
    var tooltip = d3.select('body').append('div')
            .attr('class', 'hidden tooltip');

    
d3.csv("GrippeFrance2014.csv", function(data) {
    color.domain([0,4200]);
  
    d3.json("regions.json", function(json) {
      //On fusionne les donnees avec le GeoJSON des regions
   
      
      for (var i = 0; i < data.length; i++) {
				
        var name = data[i].region

        for (var j = 0; j<json.features.length;j++)
        {
          
          if(json.features[j].properties.nom == name)
								json.features[j].properties.data=data[i] 
               
         }
      }
      
 			svg.selectAll("path")
           .data(json.features)
           .enter()
           .append("path")
           .attr("d", path)
      		 .attr("fill",function(d) {if(d.properties.data) {return color(d.properties.data.somme2014)} else {return color(0)} })
      		 .on('mousemove', function(d) {
                    var mouse = d3.mouse(svg.node()).map(function(d) {
                        return parseInt(d);
                    });
                    tooltip.classed('hidden', false)
                        .attr('style', 'left:' + (mouse[0] + 15) +
                                'px; top:' + (mouse[1] - 35) + 'px')
                        .html(d.properties.nom);
                })
                .on('mouseout', function() {
                    tooltip.classed('hidden', true);
                });
      
      
      });
    });
    
  </script>
</body>
