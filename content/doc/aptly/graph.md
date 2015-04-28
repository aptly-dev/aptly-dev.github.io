---
date: "2014-08-08T11:17:38Z"
title: "aptly graph"
menu:
    doc:
        parent: Commands
        weight: 70
---

aptly graph
-----------

aptly generates graph showing depedencies between mirrors, local repositories,
snapshots and published repositories.
 

Command graph generates graph of dependencies:

* between snapshots and mirrors (what mirror was used to create each snapshot)
* between snapshots and local repos (what local repo was used to create snapshot)
* between snapshots (pulling, merging, etc.)
* between snapshots, local repos and published repositories (how snapshots were published).

Graph is rendered to PNG file using graphviz package.

Usage:

    $ aptly graph

Flags:

-   `-format="png"`: graph output format, could be anything graphviz supports, e.g. `png`, `pdf`, `svg`, ...


Example:

<a href="/img/graphfull.png"><img src="/img/graph.png" alt="Example graph from aptly graph" class="img-responsive"></a>
 