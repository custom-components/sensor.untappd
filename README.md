# sensor.untappd

[![GitHub Release][releases-shield]][releases]
[![License][license-shield]](LICENSE.md)

![Project Maintenance][maintenance-shield1]
![Project Maintenance][maintenance-shield2]
[![GitHub Activity][commits-shield]][commits]

[![Discord][discord-shield]][discord]
[![Community Forum][forum-shield]][forum]


Get Untappd last badge, check-in, wishlist and more in Home Assistant. You can also use the [beer card](https://github.com/ciotlosm/custom-lovelace/tree/master/beer-card) by [ciotlosm](https://github.com/ciotlosm) or the [list-card](https://github.com/custom-cards/list-card) by [iantrich](https://github.com/iantrich) to display your wishlist in Lovelace.

## Like this component for home-assistant?

| Donate | Developers |
| --- | --- |
| <a href="https://www.paypal.me/swetoast"><img align="center" src="https://gitlab.com/swe_toast/asustor_firewall/raw/master/images/Untitled.png"></a>   | <a href="https://github.com/swetoast">Toast</a></div> |
| <a href="https://www.buymeacoffee.com/zJtVxUAgH"><img align="center" src="https://www.buymeacoffee.com/assets/img/custom_images/black_img.png"></a> | <a href="https://github.com/iantrich">Ian Richardson</a> |

To get started put `/custom_components/untappd/sensor.py` here:
`<config directory>/custom_components/untappd/sensor.py`

**Example configuration.yaml:**
```yaml
sensor:
  - platform: untappd
    username: average_joe
    id: FSDJLKHDF786287UGHLE
    secret: FJKSDLHKS8337R6948F
```
**Configuration variables:**

key | description
:--- | :---
**platform (Required)** | untappd
**id (Required)** | Your Untappd API id.
**secret (Required)** | Your Untappd API secret.
**username (Required)** | The username of the Untappd user, you want updates for.

You will need to apply for an [API from Untappd](https://untappd.com/api) to use this.

***
Due to how `custom_components` are loaded, it is normal to see a `ModuleNotFoundError` error on first boot after adding this, to resolve it, restart Home-Assistant.

[commits-shield]: https://img.shields.io/github/commit-activity/y/custom-components/sensor.untapped.svg?style=for-the-badge
[commits]: https://github.com/custom-components/sensor.untapped/commits/master
[discord]: https://discord.gg/Qa5fW2R
[discord-shield]: https://img.shields.io/discord/330944238910963714.svg?style=for-the-badge
[forum-shield]: https://img.shields.io/badge/community-forum-brightgreen.svg?style=for-the-badge
[forum]: https://community.home-assistant.io/t/untappd-api/54627
[license-shield]: https://img.shields.io/github/license/custom-components/sensor.untapped.svg?style=for-the-badge
[maintenance-shield1]: https://img.shields.io/badge/maintainer-Peter%20Skopa%20%40swetoast-blue.svg?style=for-the-badge
[maintenance-shield2]: https://img.shields.io/badge/maintainer-Ian%20Richardson%20%40iantrich-blue.svg?style=for-the-badge
[releases-shield]: https://img.shields.io/github/release/custom-components/sensor.untapped.svg?style=for-the-badge
[releases]: https://github.com/custom-components/sensor.untapped/releases
