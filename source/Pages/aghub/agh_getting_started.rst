.. _agh_getting_started:

*******************
AGH Getting Started
*******************


---------------
Quick Overview
---------------

The Alzheimers Genetics Hub (AGH) is a secure compute environment based largely from a clone of the Spider cluster at SURF.

-----------------------------------
Join the Collaborative Organization
-----------------------------------

Accept invitation e-mail from SRAM

`afterwards it can take 15 minutes for the system to sync`


------------------------
Set-up AGH User Account
------------------------

1. Go to [portal](https://portal.cua.surf.nl) and change password from e-mail / accept SURF Usage agreement
2. Set up [2fa token](https://2fa.surfsara.nl/)


---------------------------------
2-Step Login (doornode --> aghub)
---------------------------------


First step log-into the doornode with password set in the SURF portal
`ssh sram-aghub-[First initial][Last name]@doornode.surfsara.nl`

After logging into the doornode, select aghub which should appear in a single select list

Re-enter the password from the portal
Enter the OTP you registered earlier

Success if logging in succeeded you should see the AGHub banner

----------------------
Initalize your account
----------------------

To facilitate setting up your account, we recommend you run the following command:

.. code-block:: bash

    /project/aghub/Share/init/init.sh
    

This script will do the following:

* It will copy a conda environment to your home folder, and add it to your path. This conda environment contains 
many useful packages, both general software and software for dealing with genetics data.

* It will also create a folder in your home directory `rd` which will be used to mount the
research drive. 

* It will create a bin folder in your home directory, to which it will add some useful scripts

* It will setup your bashrc, vimrc and screenrc files with useful defaults. 


The next step now is to setup your research drive mount: :ref:`_agh_research_drive`.

Afterwards, you can find out how to install new software: :ref:`_agh_installing_software`.

----------------------
Get started with SLURM
----------------------

After getting access to the cluster, please refer to our Spider documentation for submitting your first jobs:
`Spider Documentation <https://wiki.surfnet.nl/display/SRAM/Invite+admins+and+members+to+a+collaboration/>`_ 










