# LuxmedSniper
LUX MED appointments sniper
=======================================
Simple tool to notify about available slot in LUX MED medical care service using pushover notifications.

How to use LuxmedSniper?
--------------------
First of all create virtualenv and install python requirements from requirements.txt (e.g. by using `pip3 install -r requirements.txt`)

1) For each specialist create configuration file (yaml format) and save it for example as my_favourite_surgeon.yml.

See `luxmedSniper.yaml` for an example with instructions on how to get the specific parameters.

2) Run it
```
python3 luxmedSnip.py -c /path/to/my_favourite_surgeon.yml
```
3) Wait for new appointment notifications in your pushover app on mobile :)!
