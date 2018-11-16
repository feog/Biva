# Biva
A tool for Bitcoin Network Visualization &amp; Analysis

This contains a jupyter demo for some basic Bitcoin visualization and analytics.

The demo assumes that the Bitcoin data is stored in the graph database Neo4j. The first notebook explains how the data was uploaded into Neo4j, under which format.

The second notebook contains the code for the user interface and some graph algorithms. Python queries Neo4j via some cypher magic, then once the data is retrieved, a graph representing it is displayed using python-igraph, the graph data in the Python code is mostly handled by NetworkX. 

Disclaimer: the purpose of this code is to provide a visual interface for understanding the Bitcoin network, and to do some basic Bitcoin forensics, by following the flow of Bitcoins. However is it just a small demo, which works fine, but may not be bugfree (in particular the zoom button could do with some debugging but the functionality itself is not needed for the demo). Most importantly, the code could do with a LOT of improvement: 
* The queries to Neo4j should be better written (which means learning cypher)
* The user interface should be rewritten in a clean way
However, none of the above will happen because by now, JupyterLab is available, so I would rather rewrite the code using JupyterLab than rewriting the code in a cleaner manner for the notebook.
