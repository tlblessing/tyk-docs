---
date: 2020-06-24T12:59:42Z
title: Custom Plugins
menu: "main"
weight: 80
url: "/plugins"
---

Tyk supports the use of the following plugins to extend Tyk functionality:

*   [Python, Lua, gRPC (Rich Plugins)](/docs/plugins/rich-plugins/)
*   [JavaScript Plugins](/docs/plugins/javascript-middleware/) (JSVM Middleware)
*   [Golang native plugins](/docs/plugins/golang-plugins/golang-plugins/)

inside the following areas of the API Request Lifecycle

*   [Authentication Plugins](/docs/plugins/auth-plugins/)
*   [Request Plugins](/docs/plugins/request-plugins/)
*   [Response Plugins](/docs/plugins/response-plugins/)

> **Note**: Plugins are only available for Multi-Cloud and On-Premises installations.

### Plugin Caveats

*   They must run as a single process.
*   The plugins used *must* be specified in an API definition and are not global across APIs.
*   They must manage API-specific cases in the same process, only one CoProcess will be managed by a Tyk Instance.
