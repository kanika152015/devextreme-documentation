---
id: dxTreeList
module: ui/tree_list
export: default
inherits: GridBase
---
---
##### shortDescription
The TreeList is a UI component that represents data from a local or remote source in the form of a multi-column tree view. This UI component offers such features as sorting, filtering, editing, selection, etc.

##### widgettree
dataSource: 
[{
      id:1, parentId: 0, fullName:"John Heart", position:"CEO", email:"jheart@dx-email.com"
    }, {
      id:2, parentId: 1, fullName:"Samantha Bright", position:"COO", email:"samanthab@dx-email.com"
    }, {
      id:3, parentId: 1, fullName:"Arthur Miller", position:"CTO", email:"arthurm@dx-email.com"
    }, {
      id:4, parentId: 1, fullName:"Robert Reagan", position:"CMO", email:"robertr@dx-email.com"
    }, {
      id:5, parentId: 2, fullName:"Greta Sims", position:"HR Manager", email:"gretas@dx-email.com"
}],
autoExpandAll: true,
showRowLines: true,
columns: ["position", "fullName", "email"]

##### lib
dx.web.js, dx.all.js

---
#include common-tutorialbutton with {
    url: "/Documentation/Guide/UI_Components/TreeList/Getting_Started_with_TreeList/" 
}

#include btn-open-demo with {
    href: "https://js.devexpress.com/Demos/WidgetsGallery/Demo/TreeList/Overview/"
}

#####See Also#####
#include common-link-setupdevextreme
#include common-link-configurewidget