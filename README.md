# consul-envoy

Docker Image for Consul + Envoy

Current Version:

- Consul v1.6.2
- Envoy v1.11.1

## How to Use

```bash
docker run --rm -d --network host --name echo-proxy \
  consul-envoy -sidecar-for echo
```

For more, please check links below:

[Use Envoy with Connect](https://learn.hashicorp.com/consul/developer-mesh/connect-envoy)
