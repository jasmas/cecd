cecd & piRemote
===============

cecd is an init script which can be used to run the cec-client utility from the
[libCEC][1] project as a daemon to provide an IP bridge for sending CEC commands
over an HDMI interface attached to the host. A telnet session to the configured
port will allow access to an interactive cec-client remotely. This script
requires [libCEC][1], including the cec-client utility, and [socat][2]. Default
runlevels and command-line options for cec-client are intended for running cecd
on a Raspberry Pi, but may be modified to run in any environment supported by
libCEC with an attached HDMI interface, supporting CEC.

piRemote is a distribution of device codes for [Roomie Remote][3] for use with
the Roomie Remote application and a Raspberri Pi running cecd and attached to
the HDMI interface of a TV supporting CEC. Adding the Raspberri Pi as a
piRemote device in Roomie Remote will allow IP control for switching the TV
on, putting it into standby and toggling between HDMI inputs. Instructions for
adding custom device codes to Roomie Remote can be found [here][4].

[1]: http://libcec.pulse-eight.com
[2]: http://freecode.com/projects/socat
[3]: http://www.roomieremote.com
[4]: http://www.roomieremote.com/support/#customDevice

