# HPSF Continuous Integration (CI) Working Group

HPSF aims to bring together multiple efforts to create a CI service for HPC projects,
starting with those in HPSF.

## Efforts we want to bring together

* [Spack](/spack/spack) has a CI service, co-developed by LLNL, Kitware, AWS, and U.
  Oregon,which currently:
  * Runs at [gitlab.spack.io](https://gitlab.spack.io)
  * Uses [Kitware’s CI bridge](https://github.com/spack/spack-infrastructure/pkgs/container/ci-bridge)
    to sync with GitHub
  * Has runners in AWS, U. Oregon, and Google

* U. Oregon runs the [Frank cluster](https://systems.nic.uoregon.edu/internal-wiki/index.php?title=Category:Servers), which:
  * Has many different CPU and GPU resources of interest to HPSF projects
  * Is maintained by UO staff
  * Is hosting CI for Spack and a number of other projects (E4S, Trilinos, others)

* [Hubcast](https://github.com/LLNL/hubcast)
  * A GitHub application that syncs between GitHub and a local GitLab instance
  * Manages support for trusted users/projects and can trigger on-prem GitLab CI
    to run as the user associated with a verified user's email address on GitHub.
  * The CI bridge can likely be rolled into this to make *using* this CI service as easy
    as installing HubCast in GitHub or GitLab and then being granted permission to run
    jobs in our CI service.

* [Jacamar](https://gitlab.com/ecp-ci/jacamar-ci)
  * This allows CI to run at HPC centers *as* the particular user who initiated an action in
    GitLab.
  * Combines with Hubcast to enable running as users associated with external GitHub or GitLab
    users.
  * Is used by many HPC faciltiies to provide secure (trusted) CI for users.

And, later, once we have prototypes:
* HPC facilities (e.g., ALCF, OLCF, NERSC) that want to provide cycles to support the
  HPSF software ecosystem, ensuring that key packages are built and tested at these
  facilities.

## Support / Maintenance

Currently:
* Kitware maintain the Kubernetes and AWS infrastructure that runs Spack's CI system.
* Kitware has also written commands like `spack ci` that enable us to generate build
  pipelines for Spack.
* UO maintains the Frank cluster and the runners on it.
* AWS provides credits and helps with infrastructure questions for Spack's CI cycles.

We want to decide, as a working group, who will run and maintain the HPSF CI service. It
is likely that this will become its own long-term project, so some volunteer effort is
expected, but we also need funding for things like:
  * SREs to maintain the CI service
  * Admins/staff at UO and other sites to maintain cluster and runners
  * HPC facility staff who want to provide runners and cycles to the service
  * Engagements with projects to help them get set up with CI.

We will need to work out how best to support this new scope, whether it falls under
existing projects, etc. Linux Foundation has an internal Release Management team that we
can potentially leverage in the long term, e.g. for project engagements.

## Customers

The CI service will initially be for HPSF projects, but could expand after initial
launch and willingness of resource providers.

We are collecting [project needs](project-needs) as we go along, to inform the plan.

## Plan
1. [ ] Get Spack CI working as a prototype for a couple of projects
2. [ ] Ensure that those projects can only use UO resources via gitlab.spack.io
      (not AWS or Google runners)
3. [ ] Document tagging scheme for node types on gitlab.spack.io so that projects
      can easily set up a new workflow and use GPU resources with a suitable
      `gitlab-ci.yml` file.
4. [ ] Roll CI bridge and other needed functionality in Hubcast
5. [ ] Enable Hubcast to be installed easily and to automatically connect to our CI
      service, so long as permission is granted by HPSF.
6. [ ] Eventually make it easy to log into gitlab.spack.io with:
      - [ ] GitHub credentials
      - [ ] GitLab credentials
7. [ ] Document process for setting up and using HPSF CI, e.g.:
      * Install Hubcast app
      * Register for HPSF CI
      * Add a suitable `gitlab-ci.yml` in your repo
      * Run your first job
8. [ ] Change domain of gitlab.spack.io to ci.hpsf.io (or similar) and launch the
      production service.
9. [ ] Work wtih CASS, PESO, facilities and other DOE efforts to promote this type of
      CI as a best practice for HPC projects
10. [ ] Consider developing some type of certification/metric/badge for HPSF CI so that
      projects can show that they're using it.

## Prototypes and status
So far, two projects have tried running on gitlab.spack.io:

1. Viskores has run on gitlab.spack.io on CPU nodes on the Frank cluster and is working on
   running on GPUs

2. Kokkos is in the process of setting up to run on gitlab.spack.io

3. HPCToolkit is hoping to use this CI as a resource, and has written up
   [some of their needs](project-needs/hpctoolkit.md).

Our plan is to work with these and other projects and show that they can run on GPUs /
CPUs on the machine, and then document the process per the plan above.

We may bring on additional projects as a proof of concept as needed to test
functionality we want to offer.

## Meetings

* The working group meets every **TBD** weeks.
* Zoom coordinates are **TBD**.
* To get involved or to get an invite, **TBD**.
