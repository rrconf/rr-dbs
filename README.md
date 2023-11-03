# dbs

Run debootstrap varint minbase and produce tar-gz image of the resulting tree.

## synopsis

All variables have defaults as indicated below:

```sh
export DBS_BUILD_DIR=$HOME
export DBS_IMAGE=$DBS_BUILD_DIR/$DBS_CODENAME-$DBS_ARCH.tgz

export DBS_INCLUDE=path-to-package-list-file
export DBS_EXCLUDE=path-to-package-list-file

export DBS_ARCH=$(dpkg --print-architecture)
export DBS_CODENAME=bookworm
require dbs
```

Included/excluded packages are in file `pkg.include`/`pkg.exclude` in the module, and certainly contain bare, unusable minimum.
