---
id: dxSelectBox
module: ui/select_box
export: default
inherits: dxDropDownList
---
---
##### shortDescription
The SelectBox UI component is an editor that allows an end user to select an item from a drop-down list.

##### widgettree
dataSource: [
    "HD Video Player",
    "SuperHD Video Player",
    "SuperPlasma 50",
    "SuperLED 50",
    "SuperLED 42",
    "SuperLCD 55",
    "SuperLCD 42",
    "SuperPlasma 65",
    "SuperLCD 70",
    "Projector Plus",
    "Projector PlusHT",
    "ExcelRemote IR",
    "ExcelRemote BT",
    "ExcelRemote IP"
]

##### lib
dx.web.js, dx.all.js

---
#include common-tutorialbutton with {
    url: "/Documentation/Guide/UI_Components/SelectBox/Getting_Started_with_SelectBox/" 
}

#include btn-open-demo with {
    href: "https://js.devexpress.com/Demos/WidgetsGallery/Demo/SelectBox/Overview/"
}

#####See Also#####
#include common-link-setupdevextreme
#include common-link-configurewidget