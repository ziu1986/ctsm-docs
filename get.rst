Get CTSM 
=========

Get CTSM for running (no source changes)
-----------------------------------------

If you are a novice, that's where you should start. You get the source code and run it as is.

NordicESMhub maintains a CTSM repository with all the configuration files for running on machines in the Nordics. For now we support:

- saga (sigma2, Norway)
- fram (sigma2, Norway)

If you machine is not in the list and would like we support it, please contact us.

How to get CTSM
++++++++++++++++

For compatibility, load git version 2.23.0 or higher

::

    git/2.23.0-GCCcore-8.3.0

CLONE from GitHub (run only first time, or to update clm/ctsm version), in home folder

::

    git clone -b release-clm5.0 https://github.com/NordicESMhub/ctsm.git

OBS! Before building your CTSM case make sure you unload (purge) all loaded modules.

::

    module purge

CHECK loaded modules
		 
::

    module list


How to get a specific branch
+++++++++++++++++++++++++++++


Which branch do I run?
++++++++++++++++++++++


Get CTSM for modifying the source code
-----------------------------------------

Create your own branches before continuing, in ~/ctsm AND in ~ctsm/cime. Do this for FATES or any other modules in addition.
    
::

    git branch <username_clm5.0.12>   # useful for remembering version, name according to function e.g. username_cime_clm5.0.12 and username_fates_clm5.0.12
    git checkout  <username_clm5.0.12>
    git branch # to verify that you are on the branch you just created

When you need to do your own development.
