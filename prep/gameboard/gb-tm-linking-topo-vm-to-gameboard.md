# Linking a TopoMojo VM to the Gameboard

## Create the datastore

<!--Get Matt or Jarrett to help with this section.-->

### On the TopoMojo side

These procedures assume you've got the datastore established and you are logged into a correctly deployed instance of TopoMojo. In TopoMojo:

1. Create a new workspace.

2. On the Files tab, drag and drop a virtual machine iso. <!--Where do they get the ISOs?-->

3. Click Settings, and complete the following fields: 

   - Title: Give your new workspace a name.
   - Audience: Enter "gameboard" here. This shares the workspace with the gameboard app. Audience is set on the gameboard side. 

Completing the other fields is optional. 

4. Click Templates. Add a blank template, click Edit to change attributes like Name, Description, Network, etc. Add whichever .iso file you uploaded into the iso field in the steps above.
5. Unlink the VM. 
6. Click *initialize*, then *deploy*. <!--Matt configured Alpine in the VM console here - will others have to do the same after deploying? Different instructions for different OS's?-->
7. Save the VM. At this point, the VM is part of the challenge. Next, you'll add it to a gameboard.

### On the Gameboard side

These procedures assume you are logged into a correctly deployed instance of Gameboard and have been given the appropriate role. In Gameboard:

1. Click **Admin**, then **+New game**.
2. Expand Settings. Minimally, complete the following fields:
   - Closes time
   - Session Duration
   - Session Limit
   - Gamespace Limit
   - Max submissions
3. Under Registration, Access, select Open. Complete Opens, Closes,  Minimum Team Size, and Maximum Team Size.
4. Expand Map, then click Search. The challenge created in Topomojo should appear under the Search field.
5. Add the challenge to the map. 
6. Enter a Support Key and Points value.

The Challenge should appear on the map now.

## Additional info

<!--Get with Matt or Jarrett on this, but this should probably be moved up under ESXi.-->

- - **setting up Topomojo & ESXi to talk properly is likely the largest hurdle present:**
    - "if you're working with that you'll either need a system that runs ESXi or you run the ESX nested hypervisor that the foundry docs call out"
      - `foundry.local/start/esxi` exists on the appliance and explains how to set things up
    - fair amount of resources are necessary if using a laptop, but running really lightweight VMs for testing is an option/a solution

- **Running Topomojo locally rather than in the appliance & trying to set it up with ESX:**
  - Adapt the `topomojo.values.yaml` around line 144
    - `Core__ConsoleHost:`
    - all of the lines immediately after that start with `Pod`
      - eg: `Pod__Url:`, `Pod__User:`, etc.