# tier4_planning_launch

> **Note:** 
> This package is only compatible with the latest Autoware main branch, which uses autoware_universe v0.45.0.
> Compatibility with other versions is not guaranteed.

## Structure

![tier4_planning_launch](./planning_launch.drawio.svg)

## Package Dependencies

Please see `<exec_depend>` in `package.xml`.

## Usage

Note that you should provide parameter paths as `PACKAGE_param_path`. The list of parameter paths you should provide is written at the top of `planning.launch.xml`.

```xml
<include file="$(find-pkg-share tier4_planning_launch)/launch/planning.launch.xml">
  <!-- Parameter files -->
  <arg name="FOO_NODE_param_path" value="..."/>
  <arg name="BAR_NODE_param_path" value="..."/>
  ...
</include>
```
