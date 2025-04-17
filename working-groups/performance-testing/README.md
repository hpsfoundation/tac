# Below are some boring and fun name choices for the WG
# (a) HPSF Benchmarking Working Group
# (b) HPSF Benchmarking and Testing (BT) Working Group
# (c) HPSF Performance Testing (PT) Working Group
# (d) HPSF Performance Testing Infrastructure (PTI) Working Group
# (e) HPSF Performance And Functionality Testing Infrastructure (PAFTI) Working Group
# (f) HPSF Performance and Application Regression Testing Infrastructure (PARTI) Working Group

HPSF aims to bring together projects and organizations to create an automated way to continuously 
test evolving HPC software stacks, ensuring that the components work and perform well.
Functionality testing and performance regression testing are both in scope.
Parts of the software stack we would like to test:
* Compilers
* Runtimes and programming models
* MPI and other communication libraries
* Math libraries
* HPC applications
  

## Leads

* Olga Pearce ([@pearce8](https://github.com/pearce8)])
* ???


## Meetings

* The working group meets every **TBD** weeks.
* Zoom coordinates are **TBD**.
* To get involved or to get an invite, **TBD**.


## Efforts we may be pursuing

* Community contributed catalogued library of HPC tests
  * Single component tests
  * Performance benchmarks
  * Proxy applications
  * Large applications

* Software stack representation
  * Introspection
  * Reproducibility
  * Changing one component version at a time to isolate failures

* Set up continuous testing
  * Leverage HPSF CI WG for CI technology
  * Establish testing on different platforms, at different HPC facilities (e.g., ALCF, OLCF, NERSC)
 
* Work with projects on the TAC to add relevant benchmarks
  * Kokkos, AMReX, WarpX, ...

* Work with members to ask them what they need from a framework
  * NVIDIA, Intel, AMD, HPE, AWS,
 
* Use HPSF Con to assess potential scope 


## Support / Maintenance

Currently:
* Each datacenter is for themselves
* Testing is intermittent at best
* We want to figure out, as a working group, how we can pull together resources to support and maintain continuous testing


## Customers

The software stack testing will initially be for HPSF projects and participating organizations, 
but could expand after initial launch and willingness of resource providers.
* End Users of HPC Tests and Benchmarks
  * Install, run, analyze performance of HPC tests
* Test and Benchmark Developers 
  * People who want to share their tests, reproducers, and benchmarks
* HPC software stack developers
  * Want to test the software they provide, whether in isolation or with other parts of the software stack
* Procurement teams at HPC Centers 
  * Curate tests and center workload representation
  * Evaluate and monitor system progress
* HPC Vendors 
  * Understand the curated workload of HPC centers, propose systems
  * Test software stacks

We are collecting [project needs](project-needs) as we go along, to inform the plan.

## Plan
1. [ ] Gather needs and gage interest
