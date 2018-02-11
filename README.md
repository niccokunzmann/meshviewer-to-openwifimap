# meshviewer-to-openwifimap

An application to post https://github.com/ffrgb/meshviewer data to the https://openwifimap.net.
This way, we can have all the data of the free nodes available which run a mesh viewer instance.

## Implementation

The mesh viewer downloads the nodes from a json file.

Examples
- http://map.erfurt.freifunk.net/meshviewer/nodes.json
- https://regensburg.freifunk.net/data/meshviewer.json

We translate these nodes to the format proposed by the openwifimap.
https://github.com/freifunk/openwifimap-api/blob/master/API.md

The basic implementation would get the nodes and provide neccessary information about them.

Tools
- a file named `meshviewer-nodes-list.txt` which includes a mesh viewer nodes json from various places
- a script getting the nodes and posting them
- a travis build which runs daily to update the database

