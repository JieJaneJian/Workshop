# Workshop
Workshop material for Tableau

# HTML Code 1
<html>
<header><title>This is title</title></header>
<body>
<h3>Let’s learn D3!</h3>
</body>
</html>

# HTML Code 2
<html>
<head>
    <title>Learn D3 in 5 minutes</title>
</head>
<body>
<h3>Let’s learn D3!</h3>
<script src='https://d3js.org/d3.v4.min.js'></script>
<script>
    d3.select('h3').style('color', 'darkblue');
    d3.select('h3').style('font-size', '24px');
</script>
</body>
</html>

# HTML Code 3
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<title>Minimal D3 Example</title>
<script src="http://d3js.org/d3.v3.min.js" charset="utf-8"></script>
 
<style>
.bar {
  fill: steelblue;
}
 
.bar:hover {
  fill: orange;
}
</style>
</head>
<body>
<script type="text/javascript">
 
var data = [150, 230, 180, 90];
 
var svg = d3.select("body")
            .append("svg")
            .attr("width", 300)
            .attr("height", 200);
 
svg.selectAll(".bar")
  .data(data)
  .enter()
  .append("rect")
  .attr({
    class : "bar",
    width : function(d) {return d;},
    height: "40",
    y : function(d, i) {return i*50 + 10;},
    x : "10"
   });
   
</script>	
</body>
</html>

# Good sources for d3.js: 
https://d3js.org/
