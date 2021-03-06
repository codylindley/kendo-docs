---
title: TreeMapBuilder
---

# Kendo.Mvc.UI.Fluent.TreeMapBuilder
Defines the fluent API for configuring the Kendo TreeMap for ASP.NET MVC.




## Methods


### AutoBind(System.Boolean)
If set to false the widget will not bind to the data source during initialization. In this case data binding will occur when the change event of the
            data source is fired. By default the widget will bind to the data source specified in the configuration.


#### Parameters

##### value `System.Boolean`
The value that configures the autobind.





### ValueField(System.String)
The data item field which contains the tile value.


#### Parameters

##### value `System.String`
The value that configures the valuefield.





### ColorField(System.String)
The data item field which contains the tile color.


#### Parameters

##### value `System.String`
The value that configures the colorfield.





### TextField(System.String)
The data item field which contains the tile title.


#### Parameters

##### value `System.String`
The value that configures the textfield.





### Template(System.String)
The template which renders the treeMap tile content.The fields which can be used in the template are:


#### Parameters

##### value `System.String`
The value that configures the template.





### TemplateId(System.String)
The template which renders the treeMap tile content.The fields which can be used in the template are:


#### Parameters

##### value `System.String`
The value that configures the template.





### Colors(System.String[])
The default colors for the treemap tiles. When all colors are used, new colors are pulled from the start again.


#### Parameters

##### value `System.String[]`
The value that configures the colors.





### DataSource(System.Action\<Kendo.Mvc.UI.Fluent.HierarchicalDataSourceBuilder\<System.Object\>\>)
Configure the DataSource of the component


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.HierarchicalDataSourceBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/HierarchicalDataSourceBuilder)<System.Object>>
The action that configures the M:Kendo.Mvc.UI.Fluent.TreeMapBuilder.DataSource(System.Action{Kendo.Mvc.UI.Fluent.HierarchicalDataSourceBuilder{System.Object}}).




#### Example (ASPX)
    <%= Html.Kendo().TreeMap()
    .Name("treeMap")
    .DataSource(dataSource => dataSource
        .Read(read => read
            .Action("_PopulationUS", "TreeMap")
        )
    )
    %>


### Events(System.Action\<Kendo.Mvc.UI.Fluent.TreeMapEventBuilder\>)
Configures the client-side events.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.TreeMapEventBuilder](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/TreeMapEventBuilder)>
The client events action.




#### Example (ASPX)
    <%= Html.Kendo().TreeMap()
    .Name("TreeMap")
    .Events(events => events
        .DataBound("onDataBound")
    )
    %>


### Colors(System.Action\<Kendo.Mvc.UI.Fluent.TreeMapColorRangeFactory\>)
The default colors for the treemap tiles. When all colors are used, new colors are pulled from the start again.


#### Parameters

##### configurator System.Action<[Kendo.Mvc.UI.Fluent.TreeMapColorRangeFactory](/api/wrappers/aspnet-mvc/Kendo.Mvc.UI.Fluent/TreeMapColorRangeFactory)>
The add action.






