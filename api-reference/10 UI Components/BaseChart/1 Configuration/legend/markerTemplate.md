---
id: BaseChart.Options.legend.markerTemplate
---
---
##### shortDescription
Specifies an SVG element that serves as a custom legend item marker.

##### param(legendItem): BaseChartLegendItem
Information about a legend item.

##### param(element): SVGGElement
A marker's container.

##### return: String | SVGElement | jQuery
One of the following:

- Template name
- SVG markup as a string
- SVGElement
- jQuery element that contains an SVGElement

---
#include btn-open-demo with {
    href: "https://js.devexpress.com/Demos/WidgetsGallery/Demo/Charts/CustomLegendMarkers/"
}

#include dataviz-ref-legend-markertemplate