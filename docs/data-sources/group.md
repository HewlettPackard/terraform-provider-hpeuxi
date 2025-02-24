---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "hpeuxi_group Data Source - hpeuxi"
subcategory: ""
description: |-
  Retrieves a specific group.
---

# hpeuxi_group (Data Source)

Retrieves a specific group.

## Example Usage

```terraform
# Retrieve data for level 1 group
data "hpeuxi_group" "level_1" {
  filter = {
    id = "<level_1_group_id>"
  }
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `filter` (Attributes) The filter used to filter the specific group. (see [below for nested schema](#nestedatt--filter))

### Read-Only

- `id` (String) The identifier of the group.
- `name` (String) The name of the group.
- `parent_group_id` (String) The identifier of the parent of the group.
- `path` (String) The path of the group.

<a id="nestedatt--filter"></a>
### Nested Schema for `filter`

Required:

- `id` (String) The identifier of the group.
