Content Delivery Network (CDN) Latency Analysis:

The goal of a CDN is to serve content to end-users with high availability and high performance.

In this project, we are going to answer the following question:

Where do we deploy a new CDN server???

Methodology
====================================================
1- CDNs collection
2- Choosing candidates
3- Collecting ping data
4- Building the graph
5- Visualization

Packages
======================
(1) networkX, (2) pandas



CODE FILES
======================

getPingInfo.py:

	-Collected ping data from each current CDN to all the candidates
	-Ran the script at each virtual machine
	-Transmit 5 packages and extract the average ping time

createGraph.py: 

	-Merged results for each virtual machine (CDN)
	-Final graph has 105 nodes and 776 edges

====================================================
Here is a list of virtual machines in different geographical regions, selected from Microsoft Azure Cloud Computing Platform
![Alt text](Presentation/cdns.png?raw=true "Search box")

Here is a list of candidate locations for new CDN deployment:

![Alt text](Presentation/candidates.png?raw=true "Results page")

Here is the result. The big purple star, is the suitable location for deploying new CDN.

![Alt text](Presentation/results.png?raw=true "Results page")



