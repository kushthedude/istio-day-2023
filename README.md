# Unraveling Istio: A Tale of Scale, Challenges and Triumphs at DevRev

This repository contains all the Istio manifest examples and demo files used in our talk at IstioDay in Kubecon. The directory structure of the repository is as follows:


```
├── alert_rules
│   └── alert_manager.yaml
├── envoy_filters
│   ├── BUILD.bazel
│   ├── grpc_context_jwt_decode.yaml
│   ├── grpc_transcoder.yaml
│   ├── header_routing.yaml
│   └── wss_close.yaml
├── installation
└── istio_config
    ├── authn.yaml
    ├── graceful_termination.yaml
    └── istiod_metric_opt.yaml
```

## Directory Breakdown

### `alert_rules`
Contains the alert manager rules for monitoring.

- `alert_manager.yaml`: YAML file containing the alert rules for AlertManager.

### `envoy_filters`
Contains various Envoy filter configurations.

- `BUILD.bazel`: Bazel build file for the Envoy filters.
- `grpc_context_jwt_decode.yaml`: YAML file for the gRPC context JWT decode Envoy filter.
- `grpc_transcoder.yaml`: YAML file for the gRPC transcoder Envoy filter.
- `header_routing.yaml`: YAML file for the header routing Envoy filter.
- `wss_close.yaml`: YAML file for the WebSocket close Envoy filter.

### `installation`
Contains the files necessary for Istio installation.

### `istio_config`
Contains various Istio configuration files.

- `authn.yaml`: YAML file for authentication configuration in Istio.
- `graceful_termination.yaml`: YAML file for configuring graceful termination in Istio.
- `istiod_metric_opt.yaml`: YAML file for optimizing Istiod metrics.

## Usage

To use these files, clone this repository to your local machine, navigate to the directory containing the desired files, and apply them to your Istio setup using `kubectl apply -f <filename>`.

## Contributing

We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute.

## License

This project is licensed under the [MIT License](LICENSE.md).
