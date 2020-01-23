# OPENROAD_USERS_READ_ME_FIRST
OpenROAD users should look at this repository first for instructions on getting started.

New users should start by following the directions in the [OpenROAD-flow](https://github.com/The-OpenROAD-Project/OpenROAD-flow) repo's [flow README](https://github.com/The-OpenROAD-Project/OpenROAD-flow/blob/master/README.md).
The procedures for the download of prebuilt binaries, building all of the code in a container, and building all of the code on bare metal are described there. The application submodules all point to stable and well tested versions of code.
The [OpenROAD-flow](https://github.com/The-OpenROAD-Project/OpenROAD-flow) repo also contains open source sample designs on an open source PDK. Along with these designs are Makefiles to run the designs through OpenROAD.

OpenROAD is comprised of a set of repos, however they are all integrated into the top level application repo named [OpenROAD](https://github.com/The-OpenROAD-Project/OpenROAD) except for Yosys and TritonRoute which will be integrated soon.
All of the repos that the OpenROAD top level applications needs are set up as sub modules. The top level cmake configuration builds all of them. Be sure to clone openroad with the --recursive option to clone all of the submodules in preparation for building.
If you follow this procedure and the rest of the instructions as specified in the [application README](https://github.com/The-OpenROAD-Project/OpenROAD/blob/master/README.md) you will be able to build the application and all of its submodules. Keep in mind that you will need to have the build tools in place that are required for building. There is a [DockerFile](https://github.com/The-OpenROAD-Project/OpenROAD/blob/master/Dockerfile) which can be used to build in a container or as a specification of what is needed to build.

A contribution [guide](https://github.com/The-OpenROAD-Project/OpenROAD/blob/master/doc/OpenRoadArch.md) which explains the philosophy behind the code organization and architecture and also describes the workflow for developers to follow is available. Working with submodules in git is non trivial. If you follow the procedures in the section marked Tool Work Flow, you will have a streamlined way to work efficiently. 

It is also important to pay attention to the (branching methodology)[https://github.com/The-OpenROAD-Project/OpenROAD/blob/master/doc/post_alpha2.1_branch_methodology.md].








