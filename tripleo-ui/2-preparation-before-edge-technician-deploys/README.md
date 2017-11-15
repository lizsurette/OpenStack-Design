# Undercloud Install and Preparation by Preparation Expert
Before the edge technician (Jacques) can do his job of installing the OpenStack Overcloud at an edge site, the undercloud needs to be installed and some configuration work needs to take place. This is not part of Jacques role and is captured below as part of a workflow done by what we are calling the "Preparation Expert". Read more about this persona here:

Preparation Expert Persona (TBD)

## Identify and Prepare Hardware for Undercloud
![undercloudhardwareprep](img/2017-7-24-TripleO-UI_13_PrepWork3.png)
- The Preparation Expert needs to identify and prepare the hardware they will be using to install the undercloud on. They will refer to guidance on what the specifications need to be for this hardware.

## Install Undercloud
![installundercloud](img/2017-7-24-TripleO-UI_13_PrepWork4.png)
- The preparation expert can install the undercloud in a number of different ways. One of these options is to clone and run the TripleO Quickstart project. Other options include using the RDO Quickstart or if a Red Hat customer, the guides provided with a Red Hat subscription.

## Clone Heat Templates
![cloneheattemplates](img/2017-7-24-TripleO-UI_13_PrepWork5.png)
- The Preparation Expert clones the heat templates that are provided by the TripleO project so that they can make any edits needed for the configuration for their overcloud environment.

## Edit Heat Templates
![editheattemplates1](img/2017-7-24-TripleO-UI_13_PrepWork6.png)
- Any configuration updates that need to be made should be changed in the YAML files. This includes Network and Storage configuration changes along with creating or editing any custom roles that will be used.

![editheattemplates2](img/2017-7-24-TripleO-UI_13_PrepWork7.png)

![editheattemplates3](img/2017-7-24-TripleO-UI_13_PrepWork8.png)

![editheattemplates4](img/2017-7-24-TripleO-UI_13_PrepWork9.png)

## Register & Introspect Nodes
![registernodes](img/2017-7-24-TripleO-UI_13_PrepWork10.png)
- At this point, if the user wants to test their configuration before sending it to the Edge Technician for use, they could register nodes and move forward with a test deployment.

## Assign Nodes to Roles
![assignnodestoroles](img/2017-7-24-TripleO-UI_13_PrepWork11.png)
- By updating the node count for each role, the user is assigning these nodes to the specific roles before deployment.

## Deploy
![deploy](img/2017-7-24-TripleO-UI_13_PrepWork12.png)
- The user can run the deploy command at this point to test that the deployment configuration will work on their test hardware.

## Export Plan
![deploy](img/2017-7-24-TripleO-UI_13_PrepWork13.png)
- At any point, the user can export a deployment plan.
- This will support the use cases where one deployment plan might want to be used for multiple sites. The Edge Technician can simply import the deployment plan and then use it to deploy the overcloud at their site.

## How Would this Flow look in the UI?

The preparation expert could use the UI to do all of these steps after prepping their undercloud hardware and installing the undercloud. Here is what that flow could look like in the UI...

![login](img/2017-7-24-TripleO-UI_13_PrepWork15.png)
- After logging in, the user would be dropped into the Plans card views. This would show any default plans that are available on a clean install.

![planscardview](img/2017-7-24-TripleO-UI_13_PrepWork16.png)
- At this point, the Preparation Expert would create a new plan so that they could define the specifics for what will be deployed at the Edge Site.

![createnewplan](img/2017-7-24-TripleO-UI_13_PrepWork17.png)
- On creation of a Plan, the user can choose high level configuration options.  

![editroles](img/2017-7-24-TripleO-UI_13_PrepWork18.png)
- Part of the overall configuration includes role selection and creation.
- Since this deployment will be an HCI deployment, the user is going to remove the default Compute and Storage roles and go ahead and create custom role for HCI.

![createnewrole1](img/2017-7-24-TripleO-UI_13_PrepWork19.png)
- Creating a new role will pull up another window that allows the user to define that role.

![createnewrole2](img/2017-7-24-TripleO-UI_13_PrepWork20.png)
- Roles can be given a name, description, and need to be assigned to a flavor.
- Services can be selected that will be used in this role.
- Based on the services selected, the parameters below will be built out.

![createplan](img/2017-7-24-TripleO-UI_13_PrepWork21.png)
- Once the user has finalized the high level plan details, they can confirm the creation of the plan.

![plancardsview2](img/2017-7-24-TripleO-UI_13_PrepWork22.png)
- After creating the plan, the user will see it listed in the card view. Clicking on the card will drill into the detailed workflow of that plan.

![plandetails](img/2017-7-24-TripleO-UI_13_PrepWork23.png)
- At this point, the user could choose to edit the Network and Storage configuration for this plan.

![editconfiguration1](img/2017-7-24-TripleO-UI_13_PrepWork24.png)
- The first step of this wizard would be the overall network configuration.

![editconfiguration2](img/2017-7-24-TripleO-UI_13_PrepWork25.png)
- The second step includes assigning roles to subnets.

![editconfiguration3](img/2017-7-24-TripleO-UI_13_PrepWork26.png)
- The third network configuration step covers any changes that the user might want to make to the subnet configuration.

![editconfiguration3](img/2017-7-24-TripleO-UI_13_PrepWork27.png)
- Storage configuration changes can be made here and the user can save all of the configuration changes that have been made.

![validationsrunning](img/2017-7-24-TripleO-UI_13_PrepWork28.png)
- Validations may kick off after certain changes are made to the deployment configuration.

![validations1](img/2017-7-24-TripleO-UI_13_PrepWork29.png)
- The user can click to view the entire list of validations.

![validations2](img/2017-7-24-TripleO-UI_13_PrepWork30.png)
- For each validation, the high level status is listed along with a way for the user to drill into the details of the validation.

![validationdetails](img/2017-7-24-TripleO-UI_13_PrepWork31.png)
- The validation details will give the user a better idea as to what has happened if a validation failed.

![registernodes](img/2017-7-24-TripleO-UI_13_PrepWork32.png)
- If the user wants to check that the configuration is working, they can begin the process of doing a test deployment by registering nodes.

![registernodesmodal](img/2017-7-24-TripleO-UI_13_PrepWork33.png)

![assignnodestoroles](img/2017-7-24-TripleO-UI_13_PrepWork34.png)
- At this point, the user would need to assign the registered nodes to the roles that they want them to play in the deployment.

![deploy](img/2017-7-24-TripleO-UI_13_PrepWork35.png)
- Now the deployment is ready to kickoff.

![deployconfirmation](img/2017-7-24-TripleO-UI_13_PrepWork36.png)
- The user will get a confirmation modal before deployment officially starts.

![successfuldeploy](img/2017-7-24-TripleO-UI_13_PrepWork37.png)
- After a successful deployment, the user will have access to the overcloud.

![exportplan](img/2017-7-24-TripleO-UI_13_PrepWork38.png)
- At any point, the user can export a deployment plan.
- This will support the use cases where one deployment plan might want to be used for multiple sites. The Edge Technician can simply import the deployment plan and then use it to deploy the overcloud at their site.
