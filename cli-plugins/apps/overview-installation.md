# Overview

This Tanzu CLI plugin provides the ability to create, view, update, and delete application workloads on any Kubernetes cluster that has the Tanzu Application Platform components installed.

## <a id='About'></a>About Workloads

Tanzu Application Platform enables developers to quickly build and test applications regardless of their familiarity with Kubernetes. Developers can turn source code into a workload running in a container with a URL. 

A Workload enables developers to choose application specifications such as the location of their repository, environment variables, and service claims.

Tanzu Application Platform can support range of possible workloads including, a serverless process that spins up on demand, a constellation of microservices that work together as a logical application, or a small hello-world test app.


## <a id='Installation'></a>Installation

Follow [these instructions](../../install-general.md#cli-and-plugin) to install the Tanzu CLI.

From the `$HOME/tanzu` directory, run:

```
tanzu plugin install --local ./cli apps
```

To verify that the CLI is installed correctly, run:

```
tanzu apps version
```
A version should be displayed in the output.

If the following error is displayed during installation:
```
Error: could not find plugin "apps" in any known repositories

✖  could not find plugin "apps" in any known repositories
```

Verify that there is an `apps` entry in the `cli/manifest.yaml` file. It should look like this:

```
plugins:
...
    - name: apps
      description: Applications on Kubernetes
      versions: []
```
## <a id='command-reference'></a>Command Reference

See [Command Reference](command-reference.md)

## <a id='usage-and-examples'></a>Usage and Examples

See [Usage and examples](usage-and-examples.md)

## <a id='known-issues'></a>Known Issues

See [Known Issues](known-issues.md)

## <a id='feedback'></a>Feedback

For questions or feeadback you can reach us at tanzu-application-platform-beta@vmware.com