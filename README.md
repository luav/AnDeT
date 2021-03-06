# AnDeT
AnDeT (Ant Development Tracker) is a collection of server-side application at the Department of Biology of the UNIFR.  
AnDeT is an extension of [FORT (Formicidae Tracker)](https://github.com/formicidae-tracker) of the UNIL.

License: APL v2 for the new components, an original license of the subprojects for their extensions  
Website: https://www3.unifr.ch/bio/en/groups/leboeuf-group/  
Author of the extensions: Artem Lutov &lt;&#108;u&#97;&commat;&#108;ut&#97;n.ch&gt;  
Organizations: [UNIFR](https://www.unifr.ch), [Lutov Analytics](https://lutan.ch/)

> To clone this repository with submodules use:
> ```
> $ git clone --recursive <repo_url>
> ```
> Anyway, all submodules are fetched automatically when installing requirements via the `build` script.

Components:
- `artemis` to detect and track objects;
- `leto` to configure the tracking;
- `hermes` to define the tracking data format;
- `fort-configuration` to deploy the server side, including the network configuration.
<!--
- `olympus` web UI to control climate and preview the live tracking video;
-->

## Requirements
Linux Debian 9+ / Ubuntu 18+.
> All required libraries are installed automatically during the initial build: `./build -i`.

## Build
To build all components for the first time, installing all requirements:
```
$ ./build.sh -i
```

For the subsequent builds of all components:
```
$ ./build.sh
```

Details:
```
$ ./build.sh [-h,--help] | [-i,--init]
  -h,--help  - help, show this usage description
  -i,--init  - initialize the build environment, which should be done only when building the project for the first time

  Examples:
  $ ./build.sh -i
  $ ./build.sh
```
