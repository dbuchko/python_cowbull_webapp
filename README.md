# python_cowbull_webapp

To deploy the webapp client on Pivotal Cloud Foundry:
* Run the `build-pcf.sh` shell script to download the vendor app dependencies
* Edit `COWBULL_SERVER` variable in the `manifest.yml` to point to the Cowbull Server app URL.
* Run `cf push` from the project root directory.
