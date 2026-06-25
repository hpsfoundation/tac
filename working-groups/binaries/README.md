### WG Lead(s)

Ryan Krattiger (@kwryankrattiger)

### WG Description

The goal of the Binaries WG is to address challenges in binary portability across the matrix of HPC platforms. The WG will engage projects and HPC providers to develop standards for interoperability and transparency of binary distribution that enhance productivity and scientific advancement.

Some specific areas of interest of this WG include:

- Binary Curation (defining and supporting SDKs)
- ABI compatibility
- Optimizations
- Supply chain integrity (SBOMs/signing/verification/scanning)

### Motivation for launch

Currently there are a number of existing efforts to produce binary caches and build integrated environments for use in HPC.

There are a number of integration efforts under DOE PESO building and advancing SDKs
- Data and Visualization SDK (Berk Geveci at Kitware, Inc.)
- TOOLS SDK (Bill Hoffman at Kitware, Inc.)
- xSDK (Satish Balay, ANL)
- E4S (Sameer Shende, University of Oregon)

There are further efforts in Spack CI to build additional stacks targeting specific domains
- ML (darwin/mac, Linux, CUDA, ROCm)
- HEP (Linux)
- Radiuss

Each of these efforts operate in their own isolated ecosystems. This results in a fair amount of duplicated efforts which would greatly benefit from a neutral body to come together for collaboration.

These projects, and others, are used when creating build caches. Each of these caches have a number of duplicates and low cache hits for HPC sites, especially for large applications like PyTorch, ParaView, Trillinos, etc. 

The Spack project provides binaries through AWS S3
- https://cache.spack.io

The E4S project provides some binaries
- https://oaciss.uoregon.edu/e4s/inventory.html

### Initial activities

* Create baseline environments for bootstrapping binary distributions
  *  Python
  * Compilers and Toolchains (C/C++/Fortran/Rust/etc.)
  * Build tools

### Anticipated activities

* Define binary distributions for HPC
  * Collaboration with Benchmarking WG to determine portable and impactful optimizations
  * Coordinate and expand curation efforts across communities.
  * Develop portable binary distributions
  * Catalog available binary distributions in a common place
* Refine infrastructure usage to better target HPC systems
  * Work with HPC providers to better understand how to create binaries that can run efficiently on their hardware
  * Work with CI WG to refine utilization of HPSF infrastructure 
* Define standards for binary packaging
  * Standardize how to publish binary meta data (ie. SBOMs)
 

### Customers

* HPC Vendors
  * Understand the binary constraints of HPC centers
  * Test binary distributions
* HPC Centers
  * Producing binary distributions that target new systems
* Researchers and End Users of HPC Centers
  * Install and run software directly from curated binary distributions

### Plan

The plan will evolve with respect to the needs of projects and HPC providers as we advance WG goals.
