# fjrodl_pddl_course_jazzy_pixi

## Overview

Work-in-progress.
But it builds.

## Building

### Linux

- install Pixi ([docs](https://pixi.prefix.dev/latest/installation/))
- clone [gavanderhoorn/fjrodl_pddl_course_jazzy_pixi](https://github.com/gavanderhoorn/fjrodl_pddl_course_jazzy_pixi) *somewhere* (on a disk with sufficient free space)
- `cd /path/to/fjrodl_pddl_course_jazzy_pixi`
- `pixi install`
- `pixi run fetch`
- `pixi shell`
- `colcon build`
- `source install/setup.bash`

At this point all packages in the Colcon workspace should be available.

### macOS (Intel)

Only macOS on Intel has been tested.

Make sure to switch to the `osx-64` branch.

Now follow the Linux instructions, but use `pixi run fetch_osx64` instead of the regular `fetch` task.

Note: users on macOS will have to build `popf` and `PlanSys2` from source in the Colcon workspace.
The Pixi configuration should install the necessary (build) dependencies for both.

The `fetch_osx64` task also retrieves the `popf` sources.
`PlanSys2` will have to be `git clone`d manually.
