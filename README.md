# kiyung_calamares_user_module
This module is an extension of the calamares/src/module/users module to autofill an existing user id name on the "users" page of the istaller.
## Feature
By using this users module, the calamares installer will be able to automatically detect the host user id. If the host id already existed, this module will get the id name and display it on the username box.

Modifications have been made in UserPage.cpp. getlogin() in unistd.h has been included to return the existing user id. 

'''cpp
    // auto fill username
    if( getlogin() != NULL)
    {
        QString auto_userName( getlogin() );
        ui->textBoxFullName->setText( auto_userName );
    }
'''
## Instructions
Clone this module to your calamares/src/modules direcory and replace it with calamares/src/modules/users directory
