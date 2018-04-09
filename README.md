## TripleO UI Design Documentation

The following is the documented design for the two main workflows that we are looking to support in the TripleO UI along with the edge cases that users might hit.

#### 1. [Deployment Workflow for Edge Technician](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/1-deployment-workflow-for-edge-technician/)
A walkthrough of what Jacques the Edge Technician will see as he works through Deploying the Overcloud using the UI.


#### 2. Preparation before Edge Technician Deploys
A walkthrough of what the preparation expert needs to do to get the undercloud install done and configuration prepared for before Jacques installs at edge sites.
- [Preparation before Edge Technician Deploys using the CLI](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/2-preparation-before-edge-technician-deploys/1.usingcli)
- [Preparation before Edge Technician Deploys using the UI](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/2-preparation-before-edge-technician-deploys/2.usingui)

#### 3. TripleO UI Edge Cases
Users might high a number of Edge Cases in the UI. Edge cases are the less likely path, but still something we'd like to support a user of the UI to tackle.
- [View Plan History](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/1.viewplanhistory)
- [Create New Role (Shuttle Selection)](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/2.createnewrole)
- [View Service Status](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/3.viewservicestatus)
- [View About Information](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/4.viewaboutinformation)
- [Manually Add and Configure Infrastructure](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/5.manuallyaddandconfigureintrospectiondetails)
- [Information Hover Over](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/6.informationhoverover)
- [Advanced Network Configuration and Network Topology](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/7.advancednetworkconfigurationandtopology)
- [HCI Deployment Workflow including Advanced Storage Configuration](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/8.advancedstorageconfiguration)
- [Manually Assign Nodes](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/9.manuallyassignnodes)
- [Import Validation](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/10.importvalidation)
- [Monitor a Deployment In Progress](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/11.monitordeploymentinprogress)
- [View Nodes List](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/12.viewnodeslist)
- [Localization](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/13.localization)
- [View Details on a Truncated Error Message](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/14.viewdetailstruncatederror)
- [Access Node Terminal](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/15.accessnodeterminal)
- [Run Validations in Bulk](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/16.runvalidationsinbulk)
- [Alternate Network Topology View - Nodes](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/17.alternatenetworktopologynodes)
- [Create/Update Deployment Plan](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/18.createupdateplan)
- [Notifications](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/19.notifications)
- [Export Plan](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/20.exportplan)
- [Register Large Number of Nodes](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/21.registerlargenumbernodes)
- [Define Custom Hostnames](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/22.customhostnames)
- [Predictable IPs](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/23.predictableips)
- [Predictable VIPs](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/24.predictablevips)
- [Network Plugins](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/3-tripleo-ui-edge-cases/25.networkplugins)

#### 4. OpenShift on OpenStack
There are two methods that a user might choose to deploy OpenShift on OpenStack. The first is to run OpenShift as a Tenant on top of OpenStack. The second is to define a role and use bare-metal nodes to run OpenShift.
- [OpenShift on OpenStack - Tenant](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/4-openshift-on-openstack/1.OpenShiftAsTenant)
- [OpenShift on OpenStack - Bare-Metal](https://lizsurette.github.io/OpenStack-Design/tripleo-ui/4-openshift-on-openstack/2.OpenShiftOnBareMetal)
