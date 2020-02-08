# RLBox USENIX 2020 Artifact Evaluation
This is the artifact evaluation repo for the paper "Retrofitting Fine Grain Isolation in the Firefox Renderer" submitted to USENIX 2020 in which we introduce the RLBox sandboxing framework.

This repo contains all the code and data necessary for building RLBox and reproducing the results presented in our paper.

The code is available in two forms.
- Source - The tar file contains all source code
- VirtualBox disk image

You can use either of these to reproduce results. Detailed instructions for each are provided below.

# Testing

## Get and build the source
If you wish to build the source yourself.
- Create a new Ubuntu LTS 18.04.4 LTS machine or VM. Install all updates in the OS. Note - Do not use an existing machine, our setup installs packages on the machine and has been well tested on a fresh Ubuntu Install. The VM should have at least 4 CPU cores (mandatory - benchmarks assume this), and 32-GB ram is recommended.
- Extract the tar.
- Open the LibrarySandboxing folder and run the command "make". The first stage installs dependencies. After this finishes, the build may instruct you to run "source ~/.profile" and then run "make" again to actually build the source.

Alternately,
- Use the VM image uploaded here. We upload just the VDI file representing the disk. You can create a Virtual box VM with this. The VM should have at least 4 CPU cores (mandatory - benchmarks assume this), and 32-GB ram is recommended.
- The "LibrarySandboxing" folder is located on the desktop. The username and password are both "rlbox".
- The source has already been built.

## Benchmarking

Follow the instructions in LibrarySandboxing/README.md to run the microbenchmarks.
