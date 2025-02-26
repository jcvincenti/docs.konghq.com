---
title: Runtime Manager Overview
no_version: true
---

The Runtime Manager is a {{site.konnect_short_name}} SaaS functionality module
that lets you catalogue, connect to, and monitor the status of all runtimes in
one place.

With {{site.konnect_short_name}} acting as the control plane, a runtime
doesn't need a database to store configuration data. Instead, configuration
is stored in-memory on each node, and you can easily update multiple runtimes
from one {{site.konnect_short_name}} account with a few clicks.

The Runtime Manager, and the {{site.konnect_product_name}} SaaS application as
a whole, does not have access or visibility into the data flowing through your
runtimes, and it does not store any data except the state and connection details
for each runtime.

## Hosting Runtimes

Kong does not host runtimes. You must provide your own runtime
instances.

The Runtime Manager aims to simplify this process by providing a
script to provision a {{site.ee_gateway_name}} runtime in a Docker container,
eliminating any confusion about initial configuration or setup.

## Type of Runtimes

### Kong Gateway

A {{site.ee_gateway_name}} runtime acts as a data plane, which is a node
serving traffic for the proxy. Data plane nodes are not directly connected
to a database.

Currently, the only supported runtime type in the
{{site.konnect_product_name}} SaaS application is a [{{site.ee_gateway_name}}](/enterprise/latest/introduction)
data plane running in a Docker container.

**See more**:
* [Set up a {{site.ee_gateway_name}} runtime](/konnect/runtime-manager/kong-gateway-runtime)
* [{{site.ee_gateway_name}} documentation](/enterprise/latest/introduction)
