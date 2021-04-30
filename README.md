# LuxmedSniper

LUX MED appointments sniper (twilio)
=======================================
Simple tool to notify about available slot in LUX MED medical care service using pushover notifications.

This is a fork of [https://github.com/kubukoz/LuxmedSniper](kubukoz/LuxmedSniper) that comes from
[https://github.com/pawliczka/LuxmedSniper](pawliczka/LuxmedSniper).

How to use LuxmedSniper?
--------------------
First of all create virtualenv and install python requirements from requirements.txt (e.g. by using `pip3 install -r requirements.txt`)

1) For each specialist create configuration file (yaml format) and save it for example as my_favourite_surgeon.yml.

See `luxmedSniper.yaml` for an example with instructions on how to get the specific parameters.

2) Run it
```
python3 luxmedSnip.py -c /path/to/my_favourite_surgeon.yml
```

**Note**: If you're looking for a spot on a fairly available profession,
it's worth running the sniper once with SMS sending disabled so that you don't send a hundred messages at once and use all your Twilio credit.
Just comment the content of `def send_message`.

3) Wait for new SMS with appointment notifications on mobile :)!
