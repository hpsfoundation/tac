# HPCToolkit CI Summary

To summarize where we (HPCToolkit) stands, we're hoping to use HPSF CI to run CI jobs
that require specialized hardware (AMD GPUs, Intel GPUs, IBM Power, etc.). Today we use
our limited development machines at Rice to run these jobs, we're hoping to improve our
CI speed and stability by transitioning these jobs to an HPSF CI farm. To that end, I
had some initial questions/concerns from last week's update:

## Containers

We use containers for all our CI, Jacamar CI (e.g. for UO Frank) does not enable Podman
support by default and extra per-user setup is needed for rootless Podman (e.g. sub*id
allocations). At least one of the Frank systems with the hardware we are interested in
using does not even have podman installed. Is this support going to be enabled?

## Isolation
Jacamar CI runs jobs using the authentication of the user that initiated the CI
pipeline, AFAICT if the user does not have an account on the backing system the CI job
will fail at start. I don't see a way to detect accounts ahead of time (e.g. to
conditionally run jobs that require extra accounts), and we strongly prefer to keep our
onboarding process as simple as possible when it comes to accounts. Is there a plan that
would avoid us requesting UO accounts for every backing system that may service our
jobs?

## Architectures, tagging
For CI jobs that don't require specialized hardware, we use GitLab-hosted runners (we
get a certain number of compute credits free with our GitLab license). If HPSF CI
provides runners hosted on AWS there will likely be a large overlap. If possible we
would like such runners tagged identically to the GitLab runners so that our jobs can
use either resource as availability allows, this improves the latency and reliability of
our CI pipelines (e.g. if one server is slow or down).

## Contributing cycles from Rice We would like to use our Rice machines in a similar
resource-sharing arrangement during the initial transition (as a fallback as machines
are being configured). We would like to agree on (or be notified of) the tags used for
specialized hardware resources, which we can then use to configure our Rice runners.

## Other needs
HPCToolkit is hosted on https://gitlab.com, in the update you mentioned hosting HPSF CI
in a separate GitLab instance. This has some implications when it comes to CI:

* We would like to smoothly transition between CI resources from multiple sources where
  possible as noted in (3). I don't know of a way to make this happen with a separate
  GitLab instance.

* We want to run CI on specialized hardware for MRs and not just protected branches (it
  helps testing and development). Presumably this would be handled via a bot user or
  status check. Is HPSF going to develop and host the server(s) to manage this CI bridge
  (i.e. Spackbot but more general)?

* This works around the authentication issue in (2), but running CI for MRs means
  arbitrary code may run and there are security risks involved. Will the HPSF CI runners
  have sufficient protections to ensure the backing systems are not unduly harmed by a
  rogue MR?
