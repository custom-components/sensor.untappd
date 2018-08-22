# Untappd
  
[![Version](https://img.shields.io/badge/version-0.0.9-green.svg?style=for-the-badge)](#) [![mantained](https://img.shields.io/maintenance/yes/2018.svg?style=for-the-badge)](#)

[![maintainer](https://img.shields.io/badge/maintainer-Peter%20Skopa%20%40swetoast-blue.svg?style=for-the-badge)](#) [![maintainer](https://img.shields.io/badge/maintainer-Ian%20Richardson%20%40iantrich-blue.svg?style=for-the-badge)](#)


Checks your untappd info and keeps you updated from home-assistant and your wishlist that can be automated to send the list to your phone when your at the bar if you set it up right. Use the [beer card](https://github.com/ciotlosm/custom-lovelace/tree/master/beer-card) to display the wishlist its made by [Ciotlosm](https://github.com/ciotlosm)

  Like this component for home-assistant?


<div style="text-align: center">
  <a href="https://www.paypal.me/swetoast">
    <img src="http://www.libertymachinenews.com/uploads/5/8/4/3/58432585/7594747_orig.png" width="300" />
  </a>
</div>



To get started put `/custom_components/sensor/untappd.py` here:  
`<config directory>/custom_components/sensor/untappd.py`  
  
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
Due to how `custom_componentes` are loaded, it is normal to see a `ModuleNotFoundError` error on first boot after adding this, to resolve it, restart Home-Assistant.
