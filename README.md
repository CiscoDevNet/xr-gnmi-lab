# xr-gnmi-lab

_Understand gNMI and how to build your first gNMI client with Python to interwork with IOS-XR_

<img src="images/use case.png">
 
## Use Case Description

This laboratory comes with two Jupyter notebooks for practising the gNMI functionalities of Cisco IOS XR. A set of Docker containers is used for collecting and monitoring model-driven telemetry data. 

## Installation

### Dependencies

- Python 3
- [Cisco-gnmi-python](https://github.com/cisco-ie/cisco-gnmi-python) library
- Jupyter-notebook
- Docker
- Docker-compose
- IOS XR

### Configure

1. Deploy the stack of containers for monitoring of telemetry data by following these [instructions](monitoring/README.md).

2. Load the _Traffic Monitoring_ dashboard in Chronograf.


## Configuration

The details for the connection and authentication to the IOS XR can be found in each notebook.

This laboratory assumes the following:

- the host of the Jupyter notebook and the docker containers is `198.18.134.50`
- the Jupyter notebook is exposed on port `8080`
- the Chronograf web application is exposed on port `8888`
- the IOS XR is reachable at `198.18.134.72` with username `cisco` and password `cisco`
- the IOS XR has the following gRPC configuration:
  ```
  grpc
   port 57777
  !
  ```

## Usage

Access the notebook at https://198.18.134.50:8080.

Start with the [`cisco-gNMI-main`](./cisco-gNMI-main.ipynb) notebook. To run a section of the laboratory, select the cell and press `Shift+Enter`.


## How to test the software

This laboratory was tested in an environment that had the following software installed:

| Software  | version |
| ------------- | ------------- |
| Python  | `3.6.8`  |
| Cisco-gnmi  | `1.0.4` |
| Jupyter-notebook | `6.0.2` |
| Docker | `19.03.5` |
| Docker-compose | `1.25.1` |
| IOS XR | `7.0.x` |

## Getting help

If you have questions, concerns, bug reports, etc., please create an issue against this repository.

## Getting involved

Feedback, bug fixes and feature enhancements or additions are encouraged. Please see the [CONTRIBUTING](./CONTRIBUTING.md) file for more information.

## Author(s)

This project was written and is maintained by the following individuals:

* cprecup <cprecup@cisco.com>
* nckbgov <nbelchug@cisco.com>
* sbyx <stbarth@cisco.com>
