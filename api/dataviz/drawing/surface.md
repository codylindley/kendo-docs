---
title: Surface
page_title: Configuration, methods and events of Kendo UI DataViz Drawing Surface
---

# kendo.dataviz.drawing.Surface

An abstract class representing the top-level drawing surface.
This class can't be instantiated directly.

Specific implementations are created via the static `create` method.
The implementations for SVG, Canvas and VML inherit from this base class.

## Example - Creating a drawing surface

        <div id="container" style="position: relative; width: 600px; height: 400px;"></div>
        <script>
            var d = kendo.dataviz.drawing;
            var surface = d.Surface.create($("#container"));
        </script>

## Class methods

### create

Creates a drawing surface matching the browser capabilities.

#### Example - Creating a surface with any available type

        <div id="container"></div>
        <script>
            var d = kendo.dataviz.drawing;
            var surface = d.Surface.create($("#container"));
        </script>

#### Example - Specifying a preferred type and size

        <div id="container"></div>
        <script>
            var d = kendo.dataviz.drawing;
            var surface = d.Surface.create($("#container"), {
                type: "canvas",
                width: "600px",
                height: "400px"
            });
        </script>

#### Parameters

##### element `Element`

The DOM (or jQuery) element that will host the surface.

##### options `Object`

The options to pass to the surface.
This parameter can be omitted.

#### Returns

`kendo.dataviz.drawing.Surface` An implementation matching the browser capabilities or caller preference; undefined if none is available.


## Configuration

### type `String`

The preferred type of surface to create.
Used only by Surface.create, will be ignored by the actual Surface implementation.

### height `String` *(default: "100%")*

The height of the surface element.
By default the surface will expand to fill the height of the first positioned container.

### width `String` *(default: "100%")*

The width of the surface element.
By default the surface will expand to fill the width of the first positioned container.

## Events

### click

Triggered when an element has been clicked.

> The Canvas drawing surface does not fire events.

#### Example - subscribe to the "click" event during initialization

        <div id="container"></div>
        <script>
            var d = kendo.dataviz.drawing;
            var surface = d.Surface.create($("#container"), {
                click: function(e) {
                    var element = e.element;
                }
            });
        </script>

#### Event Data

##### e.element `kendo.dataviz.drawing.Element`

The clicked element.

##### e.originalEvent `Object`

The browser event that triggered the click.

### mouseenter

Triggered when the mouse is moved over an element.

> The Canvas drawing surface does not fire events.

#### Example - subscribe to the "mouseenter" event during initialization

        <div id="container"></div>
        <script>
            var d = kendo.dataviz.drawing;
            var surface = d.Surface.create($("#container"), {
                mouseenter: function(e) {
                    var element = e.element;
                }
            });
        </script>

#### Event Data

##### e.element `kendo.dataviz.drawing.Element`

The target element.

##### e.originalEvent `Object`

The browser event that triggered the click.

### mouseleave

Triggered when the mouse is leaves an element.

> The Canvas drawing surface does not fire events.

#### Example - subscribe to the "mouseleave" event during initialization

        <div id="container"></div>
        <script>
            var d = kendo.dataviz.drawing;
            var surface = d.Surface.create($("#container"), {
                mouseleave: function(e) {
                    var element = e.element;
                }
            });
        </script>

#### Event Data

##### e.element `kendo.dataviz.drawing.Element`

The target element.

##### e.originalEvent `Object`

The browser event that triggered the click.

## Methods

### clear

Clears the drawing surface.

### draw

Draws the element and its children on the surface.
Existings elements will remain visible.

#### Parameters

##### element `kendo.dataviz.drawing.Element`

The element to draw.

### resize

Resizes the surface to match the size of the container.

#### Parameters

##### force `Boolean` *optional*

Whether to proceed with resizing even if the container dimensions have not changed.

