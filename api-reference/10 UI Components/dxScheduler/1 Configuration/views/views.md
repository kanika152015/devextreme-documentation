---
id: dxScheduler.Options.views
acceptValues: 'day' | 'week' | 'workWeek' | 'month' | 'timelineDay' | 'timelineWeek' | 'timelineWorkWeek' | 'timelineMonth' | 'agenda'
type: Array<String, Object>
default: ['day', 'week']
---
---
##### shortDescription
Specifies and configures the [views](/concepts/05%20UI%20Components/Scheduler/060%20Views/010%20View%20Types '/Documentation/Guide/UI_Components/Scheduler/Views/View_Types/') to be available in the [view switcher](/concepts/05%20UI%20Components/Scheduler/070%20View%20Switcher.md '/Documentation/Guide/UI_Components/Scheduler/View_Switcher/').

---
This property accepts an array of strings and objects:

- **String**        
A view name. Use a string if the view does not need customization, but should be available in the view switcher.

- **Object**        
An individual view's configuration. Set the [type](/api-reference/10%20UI%20Components/dxScheduler/1%20Configuration/views/type.md '/Documentation/ApiReference/UI_Components/dxScheduler/Configuration/views/#type') property to specify the view to which the configuration should apply. This documentation section describes available properties. The properties set for an individual view have a higher priority than the same properties set on the root level for all views.

        <!-- tab: JavaScript-->views: [{
                type: 'workWeek',
                name: 'Vertical Grouping',
                groupOrientation: 'vertical',
                cellDuration: 60,
                intervalCount: 2,
            }, {
                type: 'workWeek',
                name: 'Horizontal Grouping',
                groupOrientation: 'horizontal',
                cellDuration: 30,
                intervalCount: 2,
            },
            'agenda'
        ]

To specify the default view, use the [currentView](/api-reference/10%20UI%20Components/dxScheduler/1%20Configuration/currentView.md '/Documentation/ApiReference/UI_Components/dxScheduler/Configuration/#currentView') property.

#include btn-open-demo with {
    href: "https://js.devexpress.com/Demos/WidgetsGallery/Demo/Scheduler/CustomizeIndividualViews/"
}

#include btn-open-github with {
    href: "https://github.com/DevExpress-Examples/devextreme-scheduler-disable-dates-in-timelines-view"
}
