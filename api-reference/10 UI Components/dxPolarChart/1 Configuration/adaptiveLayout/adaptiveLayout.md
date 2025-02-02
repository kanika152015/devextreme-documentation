---
id: dxPolarChart.Options.adaptiveLayout
type: viz/polar_chart:AdaptiveLayout
inheritsType: viz/polar_chart:AdaptiveLayout
---
---
##### shortDescription
Specifies adaptive layout properties.

---
The adaptive layout enables the UI component to hide optional elements if they do not fit in the container. Elements are hidden in the following sequence:

1. [Title](/api-reference/10%20UI%20Components/dxPolarChart/1%20Configuration/title.md '{basewidgetpath}/Configuration/title')
2. [Export menu icon](/api-reference/10%20UI%20Components/BaseWidget/1%20Configuration/export '{basewidgetpath}/Configuration/export')
3. [Legend](/api-reference/10%20UI%20Components/dxPolarChart/9%20Types/dxPolarChartLegend '{basewidgetpath}/Configuration/legend')
4. [Argument axis labels](/api-reference/10%20UI%20Components/dxPolarChart/9%20Types/dxPolarChartCommonAxisSettings/label.md '{basewidgetpath}/Configuration/argumentAxis/label')
5. [Point labels](/api-reference/10%20UI%20Components/dxPolarChart/5%20Series%20Types/CommonPolarChartSeries/label '{basewidgetpath}/Configuration/commonSeriesSettings/label') (can be saved by setting the **adaptiveLayout**.[keepLabels](/api-reference/10%20UI%20Components/BaseChart/1%20Configuration/adaptiveLayout/keepLabels.md '{basewidgetpath}/Configuration/adaptiveLayout#keepLabels') property to **true**)

Use the **height** and **width** properties in the **adaptiveLayout** object to specify the minimum container size at which the layout begins to adapt.

<a href="https://jsfiddle.net/ChartJS/0s1tw53v/" class="button orange small fix-width-155" style="margin-right: 20px;" target="_blank">View Demo on JSFiddle</a>