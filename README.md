# gst_ds_env
My gstreamer deepstream container image setup repo.

If you're wanting to use this go to https://github.com/pwolfe8/gst_ds_examples

## Install Prereqs on Host

### Jetson
run the `./host_setup/first_time_setup.sh` script

### Desktop
Assuming you have a Ubuntu 20.04 Desktop (or 18.04 probably) with an NVIDIA GPU.
Install the recommended nvidia drivers for you GPU using `./host_setup/desktop_scripts/install_nvidia_drivers_desktop.sh` 

Then reboot your machine with `sudo reboot`

Now run the `./host_setup/first_time_setup.sh` script

## Build Options
```bash
# automatically detect host architecture and if nvidia-docker2 packages is installed
./build.sh

# override build choice:
./build.sh jetson # other options include jetson_nogpu, desktop, desktop_nogpu
```