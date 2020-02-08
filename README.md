# RLBox USENIX 2020 Artifact Evaluation
This is the artifact evaluation repo for the paper "Retrofitting Fine Grain Isolation in the Firefox Renderer" submitted to USENIX 2020 in which we introduce the RLBox sandboxing framework.

This repo contains all the code and data necessary for building RLBox and reproducing the results presented in our paper.

# Build the source

- Create a new Ubuntu LTS 18.04.4 LTS machine or VM. Install all updates in the OS. Note - Do not use an existing machine; our setup installs packages on the machine and has been well tested on a fresh Ubuntu Install. The VM should have at least 4 CPU cores (mandatory - benchmarks assume this), and 32-GB ram is recommended.
- Download the source code which is available in a tar file in the [releases](https://github.com/PLSysSec/rlbox-usenix2020-aec/releases) section in the repo. Due to the size of the file, has been split into 2 pieces. Download both files and recombine this with the following command.
```bash
cat LibrarySandboxing.tar.xz.part.* > LibrarySandboxing.tar.xz
```
- Extract the tar.
- Open the LibrarySandboxing folder and run the command "make". The first stage installs dependencies. After this finishes, the build may instruct you to run "source ~/.profile" and then run "make" again to actually build the source.

## Benchmarking

Follow the instructions in LibrarySandboxing/README.md to run the microbenchmarks.
