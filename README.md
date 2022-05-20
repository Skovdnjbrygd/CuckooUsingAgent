# CuckooUsingAgent
A collection of scripts to install Cuckoo Sandbox automated malware analysis system, but it is required to manually build the agent (analysis) machine.

Sometimes it is required to build a malware analysis environment with very specific needs. In this case the automated creation of analysis machines with VMCloak may not be desirable. 
There are also instances where VMCloak may fail to automatically install specific packages without saying why (this happened to me with adobepdf and dotnet).

If you are going to manually start the analysis VM anyways to install packages that were supposed to be automatically installed, you might as well build the whole thing yourself. 
Just create a windows7 machine named agent.ova and keep it in the same directory where you run the scripts. Refer to the cuckoo user manual on specifics steps how to build the analysis. 
Refer to agent.ova_specifications.txt to see my hardware provisioning for the VM. 

Also as a side note, I couldn't get screenshots to work with the VMCloak generated machines, but it works right out the box when I manually build the analysis machine.

TLDR: I got annoyed with VMCloak not installing all the packages I selected from the supported list, and I couldn’t get screenshots to work either. This repo is a way to install Cuckoo Sandbox with a virtual analysis machine the user has custom built according to the Cuckoo manual instructions. 
Just name it agent.ova.
