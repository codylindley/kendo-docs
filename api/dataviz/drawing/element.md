---
title: Element
page_title: Configuration, methods and events of Kendo UI DataViz Drawing Element
---

# kendo.dataviz.drawing.Element

An abstract base class representing common members of all drawing elements.

## Constructor Parameters

### options `Object`
The configuration of this Group.

## Fields

### options `kendo.dataviz.drawing.OptionsStore`

The configuration options of the drawing element.

## Configuration

### transform `kendo.dataviz.geometry.Transformation`
The transformation to apply to this element.

### visible `Boolean`
A flag, indicating if the element is visible.

## Methods

### bbox
Returns the bounding box of the element.

Transformations on the parent, or the element itself are applied
before calculating the bounding box.

#### Returns
`kendo.dataviz.geometry.Rect` The bounding box of the element with all transformations applied.


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

