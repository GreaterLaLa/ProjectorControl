# ProjectorControl
Controlling the Projectors from the Raspberry Pis

## Modules

These modules use the [Net::PJLink](https://metacpan.org/pod/Net::PJLink) module, which is a pure Perl implementation of the PJLink protocol used by the Mitsubishi projectors that are part of our project.

To install this module, use CPAN:

    cpan Net::PJLink

## Programs

There are two programs in this repo: projector_on.pl and projector_off.pl.

These are simply named: `projector_on.pl` turns the projector on, and `projector_off.pl` turns the projector off. There is no `projector_status.pl`; it might not be possible by the protocol.

Each Raspberry Pi controls it's own projector, the IP address has to be set for each projector.

## Project

This code was developed to service [GreaterLaLa](http://greaterlala.in/). We installed two Mitsubishi projectors and controlled them with a Netgear five-port switch and two Raspberry Pis. We went with the Raspberry Pis because of the low cost, and because small, single board computers would more easily handle the install environment than more standard computers, with cooling fans and moving parts and such. The Mitsubishi projectors were chosen because they were available from Purdue Surplus, take an HDMI input and are controllable via IP network.

The MatchBox gateway has a pair of ports that forward to the Pis, and each Pi in turn controls the projector it connects to, more as a bookkeeping measure than anything.

Those IP addresses and the default password hard-coded into the program, so the addresses need to be changed per Pi.
