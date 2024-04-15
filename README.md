## Prerequisites

* make
* curl
* git 
* [repo tool](https://android.googlesource.com/tools/repo)
* [docker engine](https://docs.docker.com/engine/install/)

## Checking out the project

```sh
repo init -u https://github.com/ku-sldg/attarch-manifest.git
repo sync
```

## Building

See https://github.com/ku-sldg/attarch

## Maintaining
Because the repo tool does not have a way of specifying two remote repositories to initialize from, there is no way to properly extend the seL4 manifest. Instead, it is copied here and editted with our additional remotes. This solution broke once already. Unfortunately, one will be required to manually compare and possibly update the seL4 part of the xml manifest file periodically (ie what is this bizarre build-time error?).
