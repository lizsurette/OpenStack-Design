# Undercloud Install and Preparation by Preparation Expert</br>
Before the edge technician (Jacques) can do his job of installing the OpenStack Overcloud at an edge site, the undercloud needs to be installed and some configuration work needs to take place. This is not part of Jacques role and is captured below as part of a workflow done by what we are calling the "Preparation Expert".

[Preparation Expert Persona - TBD](TBD)

## Identify and Prepare Hardware for Undercloud
![undercloudhardwareprep](img/2017-7-24 TripleO UI_13_PrepWork3.png)
- The Preparation Expert needs to identify and prepare the hardware they will be using to install the undercloud on. They will refer to guidance on what the specifications need to be for this hardware.

## Install Undercloud
![installundercloud](img/2017-7-24 TripleO UI_13_PrepWork4.png)
- The first step of installing the undercloud is to clone and run the TripleO Quickstart project.

## Clone Heat Templates
![cloneheattemplates](img/2017-7-24 TripleO UI_13_PrepWork5.png)
- The Preparation Expert clones the heat templates that are provided by the TripleO project so that they can make any edits needed for the configuration for their overcloud environment.

## Edit Heat Templates
![editheattemplates1](img/2017-7-24 TripleO UI_13_PrepWork6.png)
- Any configuration updates that need to be made should be changed in the YAML files. This includes Network and Storage configuration changes along with creating or editing any custom roles that will be used.

![editheattemplates2](img/2017-7-24 TripleO UI_13_PrepWork7.png)

![editheattemplates3](img/2017-7-24 TripleO UI_13_PrepWork8.png)

![editheattemplates4](img/2017-7-24 TripleO UI_13_PrepWork9.png)

## Optionally Create JSON File for Hardware
![JSONfileforhardware](img/2017-7-24 TripleO UI_13_PrepWork10.png)
- The Preparation Expert could optionally create a JSON file based on the hardware that will be registered at the Edge Site. This is something that could be uploaded by the deployer while registering nodes to make it quicker to register in bulk.

## How Would this Flow look in the UI?

The preparation expert could use the UI to do all of these steps after prepping their undercloud hardware and installing the undercloud. Here is what that flow could look like in the UI...

![login](img/2017-7-24 TripleO UI_13_PrepWork12.png)
- After logging in, the user would be dropped into the Plans card views. This would show any default plans that are available on a clean install.

![planscardview](img/2017-7-24 TripleO UI_13_PrepWork13.png)
- At this point, the Preparation Expert would create a new plan so that they could define the specifics for what will be deployed at the Edge Site.

![createnewplan](img/2017-7-24 TripleO UI_13_PrepWork14.png)
- On creation of a Plan, the user can choose high level configuration options.  

![editroles](img/2017-7-24 TripleO UI_13_PrepWork15.png)
- Part of the overall configuration includes role selection and creation.
- Since this deployment will be an HCI deployment, the user is going to remove the default Compute and Storage roles and go ahead and create custom role for HCI.

![createnewrole](img/2017-7-24 TripleO UI_13_PrepWork16.png)
- The Preparation Expert

![undercloudhardwareprep](img/2017-7-24 TripleO UI_13_PrepWork17.png)
- The Preparation Expert

![undercloudhardwareprep](img/2017-7-24 TripleO UI_13_PrepWork18.png)
- The Preparation Expert

![undercloudhardwareprep](img/2017-7-24 TripleO UI_13_PrepWork19.png)
- The Preparation Expert

![undercloudhardwareprep](img/2017-7-24 TripleO UI_13_PrepWork20.png)
- The Preparation Expert  

![undercloudhardwareprep](img/2017-7-24 TripleO UI_13_PrepWork21.png)
- The Preparation Expert

![undercloudhardwareprep](img/2017-7-24 TripleO UI_13_PrepWork22.png)
- The Preparation Expert

![undercloudhardwareprep](img/2017-7-24 TripleO UI_13_PrepWork23.png)
- The Preparation Expert

![undercloudhardwareprep](img/2017-7-24 TripleO UI_13_PrepWork24.png)
- The Preparation Expert

![undercloudhardwareprep](img/2017-7-24 TripleO UI_13_PrepWork25.png)
- The Preparation Expert

![undercloudhardwareprep](img/2017-7-24 TripleO UI_13_PrepWork26.png)
- The Preparation Expert  

![undercloudhardwareprep](img/2017-7-24 TripleO UI_13_PrepWork27.png)
- The Preparation Expert
