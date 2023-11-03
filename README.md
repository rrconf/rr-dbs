# dbs

Run debootstrap and produce tar-gz image of the resulting tree.

## synopsis

All variables have defaults as indicated below:

```sh
export DBS_BUILD_DIR=$HOME
export DBS_ARCH=$(dpkg --print-architecture)
export DBS_CODENAME=bookworm
export DBS_IMAGE=$DBS_BUILD_DIR/$DBS_CODENAME-$DBS_ARCH.tgz
require dbs
```

Included/excluded packages are in file `pkg.include`/`pkg.exclude`.
