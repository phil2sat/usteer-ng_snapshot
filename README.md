# usteer-ng

usteer-ng is a client steering daemon written for OpenWrt and the a fork of the famous [usteer steering deamon](https://openwrt.org/packages/pkgdata/usteer).

Its goal is to optimize roaming/band steering behavior of wireless clients (STAs) in a ESS consisting of multiple BSS / APs.

## Functions

 - Synchronization of Neighbor Reports between multiple APs
 - Policy-based decisions for probe- / association- / authentication requests received from STAs
 - Requesting clients to roam to a different BSS based on SNR / signal-level
 - Channel-load based client steering to different BSS
 - Band steering to higher bands if possible
 - Using different level of aggressiveness

## Installation

usteer-ng is available from the OpenWrt packages feed and can be installed on devices running OpenWrt 21.02+ using opkg. Usteer-ng is conflicting to Usteer as it actually based on the same code. Also it does not make sense to have two Wifi controllers installed.

```
opkg update; opkg install usteer-ng
```

## Submitting patches

usteer-ng is fully managed in Github. Please contribute via Pull-Requests to the "development" branch.