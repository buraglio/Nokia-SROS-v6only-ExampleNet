# Nokia-SROS-v6only-ExampleNet

### Nokia PCE Segment Routing testing in a v6 only context
Included here are the Test configurations for MPLS testing with Nokia SROS and JunOS as well as the Topology and Eve-NG Lab XML File. This repo consists of a 4 Router Lab utilizing Nokia SROS 16 and SROS 20 for testing.

### Files and such

1. flatten.sh - A script that takes the SROS configuration and converts it to a paste-able, flattened format. Requires https://github.com/door7302/transcode-sros
2. files named .flat.txt - flattened filed produced by the above script
3. vsr* Nokia SROS configurations as stored in the flash. Usable in the "startup configuration" for Eve-NG
5. Nokia Lab.unl - the Eve-NG XML file that is the lab

### Route creation
* Route generation is provided by a goBGP instance running on an ubuntu VM. Details and instructions for re-creating that configuration can be found [here](https://github.com/buraglio/bgp-injector)

### Diagrams and physical layout

The Physical layout of this test environment is detailed in this diagram. This was built on EVE-NG bare metal server with significant horsepower.
![Physical lab Topology](https://github.com/buraglio/Nokia-SROS-ExampleNet/blob/master/Network%20Diagram.png?raw=true "Physical Lab Topology")
