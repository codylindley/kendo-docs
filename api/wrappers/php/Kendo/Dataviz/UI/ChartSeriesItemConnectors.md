---
title: ChartSeriesItemConnectors
slug: php-dataviz-ui-chartseriesitemconnectors
tags: api, php
publish: true
---

# \Kendo\Dataviz\UI\ChartSeriesItemConnectors

A PHP class representing the connectors setting of ChartSeriesItem.


## Methods

### color
The color of the connector line.

#### Returns
`\Kendo\Dataviz\UI\ChartSeriesItemConnectors`

#### Parameters

##### $value `string`



#### Example 
    $connectors = new \Kendo\Dataviz\UI\ChartSeriesItemConnectors();
    $connectors->color('value');

### padding
The padding between the connector line and the label, and connector line and donut chart.

#### Returns
`\Kendo\Dataviz\UI\ChartSeriesItemConnectors`

#### Parameters

##### $value `float`



#### Example 
    $connectors = new \Kendo\Dataviz\UI\ChartSeriesItemConnectors();
    $connectors->padding(1);

### width
The width of the connector line.

#### Returns
`\Kendo\Dataviz\UI\ChartSeriesItemConnectors`

#### Parameters

##### $value `float`



#### Example 
    $connectors = new \Kendo\Dataviz\UI\ChartSeriesItemConnectors();
    $connectors->width(1);
