# kiyung_calamares_user_module
This module is an extension of the calamares/src/module/users module to autofill an existing user id name on the "users" page of the istaller.
* * *
## Feature
By using this users module, the calamares installer will be able to automatically detect the host user id. If the host id already existed, this module will get the id name and display it on the username box.

* ### Demonstration
    The following video demonstrates shortly how this extension would work on an environment that already contains the user id.    
    Click [here](https://www.youtube.com/watch?v=Ye19DK44Wdc) to view the demonstration.
    
* * *
## Instructions
Clone this module to your calamares/src/modules direcory and replace it with calamares/src/modules/users directory. Then, build Calamares as shown in <https://github.com/calamares/calamares/wiki/Develop-Guide>. 
