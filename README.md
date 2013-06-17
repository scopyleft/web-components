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
