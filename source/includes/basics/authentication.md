## Authentication

You must pass a token to the metrics endpoint. This token is a credential passed to the app when it is bound to the service. 
Get the access token from the VCAP_SERVICES environment variable.

```shell
"VCAP_SERVICES": {
  "metrics-forwarder": [
   {
    "credentials": {
     "access_key": "[access_token]",
     "hostname": "[endpoint]"
    },
    "label": "metrics-forwarder",
    "name": "[service_instance_name]",
    "plan": "[plan]",
    "provider": null,
    "syslog_drain_url": null,
    "tags": [],
    "volume_mounts": []
   }
  ]
 }
```