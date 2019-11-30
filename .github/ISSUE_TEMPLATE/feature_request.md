---
name: Feature request
about: Ability to select multiple extentions in FileMask
title: ''
labels: enhancement
assignees: ''

---

** v0.8.8.0 **
The version of KAPE you are currently using

****

I've created a custom target file(.tkape) with most required filesystem artifacts for me, and it runs like a champ. However i dont feel that good when it comes to modules. Since the modules mostly relayed on 'FileMask' parameter, there's no way currently to create a custom single module file (.mkape). Wish if there an option to comma seperate the FileMask, i could have customize the entire processing with one .tkape and one .mkape files.



**Describe the solution you'd like**
Option to add comma seperated extensions in mkape files.

**Describe alternatives you've considered**
NA.

**Additional context**

Ex:

Description: 'MFTECmd: process $MFT files'
Category: FileSystem
Author: Eric Zimmerman
Version: 1
Id: 7ef84a6b-5215-46bb-af2a-3339a3227e25
BinaryUrl: https://f001.backblazeb2.com/file/EricZimmermanTools/MFTECmd.zip
ExportFormat: csv
FileMask: $MFT, $J, $Secure_$SDS
Processors:
    -
        Executable: MFTECmd.exe
        CommandLine: -f %sourceFile% --csv %destinationDirectory%
        ExportFormat: csv
Regards,
Suresh Krishnan
