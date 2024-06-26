# Home Assistant Add-on: AMR2MQTT

[![GitHub Release][releases-shield]][releases]
![Project Stage][project-stage-shield]
[![License][license-shield]](LICENSE)

![Project Maintenance][maintenance-shield]
[![Community Forum][forum-shield]][forum]

_Runs rtlamr to read meter data and send to MQTT broker._

## About

Allows you to use an rtl-sdr dongle to listen for signals from ERT compatible
smart meters using [rtlamr][rtlamr]. This runs as a daemon by launching rtl-tcp
and rtlamr, parsing the output and pushing it into MQTT so Home Assistant can
consume it.

This began as a port of ragingcomputer's [amridm2mqtt][amridm2mqtt] to a Home
Assistant add-on in order to make it easier to use in HAOS and supervised setups.
There are a number of other modifications as well such as support for other formats
like `scm` and a wider variety of MQTT configurations. Big thanks to ragingcomputer's
for their work as well as all the info in the `rtlamr` repo.

## Support

Got questions?

You have several ways to get them answered:

- The Home Assistant [Community Forum][forum].
- The Home Assistant [Discord Chat Server][discord-ha]. Use the #add-ons channel.

You could also [open an issue here][issue] on GitHub.

## Authors & contributors

The original setup of this repository is by [Mike Degatano][mdegat01].

The amridm2mqtt service this was built off of was created by [ragingcomputer][ragingcomputer].

For a full list of all authors and contributors,
check [the contributor's page][contributors].

## License

MIT License

Copyright (c) 2021-2022 Mike Degatano

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[project-stage-shield]: https://img.shields.io/badge/project%20stage-production%20ready-brightgreen.svg
[amridm2mqtt]: https://github.com/ragingcomputer/amridm2mqtt
[contributors]: https://github.com/Arschoepf/addon-amr2mqtt/graphs/contributors
[discord-ha]: https://discord.gg/c5DvZ4e
[forum-centralcommand]: https://community.home-assistant.io/u/CentralCommand/?u=CentralCommand
[forum-shield]: https://img.shields.io/badge/community-forum-brightgreen.svg
[forum]: https://community.home-assistant.io/t/home-assistant-add-on-amr2mqtt/378196
[mdegat01]: https://github.com/Arschoepf
[issue]: https://github.com/mdegat01/addon-amr2mqtt/issues
[license-shield]: https://img.shields.io/github/license/Arschoepf/addon-amr2mqtt.svg
[maintenance-shield]: https://img.shields.io/maintenance/yes/2022.svg
[ragingcomputer]: https://github.com/ragingcomputer
[releases-shield]: https://img.shields.io/github/release/Arschoepf/addon-amr2mqtt.svg
[releases]: https://github.com/Arschoepf/addon-amr2mqtt/releases
[rtlamr]: https://github.com/bemasher/rtlamr
