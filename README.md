Yocto builds
============

To create an image for nonlinear bbb, run this:
```
$ repo init -u git@github.com:nonlinear-labs-dev/bbb-yocto -m yocto/manifests/default.xml
$ repo sync
$ mkdir -p ./build
$ source poky/oe-init-build-env `readlink -f ./build`
$ cp ../yocto/*.conf conf
$ bitbake nonlinear-bbb-image-default
```
