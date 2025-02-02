---
id: dxSortable.Options.onRemove
type: function(e)
default: null
---
---
##### shortDescription
A function that is called when a draggable item is removed.

##### param(e): ui/sortable:RemoveEvent
Information about the event that caused the function's execution.

##### field(e.component): {WidgetName}
The UI component that raised the event.

##### field(e.element): DxElement
#include common-ref-elementparam with { element: "UI component" }

##### field(e.event): event
#include common-ref-eventparam

##### field(e.fromComponent): {WidgetName}
The instance of the item's source UI component.

##### field(e.fromData): any
Custom [data](/api-reference/10%20UI%20Components/DraggableBase/1%20Configuration/data.md '{basewidgetpath}/Configuration/#data') associated with the source UI component.

##### field(e.fromIndex): Number
The item's original position. If the item is dragged from another UI component, the value is **-1**.

##### field(e.itemData): any
The dragged item's data.

##### field(e.itemElement): DxElement
#include draganddrop-ref-itemelementparam

##### field(e.model): any
Model data. Available only if you use Knockout.

##### field(e.toComponent): {WidgetName}
The instance of the item's target UI component.

##### field(e.toData): any
Custom [data](/api-reference/10%20UI%20Components/DraggableBase/1%20Configuration/data.md '{basewidgetpath}/Configuration/#data') associated with the target UI component.

##### field(e.toIndex): Number
The position in which the item is placed. If the item is dragged away from the UI component, the value is **-1**.

---
<!-- Description goes here -->
