# Untapped
  
[![Version](https://img.shields.io/badge/version-0.0.4-green.svg?style=for-the-badge)](#) [![mantained](https://img.shields.io/maintenance/yes/2018.svg?style=for-the-badge)](#) [![maintainer](https://img.shields.io/badge/maintainer-Peter%20Skopa%20%40swetoast-blue.svg?style=for-the-badge)](#)   
Checks your untappd info and keeps you updated from home-assistant and your wishlist that can be automated to send the list to your phone when your at the bar if you set it up right.

Like this component for home-assistant?

<a href="https://www.paypal.me/swetoast">![Buy me a beer](https://img.shields.io/badge/Buy%20me%20a%20beer-red.svg?longCache=true&style=for-the-badge)</a>

To get started put `/custom_components/sensor/untappd.py` here:  
`<config directory>/custom_components/sensor/untappd.py`  
  
**Example configuration.yaml:**
```yaml
sensor:
  platform: untappd
  key: FSDJLKHDF786287UGHLE
  secret: FJKSDLHKS8337R6948F
  username: username
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
Due to how `custom_componentes` are loaded, it is normal to see a `ModuleNotFoundError` error on first boot after adding this, to resolve it, restart Home-Assistant.
