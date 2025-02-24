---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "hpeuxi_sensor_group_assignment Data Source - hpeuxi"
subcategory: ""
description: |-
  Retrieves a specific sensor group assignment.
---

# hpeuxi_sensor_group_assignment (Data Source)

Retrieves a specific sensor group assignment.

## Example Usage

```terraform
# Retrieve data for a sensor group assignment
data "hpeuxi_sensor_group_assignment" "my_sensor_group_assignment" {
  filter = {
    id = "<my_sensor_group_assignment_id>"
  }
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `filter` (Attributes) The filter used to filter the specific sensor group assignment. (see [below for nested schema](#nestedatt--filter))

### Read-Only

- `group_id` (String) The identifier of the assigned group.
- `id` (String) The identifier of the network group assignment.
- `sensor_id` (String) The identifier of the assigned sensor.

<a id="nestedatt--filter"></a>
### Nested Schema for `filter`

Required:

- `id` (String) The identifier of the sensor group assignment.
