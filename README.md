# Untapped
  
[![Version](https://img.shields.io/badge/version-0.0.1-green.svg?style=for-the-badge)](#) [![mantained](https://img.shields.io/maintenance/yes/2018.svg?style=for-the-badge)](#)   
Checks your untappd info and keeps you updated from home-assistant
  
To get started put `/custom_components/sensor/untapped.py` here:  
`<config directory>/custom_components/sensor/untapped.py`  
  
**Example configuration.yaml:**
```yaml
sensor:
  platform: untapped
  key: FSDJLKHDF786287UGHLE
  secret: FJKSDLHKS8337R6948F
  username: username
```
**Configuration variables:**  
  
key | description  
:--- | :---  
**platform (Required)** | untapped  
**key (Required)** | Your Untapped API key.  
**secret (Required)** | Your Untapped API secret.  
**username (Required)** | The username of the Untaped user, you want updates for.  
  
You will need to apply for an [API from Untapped](https://untappd.com/api) to use this.  
  
***
Due to how `custom_componentes` are loaded, it is normal to see a `ModuleNotFoundError` error on first boot after adding this, to resolve it, restart Home-Assistant.