Home: [ubuntu-setup](README.md)

# Redshift: Installation

To install **redshift** just run following command:
```bash
sudo apt-get install redshift-gtk
```

If ```Unable to start GeoClue client``` error appears on starting, create this config file to set latitude and longitude manually. 

**~/.config/redshift.conf**
```bash
[redshift]
location-provider=manual

[manual]
lat=42.7
lon=23.3
```

__Source:__ https://itsfoss.com/night-shift-flux-ubuntu-linux/

__Source:__ https://github.com/jonls/redshift/issues/158