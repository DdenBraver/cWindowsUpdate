# cWindowsUpdate

The **cWindowsUpdate** module contains the **cWindowsUpdate** and **cMicrosoftUpdate** DSC resources.
**cWindowsUpdate** installs a Windows Update (or hotfix) from a given path. For more information on Windows Update and Hotfix, please refer to [this TechNet article](http://technet.microsoft.com/en-us/library/cc750077.aspx).
**cMicrosoftUpdate** enables or disables Microsoft Update.

## Resources

### cWindowsUpdate

* **Path**: The path from where the hotfix should be installed
* **Log**: The name of the log where installation/uninstallation details are stored. 
If no log is used, a temporary log name is created by the resource. 
* **Id**: The hotfix ID of the Windows update that uniquely identifies the hotfix.
* **Ensure**: Ensures that the hotfix is **Present** or **Absent**. 
* **Reboot**: If set to true, it will notify the computer that a reboot is required after a change has happened.

### cMicrosoftUpdate

* **Ensure**: Determines whether the MS Update should be enabled (ensure) or disabled (absent)

## Versions

### 2.2.0.2

* Added reboot switch to **cWindowsUpdate** resource.
* Minor updates to examples files

### 2.2.0.0

* Cloned resource from cWindowsUpdate

