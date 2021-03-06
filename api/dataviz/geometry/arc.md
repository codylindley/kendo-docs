---
title: Arc
page_title: API reference for methods and fields of Kendo UI DataViz Geometry Arc
---

# kendo.dataviz.geometry.Arc

Represents an arc with set center, direction, angular range and x/y radius.

## Example - Creating an arc
        <script>
            var geo = kendo.dataviz.geometry;
            var center = [10, 10];
            var arc = new geo.Arc(center, {
                radiusX: 10,
                radiusY: 5,
                startAngle: 90,
                endAngle: 270,
                anticlockwise: false
            });
        </script>

## Fields

### anticlockwise `Boolean` *(default: false)*

A flag indicating if the arc should be drawn in clockwise or anticlockwise direction.
Defaults to clockwise direction.


### center `kendo.dataviz.geometry.Point`

The location of the arc center.


### endAngle `Number`

The end angle of the arc in decimal degrees.
Measured in clockwise direction with 0 pointing "up".
Negative values or values greater than 360 will be normalized.


### radiusX `Number`

The x radius of the arc.


### radiusY `Number`

The y radius of the arc.


### startAngle `Number`

The start angle of the arc in decimal degrees.
Measured in clockwise direction with 0 pointing "up".
Negative values or values greater than 360 will be normalized.


## Methods

### bbox

Returns the bounding box of this arc after applying the specified transformation matrix.

#### Parameters

##### matrix `kendo.dataviz.geometry.Matrix`

Transformation matrix to apply.

#### Returns

`kendo.dataviz.geometry.Rect` The bounding box after applying the transformation matrix.


### getAnticlockwise

Gets the arc anticlokwise flag.

#### Returns

`Boolean` The anticlokwise flag of the arc.


### getCenter

Gets the arc center location.

#### Returns

`kendo.dataviz.geometry.Point` The location of the arc center.


### getEndAngle

Gets the end angle of the arc in decimal degrees.
Measured in clockwise direction with 0 pointing "up".

#### Returns

`Number` The end angle of the arc.


### getRadiusX

Gets the x radius of the arc.

#### Returns

`Number` The x radius of the arc.


### getRadiusY

Gets the y radius of the arc.

#### Returns

`Number` The y radius of the arc.


### getStartAngle

Gets the start angle of the arc in decimal degrees.
Measured in clockwise direction with 0 pointing "up".

#### Returns

`Number` The start angle of the arc.


### pointAt

Gets the location of a point on the arc's circumference at a given angle.

#### Parameters

##### angle `Number`

Angle in decimal degrees. Measured in clockwise direction with 0 pointing "up".
Negative values or values greater than 360 will be normalized.

#### Returns

`kendo.dataviz.geometry.Point` The point on the arc's circumference.


### setAnticlockwise

Sets the arc anticlokwise flag.

#### Parameters

##### value `Boolean`

The new anticlockwise value.

#### Returns

`kendo.dataviz.geometry.Arc` The current arc instance.


### setCenter

Sets the arc center location.

#### Parameters

##### value `kendo.dataviz.geometry.Point`

The new arc center.

#### Returns

`kendo.dataviz.geometry.Arc` The current arc instance.


### setEndAngle

Sets the end angle of the arc in decimal degrees.
Measured in clockwise direction with 0 pointing "up".

#### Parameters

##### value `Number`

The new arc end angle.

#### Returns

`kendo.dataviz.geometry.Arc` The current arc instance.


### setRadiusX

Sets the x radius of the arc.

#### Parameters

##### value `Number`

The new arc x radius.

#### Returns

`kendo.dataviz.geometry.Arc` The current arc instance.


### setRadiusY

Sets the y radius of the arc.

#### Parameters

##### value `Number`

The new arc y radius.

#### Returns

`kendo.dataviz.geometry.Arc` The current arc instance.


### setStartAngle

Sets the start angle of the arc in decimal degrees.
Measured in clockwise direction with 0 pointing "up".

#### Parameters

##### value `Number`

The new arc atart angle.

#### Returns

`kendo.dataviz.geometry.Arc` The current arc instance.

