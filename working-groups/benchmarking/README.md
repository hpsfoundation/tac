# HPSF Benchmarking Working Group

Benchmarking WG aims to bring together projects and organizations 
to create an automated way to 
continuously test the performance of evolving HPC software stacks, 
ensuring that the components work and perform well.
Functionality testing and performance regression testing are both in scope.
Parts of the software stack we would like to test:
* Compilers
* Runtimes and programming models
* MPI and other communication libraries
* Math libraries
* HPC applications
  

## Leads

* Olga Pearce ([@pearce8](https://github.com/pearce8))


## Meetings

* The working group meets every 2 weeks. [meeting notes](https://docs.google.com/document/d/13edPtYo5hPpbFg7PO71v8RMGJByJRb1fUY1JPuwshkA/edit?usp=sharing)
* [Zoom coordinates](https://zoom-lfx.platform.linuxfoundation.org/meeting/96185757639?password=b7ec8266-4aaf-4f11-bfb0-eae19b8570d9)
* To get involved, join the [Slack channel](https://hpsf.slack.com/archives/C08NKKL97NZ)


## Motivation for launch

* There is not a group that is consolidating and maintaining open source benchmarks
* Each datacenter is for themselves
* Testing/benchmarking of the HPC software stack is intermittent at best
* We want to figure out, as a working group, how we can pull together resources to support and maintain continuous testing,
  with the purpose of testing the performance of the software stack as it evolves (compilers, libraries).


## Initial objectives

* First goal: Run [insert benchmark here] on [insert system here]
* Identify open source benchmarks of general interest
* Work towards running the benchmarks in a sustainable way on a few systems


## Anticipated activities

* Community contributed catalogued library of HPC tests and benchmarks
  * Single component tests
  * Performance benchmarks
  * Proxy applications
  * Large applications
  * Determine a reasonable granularity for code instrumentation/performance measurements (one number is not enough)

* Software stack representation: sharing methodologies, creating best practices
  * Introspection
  * Reproducibility
  * Changing one component version at a time to isolate failures

* Set up continuous testing
  * Leverage HPSF CI WG for CI technology
  * Establish testing on different platforms, at different HPC facilities (e.g., ALCF, OLCF, NERSC), and academic centers (TACC, NCSA)
 
* Work with projects on the TAC to add relevant benchmarks
  * Kokkos, AMReX, WarpX, ...

* Work with members to ask them what they need from a framework
  * NVIDIA, Intel, AMD, HPE, AWS
 
* Use HPSF Con to assess potential scope and showcase progress/results annually


## Customers

The software stack testing will initially be for HPSF projects and participating organizations, 
but could expand after initial launch and willingness of resource providers.
* HPC Vendors 
  * Understand the curated workloads of HPC centers, propose systems
  * Test software stacks
* Procurement teams at HPC Centers 
  * Curate tests and center workload representation
  * Evaluate and monitor system progress
* HPC software stack developers
  * Want to test the software they provide, whether in isolation or with other parts of the software stack
  * E.g., E4S
* Test and Benchmark Developers 
  * People who want to share their tests, reproducers, and benchmarks in a sustainable manner
  * E.g., HPCG
* Researchers and End Users of HPC Tests and Benchmarks
  * Install, run, analyze performance of HPC tests


## Plan

We are collecting project needs as we go along, to inform the plan.
