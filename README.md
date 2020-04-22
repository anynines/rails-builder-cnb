# Rails Cloud Native Buildpacks builder

The Rails Cloud Native Buildpacks builder is optimized for Ruby On Rails applications. It is meant to be used in conjunction [Cloud Native Buildpacks](https://buildpacks.io).

## Create the rails builder image

Currently, the builder relies on CNBs being stored in the parent directory of this repository (e.g. `../procfile-cnb`). See `builder.toml` to learn which CNBs are currently used.

Execute:

    pack create-builder anyninesgmbh/rails-builder:latest --builder-config ./builder.toml
