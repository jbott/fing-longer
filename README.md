# fing-longer

Enabling remote hardware orchestration

## Proselytizing Prose

Deploying hardware for software has been transformed multiple times in the last few years, from on-prem to cloud to
containers. However, the tools for building embedded firmware (or anything interfacing with physical hardware) has not
kept pace.

Of the support that does exist, most of it is based around GPU-type workloads. Docker barely supports passing devices
into containers, resulting in workarounds like [pbelskiy/docker-usb-sync](https://github.com/pbelskiy/docker-usb-sync).
Cloud scheduling tools are laughable at exposing hardware-based resources (see
[nomad](https://github.com/hashicorp/nomad/issues/1081), and
[Kubernetes](https://kubernetes.io/docs/concepts/extend-kubernetes/compute-storage-net/device-plugins/)).

It's kind of unclear what this is yet, but I think there's something to be done with regards to exposing hardware
"as-a-service", in a way that can be consumed both by individual developers ("give me a piece of hardware to test this
code on for the next 6 hours") and by CI ("let me run these 1000 test across the fleet of machines").

## License

This is currently MIT licensed, because right now it's nothing, and I'd rather see this in the world in any form rather
than lock it down behind a restrictive license (either commercial or copyleft).
