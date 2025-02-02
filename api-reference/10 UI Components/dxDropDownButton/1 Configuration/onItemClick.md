---
id: dxDropDownButton.Options.onItemClick
type: function(e)
default: null
---
---
##### shortDescription
A function that is executed when a drop-down menu item is clicked.

##### param(e): ui/drop_down_button:ItemClickEvent
Information about the event that caused the function to execute.

##### field(e.component): {WidgetName}
The UI component's instance.

##### field(e.element): DxElement
#include common-ref-elementparam with { element: "UI component" }

##### field(e.event): event
#include common-ref-eventparam

##### field(e.itemData): Object
The clicked item's data.

##### field(e.itemElement): DxElement
#include common-ref-elementparam with { element: "item" }

##### field(e.model): any
Model data. Available only if you use Knockout.

---
