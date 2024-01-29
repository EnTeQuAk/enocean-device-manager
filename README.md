[![Generic badge](https://img.shields.io/github/commit-activity/y/grimmpp/home-assistant-eltako.svg?style=flat&color=3498db)](https://github.com/grimmpp/home-assistant-eltako/commits/main)
[![Generic badge](https://img.shields.io/badge/Community-Forum-3498db.svg)](https://community.home-assistant.io/)
[![Generic badge](https://img.shields.io/badge/Community_Forum-Eltako_Integration_Debugging-3498db.svg)](https://community.home-assistant.io/t/eltako-baureihe-14-rs485-enocean-debugging/49712)
[![Generic badge](https://img.shields.io/badge/License-MIT-3498db.svg)](/LICENSE)
[![Generic badge](https://img.shields.io/badge/SUPPORT_THIS_PROJECT-PayPal.me-27ae60.svg)](https://paypal.me/grimmpp)

# Enocean Device Manager and Home Assistant Configuration Exporter

# WORK IN PROGRESS!!! NOT YET RELEASE READY!!!

This client application allows you to **inventory all EnOcean devices**. It can **automatically read and detect devices** from the RS485 bus or from wireless network. After the devices are listed in the EnOcean Device Manager **you can enricht device information** like changing the name, comment or adapt parameters like timeframes, thresholds, units, ... .
Furthermore, it automatically can detect default settings for Home Assistant configuration which can be adjust as well and it allows you to **generate and export the configuration for Home Assistant**. 
(The exported Home Assistant configuration is intended for the [Eltako Home Assistant Integration](https://github.com/grimmpp/home-assistant-eltako/))

## Preview
<img src="./screenshot.png" /> 
What you can see here can automatically detected by reading the memory of the bus devices via FAM14. Telegrams of sensors and decentralized devices will be received and additionally added. 
Additional info for Home Assistant is automatically added. The configuration for Home Assistant can be generated by the detected information.
For further steps it is planned to extend the support for changing the data which was collected so that a proper management of the devices can be supported.

## Install dependencies and run the App
1. Clone/Download the repo.
2. Change into the repo directory.
3. Create virtual environment for python: `python.exe -m venv .venv`
4. Install dependencies: `.\.venv\Scripts\pip.exe install -r .\requirements.txt` (This step takes a bit.)
5. Start the app: `.\.venv\Scripts\python.exe main.py`

For update you can execute:
1. `git pull` (Gets newest state of the code)
2. `.\.venv\Scripts\pip.exe install -r .\requirements.txt` installs changes of dependencies. Sometimes I have to execute this command twice. (I often adapt the [eltako14bus](https://github.com/grimmpp/eltako14bus) library for communicaiton to the bus.)

## Bugs and Features 
Please open [issues](/issues) if you encounter bugs or if you have ideas for new features. Also quite a lot of devices are not yet supported.

# Contribution and Support to this Project
I'm really happy to provide a more and more growing Home Assistant Eltako Integration and tools like this which extend this automation corner even more. The size of this integration is getting much bigger than the use cases I've realized at home, the variety of supported devices is increasing and the stability of the integraiton is getting to a professional level. On the other side it is getting hard to keep this level of development speed and operational quality. I'm about to build up a professional development and testing environment so that the quality can even improved and futher features can still be delivered in a short time frame. You can support this activity in sending devices and/or money.

In general, you can contribute to this project by:
* Support users in the Home Assistant Community ([Eltako “Baureihe 14 – RS485” (Enocean) Debugging](https://community.home-assistant.io/t/eltako-baureihe-14-rs485-enocean-debugging))
* Reporting [Issues]([/issue](https://github.com/grimmpp/home-assistant-eltako/issues))
* Creating [Pull Requests](https://github.com/grimmpp/home-assistant-eltako/pulls)
* Providing [Documentation](https://github.com/grimmpp/home-assistant-eltako/tree/main/docs)
* Supporting a proper development and test environment by sending devices and/or money. [![Generic badge](https://img.shields.io/badge/SUPPORT_THIS_PROJECT-PayPal.me-27ae60.svg)](https://paypal.me/grimmpp)