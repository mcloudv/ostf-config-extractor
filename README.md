# ostf-config-extractor

## Description

OSTF Config Extractor is the tool which extracts data from Nailgun and saves it into a config file. That config file can be used as a custom Fuel config so that OSTF tests could be invoked without Nailgun itself.


## Usage:

Extractor requires some credentials (environment variables):

```
export NAILGUN_HOST=<ip_of_nailgun_host>
export NAILGUN_PORT=<port>

export CLUSTER_ID=<cluster_id>

export OS_USERNAME=<username>
export OS_PASSWORD=<password>
export OS_TENANT_NAME=<tenant>
export OS_AUTH_URL=http://<ip_of_nailgun_host>:5000/v2.0

ostf-config-extractor -o ostf.conf
# or ostf-config-extractor --output ostf.conf
```

By default, on MOS cloud there're username=admin, password=admin, tenant=admin,
nailgun_port=8000, cluster_id=1. The parameter OS_AUTH_URL should point to
Nailgun host, as the Extractor works definitely with Nailgun host only.
