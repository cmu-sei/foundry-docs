# Admin Workspaces

The **Workspaces** tab is where the admin can search for workspaces. Once workspaces are found, the admin can perform limited actions. This is useful because...

Use the **Search** field to locate a workspace. Selecting a workspace takes you the **Settings** tab of that particular workspace. For additional help on the **Settings** tab, see [Building a new workspace](/tm-building-a-workspace.md).

The *workspace identifier* is present here too. The workspace identifier matches the directory name used to store workspace files like unlinked virtual machines, Markdown documents, images, etc. Copying it to the clipboard is useful if you need to use it in a terminal when navigating the filesystem. The workspace identifier is called out in the screen capture below.

![tm-wksp-iden](img/wksp-iden.png)

## View (expanded)

**Template Limit:**

**Template Scope:**

**Audience:**

**VMs:**

<!--what are we doing here that is different from "building a workspace"?-->

**Refresh**: (arrows) Refresh queries the state of the VM from the hypervisor. This is useful if you run a `shutdown` command in the VM and the TopoMojo UI icons haven't updated to reflect the powered off state of the VM yet. 

**Deploy**: (lightning bolt) Deploys that virtual machine into your workspace.

**Console:** Opens the console for the virtual machine.

**Stop/Start:** Power off/on the VM, but leaves the resource deployed on the hypervisor. Clicking **stop** results in the hypervisor showing a deployed VM in a powered off state.  Clicking **start** powers on the deployed VM.

**Revert:** Reverts the VM to its last saved state. All changes made since the last commit are lost.

**Delete:** Deletes a running VM instance. Before you click **delete**, make sure you have saved any changes to the disk.

**Save:** The **save** icon appears only when an unlinked disk is being used; changes can't be saved to a linked disk. The **save** icon removes the last disk snapshot and creates a new snapshot that saves all changes made to the VM.