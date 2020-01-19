![Consul Envoy Icon](https://github.com/VitoVan/consul-envoy/raw/master/iconfile.png)

# consul-envoy

[![Docker Image for Consul Envoy](https://img.shields.io/docker/cloud/build/vitovan/consul-envoy)](https://hub.docker.com/r/vitovan/consul-envoy)

Docker Image for Consul + Envoy

Current Version:

- [Consul](https://www.consul.io/) [v1.6.2](https://hub.docker.com/layers/consul/library/consul/1.6.2/images/sha256-6ba4bfe1449ad8ac5a76cb29b6c3ff54489477a23786afb61ae30fb3b1ac0ae9)
- [Envoy](https://www.envoyproxy.io/) [v1.12.2](https://hub.docker.com/layers/envoyproxy/envoy/v1.12.2/images/sha256-b36ee021fc4d285de7861dbaee01e7437ce1d63814ead6ae3e4dfcad4a951b2e)

## How to Use

```bash
docker run --rm -d --network host --name echo-proxy \
  consul-envoy -sidecar-for echo
```

For more, please check links below:

[Use Envoy with Connect](https://learn.hashicorp.com/consul/developer-mesh/connect-envoy)
