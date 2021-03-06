sigma.helpers.graph
==================

Plugin developed by [Sébastien Heymann](https://github.com/sheymann) for [Linkurious](https://github.com/Linkurious) and published under the licence [GNU GPLv3](LICENSE) unless otherwise noticed by Linkurious.

---
## General
This plugin extends the [Graph API](https://github.com/jacomyal/sigma.js/wiki/Graph-API) with new public methods:

**dropNodes( *string|number* )** : *graph*
**dropNodes( *array* )** : *graph*
 * This methods is used to drop a node or a set of nodes from the graph, depending on how it is called. The method must be called with an array of node IDs.

**dropEdges( *string|number* )** : *graph*
**dropEdges( *array* )** : *graph*
 * This methods is used to drop an edge or a set of edges from the graph, depending on how it is called. The method must be called with an array of edge IDs.

**adjacentNodes( *string|number*, *?object* )** : *array*
 * This methods is used to retrieve the adjacent nodes of a specified node from the graph. The method must be called with the ID of a node. Set the optional object property `withHidden` to `false` to get non-hidden nodes only.

**adjacentEdges( *string|number*, *?object* )** : *array*
 * This methods is used to retrieve the adjacent edges of a specified node from the graph. The method must be called with the ID of a node. Set the optional object property `withHidden` to `false` to get non-hidden edges only.

**fixNode( *string|number* )** : *graph*
 * This methods will set the value of `fixed` to `true` on a specified node. The method must be called with the ID of a node.

**unfixNode( *string|number* )** : *graph*
 * This methods will set the value of `fixed` to `false` on a specified node. The method must be called with the ID of a node.

**hasFixedNodes()** : *boolean*
 * This methods returns true if fixed nodes exist.

**getFixedNodes()** : *array*
 * This methods returns the list of fixed nodes.

See the following [unit tests](../../test/unit.helpers.graph.js) for full usage.

To use, include all .js files under this folder.
