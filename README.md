# Web Components

A collection of web components using the [Polymer lib](http://www.polymer-project.org/).

**Because Web Components are the future of the Web (and we want to be part of it).**

## Installation

    $ git clone git://github.com/scopyleft/web-components.git
    $ cd web-components
    $ git clone git://github.com/Polymer/polymer-all.git --recursive
    $ python3 -m http.server 8765
    (or $ python -m SimpleHTTPServer 8765)
    $ open http://127.0.0.1:8765/

## Components

### `github-repository`

Displays a github-like summary for a given repository. Inspired by [GitHub-jQuery-Repo-Widget](https://github.com/JoelSutherland/GitHub-jQuery-Repo-Widget).

Attributes:

* **repository** (required): a string containing `repository owner`/`repository name`
* **width** (optional, default=`500px`): a string setting the width of the component with the related unit.

### `trello-card`

Displays a Trello card from a public board.

Attributes:

* **cardId** (required): a string containing the Trello card id
* **trelloKey** (required): a string containing the Trello key [available for developers](https://trello.com/1/appKey/generate)
* **width** (optional, default=`500px`): a string setting the width of the component with the related unit.

### `feed-box`

Work in progress.


### `x-map`

Displays a [Leaflet](http://leafletjs.com/) map.

`x-map` attributes:

* **lat** (required): the latitude where to center
* **lng** (required): the longitude where to center
* **zoom** (optional, default=`12`): The zoom level
* **width** (optional, default=`200`): The width of the map in pixels
* **height** (optional, default=`200`): The height of the map in pixels
* **credit** (optional): A text (HTML allowed) to insert into the footer of the map.

#### `x-marker`

You can also insert markers inside an `x-map`:


    <x-map lat="43.656291" lng="3.89034">
        <x-marker lat="43.610772" lng="3.876715">
            <h1>City of Montpellier</h1>
        </x-marker>
    </x-map>


`x-marker` attributes:

* **lat** (required): the latitude where to place the marker
* **lng** (required): the longitude where to place the marker
* **open** (optional): if specified and the node as a content, the content will be rendered in an open popup.

> Note that an x-marker can have an optional content inside its node. It will be rendered as a popup that will open on click (or open on load if the `open` attribute is specified)

