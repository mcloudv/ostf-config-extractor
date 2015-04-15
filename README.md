# ostf-config-extractor

The tool extracts data from Nailgun and saves it into a config file. That config file can be used as a custom fuel config so that OSTF tests could run without Nailgun.


Usage:
```
export NAILGUN_HOST=...
export NAILGUN_PORT=...
export NAILGUN_TOKEN=...
export CLUSTER_ID=...

ostf-config-extractor --output ostf.conf
```
