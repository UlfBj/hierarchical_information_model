---
title: "Read-only node"
weight: 30
---

This node type shall be used for data that can only be read and not written to. The HIM node type name is `ro`.

Nodes of the type `ro` must have the following mandatory metadata:
- Name
- Type
- Datatype
- Description

For more information, see the [Common Rule Set: Mandatory Metadata](/hierarchical_information_model/common_rule_set/basics#mandatory-metadata).

Besides the mandatory metadata mentioned above, the following optional metadata may be used
- Unit
- Min
- Max
- Allowed
- Comment

For more information, please see the [Common Rule Set: Optional Metadata](/hierarchical_information_model/common_rule_set/basics#optional-metadata).

This node type must have a node of type `branch` as parent, and must not have any children.

An example of the specification of a `ro` node is given below.

```YAML
Name:
  type: ro
  datatype: string
  description: The name of a vehicle occupant.
```
