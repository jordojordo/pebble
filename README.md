# Pebble

Setup a fresh Raspberry Pi with pi-hole using Ansible.

## Usage

First you'll need a new instance of Ubuntu installed on an SD for the Raspiberry Pi. You can install it with [RPI Imager](https://www.raspberrypi.com/software/).

Once the image has been copied, mount the drive and copy the `user-data` config file from the repo into the boot partition of SD card.

Boot the Raspberry Pi. You will need the secret key from when you created a key during the setup. It will take ≈10-15 minutes to complete the setup.

You will find the provisioning and troubleshooting logs at `/var/log/ansible-provision.run` and `/var/log/cloud-init-output.log`.

After the seed node is finished installing you can access it at `<SEED_ID>>@<PUBLIC_ADDR>:<PORT>`. If you didn't set a `public_addr` you can find it at your Raspberry's IP.
