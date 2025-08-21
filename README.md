# pyMiWiFi

* Remote Management API for Xiaomi Routers

* A fork of the [pyMiWiFi](https://github.com/x2x4com/pyMiWiFi) project.

* Xiaomi terminal devices only support scheduled reboot for the main router, ​​but do not support scheduled reboot for mesh sub-router nodes​​. Therefore, this fork adds a reboot API implementation. By combining this with a scheduled task service, you can achieve scheduled reboots for sub-routers.

# Sub-Router Reboot Usage

```
from MiWiFi import MiWiFiClient

client = MiWiFiClient('miwifi_password', "sub_router_ip")

client.reboot()
```
