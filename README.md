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
* Click on people icon on password and select store password for all users
* Use ```sudo nmcli connection modify $iface ipv4.route-metric 0``` so it can get out because the virtualbox stuff has a priority of zero for the NATed interface

### Wireguard

## Todo

* UDP OpenVPN fails on some nat + Virtualbox configurations (Maybe all) revisit.
