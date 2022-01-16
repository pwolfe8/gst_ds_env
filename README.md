# gst_ds_env
my gstreamer deepstream container environments

## Host Prereq Installs
see `setup_host` folder

## Use Container
```bash
# example to build container on jetson using GPU passthrough
./build.sh jetson # other choices: nongpu_jetson, desktop, nongpu_desktop
./run.sh
./attach.sh

# to remove after you're done
./remove.sh
```
