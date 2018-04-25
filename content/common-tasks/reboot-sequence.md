+++
title = "Reboot Sequence"
chapter = true
weight = 103
+++

# Reboot Sequence

When things go really wrong, it may be necessary to turn everything off and on again.

Only shut down by holding down the power button in dire circmustances.

This is also useful when a power outage affects the station and the UPS runs out of power.

## Systems must be started in order of dependance
Most services should be configured to startup automatically after boot

1. FS0
2. DPS0
3. RAW
4. WP-GW*
5. LOG1
5.1. run ~/run_darkice.py as root on LOG1
6. LOG2
6.1. run ~/run_darkice.py as root on LOG2
7. VM1

* WP-GW needs to be started up in a particular way
(to be added)
