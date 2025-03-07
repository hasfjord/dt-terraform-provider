---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "dt_device Data Source - dt"
subcategory: ""
description: |-
  
---

# dt_device (Data Source)



## Example Usage

```terraform
# Copyright (c) HashiCorp, Inc.

data "dt_device" "test_device" {
  provider = disruptive-technologies
  name     = "projects/your-project-id/devices/your-device-id"
}

output "device" {
  value = data.dt_device.test_device
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `name` (String) The resource name of the device. On the form `projects/{project_id}/devices/{device_id}`.

### Read-Only

- `device_id` (String) The resource ID of the device.
- `labels` (Map of String) The labels of the device.
- `project_id` (String) The resource ID of the project.
- `type` (String) The type of the device.
