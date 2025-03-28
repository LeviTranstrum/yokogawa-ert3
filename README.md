# Yokogawa e-RT3 TFLite Runtime Wheel

Building this wheel took most of the day, so I wanted to make it available to others trying to run TFLite on Yokogawa e-RT3.
This was built on RP70 running the `debian_20240209` image provided by Yokogawa.

## Instructions for use
Download the wheel:

`curl -OL https://github.com/LeviTranstrum/yokogawa-ert3/blob/master/tflite_runtime-2.6.0-cp39-cp39-linux_armv7l.whl`

Install the wheel:

`pip install tflite_runtime-2.6.0-cp39-cp39-linux_armv7l.whl`