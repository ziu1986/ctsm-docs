Get CTSM 
=========

Get CTSM for running (no source changes)
-----------------------------------------

If you are a novice, that's where you should start. You get the source code and run it as is.

NordicESMhub maintains a CTSM repository with all the configuration files for running on machines in the Nordics. For now we support:

- saga (sigma2, Norway)
- fram (sigma2, Norway)

If your machine is not in the list and you would like us to support it, please contact us.

How to get CTSM
++++++++++++++++

For compatibility, load git version 2.23.0 or higher

::

    git/2.23.0-GCCcore-8.3.0

CLONE from GitHub

::

    git clone -b release-clm5.0 https://github.com/NordicESMhub/ctsm.git ${HOME}/ctsm
   
In this example we are checking out the release-clm5.0 tag and create a new local branch (recomended).
The destination of the checkout is a directoy (eg. ctsm) in our home directory. 

How to get a specific branch
+++++++++++++++++++++++++++++

Check all existing branches

::

    git branch --all

To run FATES EMERALD platform (in this example release 2.0.1)

::

    git checkout release-emerald-platform2.0.1 -b new_branch_name

Which branch do I run?
++++++++++++++++++++++


Get CTSM for modifying the source code
-----------------------------------------

Create your own branches before continuing, in ~/ctsm AND in ~ctsm/cime. Do this for FATES or any other modules in addition.
    
::

    git checkout fates_emerald_api -b new_branch_name # useful for remembering version, name according to function e.g. username_cime_clm5.0.12 and username_fates_clm5.0.12
    git branch # to verify that you are on the branch you just created

When you need to do your own development.
