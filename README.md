# k8e-vagrant

Vagrant box with wireguard, openvpn and GUI

## Start From Scratch

* ```vagrant up``` if VM not yet running
* Set password if not set because required for GUI login
  * ```vagrant ssh``` Get shell
  * ```sudo passwd vagrant``` Reset password
* ```vagrant reload``` if GUI not showing

## Useful keys

* right-ctrl is default host key
* host+f => Full Screen
* host+m => Minimize

## Setup VPN

### OpenVPN

* Extract VPN profile and passcode from Proton (Or other provider)
* Put passcode and config in directory that becomes /vagrant directory
* Import an existing config
* Set perms to global afterwards

### Wireguard

## Todo

* UDP OpenVPN fails on some nat + Virtualbox configurations (Maybe all) revisit.
