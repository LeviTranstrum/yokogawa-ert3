# TFLite Runtime Wheel for Yokogawa e-RT3 

Building this wheel took most of a day, so I wanted to make it available to others trying to run TFLite on Yokogawa e-RT3.
This was built on RP70 running the `debian_20240209` image provided by Yokogawa.

## Instructions for use
### Download the wheel:

```
curl -OL https://github.com/LeviTranstrum/yokogawa-ert3/raw/master/tflite_runtime-2.6.0-cp39-cp39-linux_armv7l.whl
```

If you get a `curl: (60) SSL certificate problem: certificate is not yet valid` error, you likely don't have the correct date and time set on your e-RT3. To fix this, use `ntpdate`, then retry:

```
sudo apt update
sudo apt install ntpdate
sudo ntpdate pool.ntp.org
curl -OL https://github.com/LeviTranstrum/yokogawa-ert3/raw/master/tflite_runtime-2.6.0-cp39-cp39-linux_armv7l.whl
```

Or, if you're not worried about github.com's SSL certificate, pass the `-k` flag to `curl`:

```
curl -k -OL https://github.com/LeviTranstrum/yokogawa-ert3/raw/master/tflite_runtime-2.6.0-cp39-cp39-linux_armv7l.whl
```

### Install the wheel:

```
pip install tflite_runtime-2.6.0-cp39-cp39-linux_armv7l.whl
```
