apache2-simplyadrian Cookbook
========================
This cookbook sets up apache2 for simplyadrian. A minimal configuration of a vhost file at this point for testing of html display. More will need to be developed to make this a meaningful production cookbook.

Requirements
============

- Apache2 - Official windows cookbook from opscode https://supermarket.chef.io/cookbooks/apache2

Attributes
----------

#### apache2-simplyadrian::vhost
<table>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td><tt>['apache2-simplyadrian']['app_name']</tt></td>
    <td>String</td>
    <td>Provide the name of the app you are loading into Apache2</td>
    <td><tt>helloWorld</tt></td>
  </tr>
</table>

Usage
-----
#### apache2-simplyadrian::vhost

Just include `apache2-simplyadrian::vhost` in your node's `run_list`:

```json
{
  "name":"my_node",
  "run_list": [
    "recipe[apache2-simplyadrian::vhost]"
  ]
}
```

License and Authors
-------------------
Authors: Adrian Herrera
