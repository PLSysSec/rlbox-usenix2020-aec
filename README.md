# RLBox USENIX 2020 Artifact Evaluation
This is the artifact evaluation repo for the paper "Retrofitting Fine Grain Isolation in the Firefox Renderer" submitted to USENIX 2020 in which we introduce the RLBox sandboxing framework.

This repo contains instructions specific for the AEC committee. We provide simple instructions to while the code itself are stored in different repos. Below we give a description for the recommended setup for the AEC.

# Get the source

- Create a new Ubuntu LTS 18.04.4 LTS machine or VM. Install all updates in the OS. Note - Do not use an existing machine; our setup installs packages on the machine and has been well tested on a fresh Ubuntu Install. The VM should have at least 4 CPU cores (mandatory - benchmarks assume this), and 32-GB ram is recommended.
- Get the source available from the [LibrarySandboxing](https://github.com/shravanrn/LibrarySandboxing/) repo using 
```bash
git clone https://github.com/shravanrn/LibrarySandboxing
```
- Follow instructions in the Library Sandboxing repo's README to build the code and run benchmarks.
- If you run into issues here, we are happy to provide a VM with pre-built binaries on request.
