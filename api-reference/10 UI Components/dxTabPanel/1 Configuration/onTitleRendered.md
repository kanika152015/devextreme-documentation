---
id: dxTabPanel.Options.onTitleRendered
type: function(e)
default: null
---
---
##### shortDescription
A function that is executed after a tab is rendered.

##### param(e): ui/tab_panel:TitleRenderedEvent
Information about the event.

##### field(e.component): {WidgetName}
The UI component's instance.

##### field(e.element): DxElement
#include common-ref-elementparam with { element: "UI component" }

##### field(e.itemData): any
The data of the item whose title is rendered.

##### field(e.itemElement): DxElement
#include common-ref-elementparam with { element: "item" }

##### field(e.model): any
Model data. Available only if Knockout is used.

---
