# vmdkReader
.Net 4.0 Console App to read and extract files from vmdk images

Uses https://github.com/DiscUtils/DiscUtils lib to parse the vmdk images.

Useful in cases where the vmdk is on the network and you only want to copy a single file instead of GBs (e.g ntds.dit), since it does not transfer the whole disk over the network.

Project uses:
* Quamotion.DiscUtils.Core
* Quamotion.DiscUtils.Ntfs
* Quamotion.DiscUtils.Streams
* Quamotion.DiscUtils.Vmdk

and ILMerge 3.0.29 & ILMerge.MSBuild.Task to bundle the required dlls. Generated file < 1024kb

WARNING - tested only with specific vmdk images and network latencies

C# console app to read and extract files from vmdk images 
