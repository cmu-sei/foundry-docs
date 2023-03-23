# Challenge

The **Challenge** page in the Topo workspace is used when both Gameboard and TopoMojo are integrated to execute a cyber competition. More information on linking those two applications together can be found elsewhere in the Foundry documentation. The Challenge page is where you create random key/values, embed them in a *gamespace* at deploy time, and ask questions of competitors (players).

## Transforms

## Markdown

## Variants

A *variant* describes a different version of a challenge. Variants can contain different ISO attachments, different virtual machines, and different questions and answers. Each time a challenge is deployed, a variant is randomly selected for the deployment. For example, two competitors can attempt the same challenge, but one competitor may receive *variant #1* and the other competitor may receive *variant #2*.  When creating a challenge using variants, make sure all variants test the same competitor skills at the same difficulty level. That is, variant #1 should test the same skills as variant #2 and one variant shouldn't be harder to solve than another variant.

### Show Variant Detail

**Detail:**

**Clone:** 

**Remove:**

**Markdown:**

**Iso:** TopoMojo does allow you to attach a variant-specific ISO file to "target" templates. To attach an ISO file  to a subset of VMs only when deployed in a gamespace:

1. On the **Challenge** tab, enable **Show Variant Detail**. 

2. Under **Iso**, select an ISO file. This is the file you'll attach to the VM target.

3. Under **Targets**, specify the VMs that should have the ISO attached when a gamespace is deployed. 

A different ISO can be defined for each variant. 

**QuestionSet:**
