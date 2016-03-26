## Getting Started ##
---------------

To get started with OMNI sources to build Samsung devices, you'll need to get familiar with Git and Repo.

To initialize your local repository using the OMNIROM trees to build Samsung, use a command like this:
```bash
repo init -u git://github.com/sweesineng/platform_manifest_omni_samsung.git -b android-4.4
```
Then to sync up:
```bash
repo sync -j4 -f --no-clone-bundle
```
Configure ccache
```bash
echo "export USE_CCACHE=1" >> ~/.bashrc
 ~/android/omni/prebuilts/misc/linux-x86/ccache/ccache -M 25G
```

Then to build, ex Samsung GT-N7000
```bash
 . build/envsetup.sh
 breakfast n7000
 brunch n7000
```
