# consul-envoy

Docker Image for Consul + Envoy

Current Version:

- [Consul](https://www.consul.io/) [v1.6.2](https://hub.docker.com/layers/consul/library/consul/1.6.2/images/sha256-6ba4bfe1449ad8ac5a76cb29b6c3ff54489477a23786afb61ae30fb3b1ac0ae9)
- [Envoy](https://www.envoyproxy.io/) [v1.11.1](https://hub.docker.com/layers/envoyproxy/envoy/v1.11.1/images/sha256-9ef9c4fd6189fdb903929dc5aa0492a51d6783777de65e567382ac7d9a28106b)

## How to Use

```bash
docker run --rm -d --network host --name echo-proxy \
  consul-envoy -sidecar-for echo
```

For more, please check links below:

[Use Envoy with Connect](https://learn.hashicorp.com/consul/developer-mesh/connect-envoy)
