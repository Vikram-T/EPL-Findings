# EPL-Findings

This repo is split into two sections

1. Internet in a box experiments
2. Jitsi network tests


## Networking tools used
* iperf3
  * Used to determine the max throughput between two connections
* netdata
  * Provides really good visualizations of everything happening on the computer
  * Used for visualizing network usage/bandwidth
* FireHol/fireqos
  * Used for traffic shaping, can artifically limit bandwidth to simulate a lower bandwidth network
  * A rapper around tc
