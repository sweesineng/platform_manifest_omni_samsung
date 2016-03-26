Getting Started

To get started with OMNI sources to build Samsung devices, you'll need to get familiar with Git and Repo.

To initialize your local repository using the OMNIROM trees to build Samsung, use a command like this:

repo init -u git://github.com/sweesineng/platform_manifest_omni_samsung.git -b <<branch>>
Then to sync up:

repo sync
Then to build:

 cd <source-dir>; . build/envsetup.sh; lunch omni_<device>-eng; mka recoveryimage
