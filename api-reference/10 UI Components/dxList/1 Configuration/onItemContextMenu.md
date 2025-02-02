---
id: dxList.Options.onItemContextMenu
type: function(e)
default: null
---
---
##### shortDescription
A function that is executed when a collection item is right-clicked or pressed.

##### param(e): ui/list:ItemContextMenuEvent
Information about the event.

##### field(e.component): {WidgetName}
The UI component's instance.

##### field(e.element): DxElement
#include common-ref-elementparam with { element: "UI component" }

##### field(e.event): event
#include common-ref-eventparam

##### field(e.itemData): any
The target item's data object.

##### field(e.itemElement): DxElement
#include common-ref-elementparam with { element: "target item" }

##### field(e.itemIndex): Number | Object
The target item's index. In a grouped list, the index is specified as an object defining group and item indexes: { group: 0, item: 0 }.

##### field(e.model): any
Model data. Available only if Knockout is used.

---
