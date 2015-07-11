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
