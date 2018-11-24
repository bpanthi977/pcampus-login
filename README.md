# pcampus-login

Shell script to automatically login to Pulchowk Campus Wifi. 

# Requirements
* `curl` : To make network requests (Mostly probably installed in your system )
* `NetworkManager` : To automatically dispatch the login script on network connection. (Also installed in most systems)

# Use

* Clone this repo 
`git clone https://github.com/bpanthi977/pcampus-login`

* Edit the `pcampus-login` file and save your username and password.
* Run the install script 
`sudo ./install.sh`

# Note 
* don't add `.sh` extension to `pcampus-login` file. 
* login `curl` command is executed for ethernet connection only. If you want to execute it for your wireless device too (or your ethernet device name is not `enp4s0`), edit the `pcampus-login` file and change the device name at `$1 = "enp4s0"` position.

You can find your device name by running `ifconfig` at the shell.

