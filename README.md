tracelytics-openstack
=====================

Patches to add Tracelytics Oboe middleware to Openstack

Installing Tracelytics
======================

See http://support.tracelytics.com/kb/installation-instructions/installation-overview

Patching Openstack
==================

Per the documentation on the Tracelytics knowledgebase it is necessary insert the OboeMiddleware into any components you wish to trace. Patches are included in this repository to demonstrate how this can be acheived. The patches were written against Devstack and may require some modifications to work as the codebase progresses.

Patching Tracelytics
====================

In order to collect full controller and action detail from Openstack it is necessary to make a minor alteration to the OboeMiddleware which was designed to work with pylons. There is an example of how to make this change provided in this repository.
