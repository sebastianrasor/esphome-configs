# Sebastian's ESPHome configs

These are the ESPHome configuration files for all of the smart devices in my
home. I've tried to organize everything to be as easy to copy and utilize in
your own smart home as possible.

## Structure

Every .yaml file in the root directory of this project has substititions to
provide some basic information and then the following packages:
* `base`: This package is meant to hold configurations common to all ESPHome
devices. Currently the only base configuration is
[packages/base.yaml](/packages/base.yaml).
* `device`: This package is meant to expose outputs or internal sensors. These
packages live in [packages/devices/](/packages/devices/).
* `component`: This package is meant to use the outputs or internal sensors
exposed by a `device` package to expose one or more components to Home
Assistant. These packages live in [packages/components/](/packages/components/).
