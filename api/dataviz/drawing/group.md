---
title: Group
page_title: API reference for methods and fields of Kendo UI DataViz Drawing Group
---

# kendo.dataviz.drawing.Group
Represents a set of drawing elements, possibly including other groups.

## Constructor Parameters

### options `Object`
The configuration of this Group.

## Configuration

### transform `kendo.dataviz.geometry.Transformation`
The transformation to apply to the children of this group.

### visible `Boolean`
A flag, indicating if the children are visible.

## Fields

### children `Array`
The children of this group.

## Methods

### append
Appends the specified element as a last child of the group.

#### Parameters

##### element `kendo.dataviz.drawing.Element`
The element to append. Multiple parameters are accepted.


### bbox
Returns the bounding box (rectangle) of the group.

Transformations on the parent, the group itself and its children are applied
before calculating the bounding box.

#### Returns
`kendo.dataviz.geometry.Rect` The bounding box of the group with all transformations applied.


### clear
Removes all child elements from the group.


### remove
Removes the specified element from the group.

#### Parameters

##### element `kendo.dataviz.drawing.Element`
The element to remove.


### removeAt
Removes the child element at the specified position.

#### Parameters

##### index `Number`
The index at which the element currently resides.


### transform
Gets or sets the transformation of the element.

#### Parameters

##### transform `kendo.dataviz.geometry.Transformation`
The transformation to apply to the element.

#### Returns
`kendo.dataviz.geometry.Transformation` The current transformation on the element.


### visible
Gets or sets the visibility of the element.

#### Parameters

##### visible `Boolean`
A flag indicating if the element should be visible.

#### Returns
`Boolean` true if the element is visible; false otherwise.

