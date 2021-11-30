# 1.​ Survey of NSI and SENSE software
This document contains a list of software packages currently available for the AutoGOLE project supporting the NSI and SENSE protocols.

## ​1.1.​ nsi-requester
The SURFnet NSI web client supports the NSI CS 2.1 protocol.  Simple but functional.
 
Very stable.

[https://github.com/BandwidthOnDemand/nsi-requester](https://github.com/BandwidthOnDemand/nsi-requester)

## ​1.2.​ nsi-safnari
The SURFnet NSI aggregator.  Fully implements the NSI CS 2.1 protocol.  Requires deployment of the nsi-pce and nsi-dds software.

Very stable.  Small bug fixes over the last few years as more usage find small protocol compliance issues.

[https://github.com/BandwidthOnDemand/nsi-safnari](https://github.com/BandwidthOnDemand/nsi-safnari)

## ​1.3.​ nsi-pce
The NSI Path Computation Engine implements a series of NSI 2.1 specifications needed to realize a functional aggregator NSA.  The PCE core provides a RESTful interface for requesting path resolution within a network of NSI Connection Service enabled domains. The NSI Topology Service provides an NSI Topology compliant service with an independent RESTful interface giving access to discovered network topology.

Very stable.  There have been almost no changes over the last few years, however, we need a complete rewrite of memory management associated with the graph.  It was fine for a small AutomatedGOLE, but as the network grew so did memory utilization. 

[https://github.com/BandwidthOnDemand/nsi-pce](https://github.com/BandwidthOnDemand/nsi-pce)

## ​1.4.​ nsi-dds
The ESnet implementation of the NSI Document Distribution Protocol provides services to an aggregator NSA for collection and distribution of NSI related documents (NSA and  NML topology).

Very stable.  Changes have been minimal in the last few years.  Mostly corner case bug fixes.

[https://github.com/BandwidthOnDemand/nsi-dds](https://github.com/BandwidthOnDemand/nsi-dds)

## ​1.5.​ OSCARS
ESnet’s bandwidth-on-demand system implementing the uPA portion of the NSI CS 2.1 protocol.

[https://github.com/esnet/oscars](https://github.com/esnet/oscars)
​
## ​1.6.​ OpenNSA
NORDUnet’s implementation of the uPA portion of the NSI CS 2.0 protocol (not the current 2.1 release).  It was designed to talk to a single switch, forcing users to expose a network topology per switch.  New aggregation features have been added, however, these are not compliant to the NSI CS definition of aggregator, and is really still a uPA with additional functionality.

Stability of OpenNSA is an issue.  There are a number of bugs and deficiencies that force applications to code specific handling not compliant to the NSI CS protocol.

[https://github.com/nordunet/opennsa](https://github.com/nordunet/opennsa)
​
## ​1.7.​ Add Japanese and Korean NSA information
Add text here…
​
## ​1.8.​ sense-nsi-rm
This is an ESnet implementation of a SENSE Resource Manager (RM) that will convert between the SENSE protocol and a standard NSI CS 2.1 protocol.  This functionality also creates associated MRML resource documents by combining information from the NSI NML topology representation, and  NSI CS 2.1 reservation information.

Stable releases available. Software is undergoing regular changes to address compatibility issues between SENSE and NSI, as well as buggy NSA implementations.

[https://github.com/esnet/sense-rm](https://github.com/esnet/sense-rm)
​
## ​1.9.​ sense-nrm-oscars
This is an ESnet implementation of a SENSE Resource Manager (RM) that will convert between the SENSE protocol and the OSCARS northbound interface.

Very stable.

[https://github.com/esnet/sense-nrm-oscars](https://github.com/esnet/sense-nrm-oscars)
​
## ​1.10.​ SENSE-O
The SENSE Orchestrator (SENSE-O), a component within this overall SENSE system, is responsible for processing user service requests, computing workflows, and interacting with SENSE Resource Managers (RMs) to provision end-to-end resources.

Under development.  Stable releases available.

[Document repository](https://github.com/esnet/SENSE-Orchestrator)

[SENSE-O source code](https://github.com/esnet/StackV)

