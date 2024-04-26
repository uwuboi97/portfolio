

document.addEventListener("DOMContentLoaded", function() {
	var openscroll = document.getElementsByClassName("text");
	var scrolltxtbox = document.getElementsByClassName("scroll");
	
		// Open the corresponding div when the button is clicked
	for (var i = 0; i < openscroll.length; i++) {
			openscroll[i].addEventListener("click", function() {
				console.log("scroll")
				var index = Array.prototype.indexOf.call(openscroll, this);
				d3.select(".scroll").style("opacity", "1").style("visibility", "visible").style("transition", "opacity 0.5s, visibility 0s").style("transition-delay", "500ms").style("pointer-events", "auto")	
				d3.select(".mask").style("opacity", "1").style("transition", "opacity 1.5s").style("pointer-events", "auto")	
			});
		}
	
		// Close the div when clicking anywhere on the page once open
		document.addEventListener("click", function(event) {
			if (event.target !== openscroll[0] && event.target !== scrolltxtbox[0]) {
				d3.select(".scroll").style("opacity", "0").style("visibility", "hidden").style("transition", "opacity 0.5s, visibility 0.5s").style("transition-delay", "500ms").style("pointer-events", "none")	
				d3.select(".mask").style("opacity", "0").style("transition", "opacity 1.5s").style("pointer-events", "none")	
			}
		});
	});
