---
title: GridColumnSortable
---

# \Kendo\UI\GridColumnSortable

A PHP class representing the sortable setting of GridColumn.


## Methods

### compare
A JavaScript function which is used to compare the values - should return -1 if first argument is less than second one, 0 if both are the same or +1 if the first one is greater than second one.

#### Returns
`\Kendo\UI\GridColumnSortable`

#### Parameters

##### $value `\Kendo\JavaScriptFunction`



#### Example 
    <?php
    $sortable = new \Kendo\UI\GridColumnSortable();
    $sortable->compare(new \Kendo\JavaScriptFunction('function() { }'));
    ?>

