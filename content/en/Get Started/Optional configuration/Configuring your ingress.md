---
title: Configuring your ingress
weight: 15
description: 'In this section, you will find how to configure your ingress.'
---

---

If you want to use your own ingress instead of the one provided with Charles' installation, follow the next step: 

* On `charlescd/install/helm-chart/values.yaml`, change the **`enabled`** value to **`true`**, like the example below:

```text
ingress:
  enabled: true
  host: charles.info.example
  class: nginx

```
