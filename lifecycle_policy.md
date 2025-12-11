# High Performance Software Foundation Project Lifecycle Policies

## I. Overview

*This governance policy describes how an open source project can formally join the High Performance Software Foundation via the Project Proposal Process. It describes the Stages a project may be admitted under and what the criteria and expectations are for a given stage, as well as the acceptance criteria for a project to move from one stage to another. It also describes the Periodic Review Process (PRP) to reassess project stage assignments.*

Project progression - movement from one stage to another - allows projects to participate at the level that is most appropriate for them given where they are in their lifecycle. Regardless of stage, all High Performance Software Foundation projects benefit from a deepened alignment with existing projects, and access to mentorship, support, and foundation resources.

Capitalized terms not otherwise defined in this Project Lifecycle Policy have the meanings ascribed to them in the Charter of the High Performance Software Foundation.


## II. Project Proposal Process

### Introduction
This governance policy sets forth the proposal process for projects to be accepted into the High Performance Software Foundation. The process is the same for both existing projects which seek to move into the High Performance Software Foundation and new projects to be formed within the High Performance Software Foundation.

### Project Proposal Requirements
Projects must be formally proposed via GitHub. Project proposals submitted to the High Performance Software Foundation should provide the information listed in our
[New Project Proposal Template](https://github.com/hpsfoundation/tac/blob/main/.github/ISSUE_TEMPLATE/new-project-proposal.md) to the best of their ability.

An important requirement from the list is to find two sponsors for your
proposal on the TAC, as the sponsors will be arguing for your acceptance to HPSF. You
should be sure that the sponsors are familiar with your project and your reasons for
wanting to join HPSF.

[Click this link](https://github.com/hpsfoundation/tac/issues/new?template=new-project-proposal.md) to start a new project proposal issue on GitHub.

To see past project proposals, you can look at the closed issues in this repository. See here:

* [Emerging Project Proposals](https://github.com/hpsfoundation/tac/issues?q=is%3Aissue%20state%3Aclosed%20label%3Alevel%3Aemerging)
* [Established Project Proposals](https://github.com/hpsfoundation/tac/issues?q=is%3Aissue%20state%3Aclosed%20label%3Alevel%3Aestablished)
* [Core Project Proposals](https://github.com/hpsfoundation/tac/issues?q=is%3Aissue%20state%3Aclosed%20label%3Alevel%3Acore)

### Project Acceptance Process
Once a project has submitted a proposal as outlined above, the process for accepting them to HPSF is as follows:

1. **Sponsor Review**

   TAC sponsors shall read through the project proposal and ensure that all criteria for the project's requested level are addressed in the proposal.
   If insufficient evidence is presented for any of the criteria, the sponsors should work with the project to bolster the case, or to choose a different, more appropriate initial level.

2. **Sponsor Proposal**

    Once the proposal is in a suitable state, the sponsors shall propose it to the full TAC for onboarding, and the TAC shall decide on a future meeting to hear the presentation.

3. **TAC Preparation**

   TAC voting members shall read the project's proposal and ensure that they are familiar with the state of the project to be onboarded *before* the onboarding presentation.

4. **Presentation** 

   Project members shall present their proposal at the scheduled TAC meeting.
   This should take no more than 30 minutes, to leave time for the TAC to privately discuss after the meeting.
   The presentation should include an introduction to the project and an explanation of alignment with HPSF and key elements of the proposal.
   See links in the prior section to past project proposals for links to past talks.

5. **Private Discussion**

   Once the project members finish their presentation, voting members of the TAC shall convene a private session (e.g., by closing the teleconference to people not on the TAC).
   The project's sponsors shall discuss the project, its presentation, its proposal, and any questions the voting members have as to the evidence for onboarding criteria.

   In the closed session, sponsors are expected to advocate for the project and to clarify any questions the TAC may have.

6. **Voting**

   After the private session, the TAC shall vote asynchronously before the next TAC meeting on the criteria for acceptance of the project.

   The ballot shall include items for each criterion of the proposed stage and for each criterion in all lower stages.
   For each criterion, voting TAC members can choose "Accept", "Against", or "Abstain". There is a [sample ballot here](templates/ballot_template.md) that shows criteria for all levels.

   The ballot shall also include an option to indicate that a project should be accepted provisionally.

   Votes for project acceptance should include options to:
   1. Accept the project at the proposed level;
   2. Accept the project at a lower level than proposed (the poll should list all lower levels as options);
   3. Accept provisionally at the proposed level, pending minor requirements; or
   4. Reject the project.
   
7. **Vote Aggregation Rules**

   For a project to be accepted, the TAC must vote by 2/3 majority to accept all of the criteria for that stage *and* to accept all criteria for lower stages.

   These rules apply for all criteria on the ballot:

   * If the number of votes cast (including explicit "Abstain" votes) is not greater than half of the number of voting TAC members, then the result of the poll is "Against".
   * Otherwise, if the number of "Approve" votes is at least two thirds of the votes cast (not including explicit "Abstain" votes), then the result of the poll is "Approve".
   * Otherwise, the result of the poll is "Against".

   A project is accepted at the *highest* level for which it achieves a 2/3 majority on all criteria. For example, if the project receives:
   * 5 Accept votes and 4 Against votes for all criteria at the "established" level; and
   *  6 accepts and 3 rejections for all criteria at the "emerging" level

   then the project is accepted at the "emerging" level as there was a 2/3 majority for "emerging" but not for "established".

8. **Provisional acceptance**

   If a project is accepted pending minor requirements, it is the sponsors' responsibility to make sure that the project accomplishes the requested changes. This could include (and has included in the past):

   1. Adding a governance document to a repository;
   2. Adopting a Code of Conduct; or
   3. Awaiting approval as a Linux Foundation project.

   Requirements like this should be noted on the project proposal pull request, and an action item for sponsors to follow up should remain on the TAC agenda until the changes are satisfied.

9. **Further Progression** 

   Once accepted, projects can apply for a different stage in HPSF via the Periodic Review Process.

## III. Stages - Definitions & Expectations
Every High Performance Software Foundation project has an associated maturity level.

All projects may attend TAC meetings and contribute work regardless of their stage.

### Emerging Projects

Emerging projects are projects which the TAC believes are, or have the potential to be, important to the ecosystem of Technical Projects or the High Performance Software Foundation ecosystem as a whole. The Emerging stage provides a beneficial, neutral home for these projects. The Emerging stage is intended as a low barrier of entry to the HPSF, which fosters collaborative development and provides a path to deeper alignment with other HPSF projects via the graduation process.

**Possible Characteristics**

* New projects that are designed to extend one or more High Performance Software Foundation projects with functionality or interoperability libraries.
* Independent projects that fit within the Foundation mission and provide potential for a novel approach to existing functional areas or are an attempt to meet an unfulfilled need.
* Projects commissioned or sanctioned by the High Performance Software Foundation.
* Any project that realistically intends to join the Established or later stages in the future and wishes to lay the foundations for that transition.

**Expectations**

End users should evaluate Emerging projects with care, as this stage does not set requirements for community size, governance, or production readiness. Emerging projects will receive minimal support from the Foundation. Projects will participate in the Periodic Review Process; they may also request a status review by submitting a report to the TAC.

**Acceptance Criteria**

To be considered for the Emerging Stage, the project must meet the following requirements:
* Have 2 TAC sponsors to champion the project & provide mentorship as needed
* Align with the mission of the HPSF as laid out above. This will be determined by a majority vote of the TAC
* Submit a proposal for membership and present it at a meeting of the TAC
* Have a code of conduct (part of default governance for LF – there is a template)
* Have a publicly available governance document — even if your governance is somewhat ad hoc, state what it is, including the project's technical leadership and roles
* Upon acceptance, projects must list their status prominently on their website/README


### Established Stage

The Established Stage is for projects that are major components of the High Performance Computing software ecosystem. Established Stage projects will receive mentorship from the TAC and are expected to actively develop their community of contributors, governance, project documentation, and other variables that factor into broad success and adoption.

In order to support their active development, projects in the Established stage have a higher level of access to foundation resources. Projects will participate in the Periodic Review Process.

**Possible characteristics**

* Projects that are looking to create a lifecycle plan (maintainership succession, contributor programs, version planning, etc.).
* Projects which have a substantial user base, but don’t yet have sufficient diversity of their developer community to become a Core project.
* Projects in growing areas of HPC that are working towards becoming Core projects.

**Expectations**

End users can have more confidence in projects in the Established stage, as they have been through an initial round of due diligence and have proven adopters and development processes. Established stage projects are not necessarily expected to have robust succession plans nor broad community backing for long-term sustainability, but are expected to be working towards those criteria of Core projects.

There is no explicit expected timeframe for Established projects to move to Core projects. Established Stage projects are expected to participate actively in TAC proceedings, and as such have a binding vote on TAC matters requiring a formal vote, such as the election of TAC representatives to the governing board.

**Acceptance Criteria**

To be considered for Established Stage, the project must meet the Emerging requirements as well as the following:

* Document that it is being used successfully in production by at least three independent end users which, in the TAC’s judgment, are of adequate quality and scope.
* Demonstrate development processes (e.g., use of pull requests, code review, testing, CI) that lower barriers to contribution and ensure software quality necessary for increased adoption.
* Demonstrate a substantial ongoing flow of commits and merged contributions.
* Since these metrics can vary significantly depending on the type, scope and size of a project, the TAC has final judgment over the level of activity that is adequate to meet these criteria.
* Receive a 2/3 majority vote of the TAC to move to the Established Stage.

### Core Stage

The Core Stage is for projects that are on a sustaining cycle of development, maintenance, and long-term support. Core Stage projects are used commonly in production environments and have large, well-established project communities. Projects in the Core stage have a higher level of access to foundation resources. Projects will participate in the Periodic Review Process.

**Possible characteristics**

* Projects that are essential to the HPC software ecosystem.
* Projects that have publicly documented release cycles and plans for Long Term Support ("LTS").
* Projects that are widely used and receive major contributions from multiple institutions
* Projects that are widely used and developed by a wide array of individual developers

**Expectations**

Like Established projects, Core Stage projects are expected to participate actively in TAC proceedings, and as such have a binding vote on TAC matters requiring a formal vote, such as the election of TAC representatives to the governing board. They receive ongoing financial and marketing support from the Foundation, and are expected to cross promote the foundation along with their activities.

**Acceptance Criteria**

To graduate from Emerging or Established status, or for a new project to join as a Core project, a project must meet the Established stage criteria plus:

* Have a defined governing body of at least 4 or more members (owners and core maintainers), of which no more than 1/2 of whom are affiliated with the same employer. No single institution may control a voting majority of the governing body.
* Have a documented and publicly accessible description of the project's governance, decision-making, and release processes.
* Have a healthy number of committers from at least two organizations. A committer is defined as someone with the commit bit; i.e., someone who can accept contributions to some or all of the project.
* Explicitly defined security reporting and incident mitigation processes, as appropriate to the security risks of the project
* Explicitly defined project governance and committer process.
* Provide evidence of widespread adoption in the HPC ecosystem or in some important component thereof.
* Receive a 2/3 majority vote from the TAC to move to Core stage. Projects can move directly from Emerging to Core, if they can demonstrate sufficient maturity and have met all requirements.


### Emeritus Stage

Emeritus projects are projects which the maintainers feel have reached or are nearing end-of-life. Emeritus projects have contributed to the ecosystem, but are not recommended for modern development except in unusual circumstances, as other options are preferable. The Foundation appreciates the contributions of these projects and their communities, and the role they have played in moving the ecosystem forward.

**Possible characteristics**

* Projects that are "complete" by the maintainers' standards.
* Projects that do not plan to release major versions in the future.
* Projects that have been superseded by other capabilities or incorporated into another project for ongoing support
* Projects that are no longer relevant to the broader software ecosystem

**Expectations**

Projects in this stage are not in active development. Their repositories may have minimal monitoring; in particular, security problems may not be addressed in a timely manner or even at all. Updates, if any, are typically limited to bug fixes. Emeritus projects should clearly state their status and what any user or contributor should expect in terms of response or support. If there is an alternative project the maintainers recommend, it should be listed as well. The foundation will continue to hold the IP and any trademarks and domains, but the project does not draw on foundation resources.

**Acceptance Criteria**

Projects may be granted Emeritus status by a 2/3 vote of the TAC and with approval from project ownership. In cases where there is a lack of project ownership, only a 2/3 vote from the TAC is required. Projects may move to Emeritus status from any prior stage.


## IV. Periodic Review Process

The TAC shall periodically review projects to determine whether they are in the stage that accurately reflects their current status, needs, and goals.

Projects must be reviewed no less frequently than every 24 months. Projects may also request review at any time to present a case to move to a new stage.

Projects that are determined not to meet the acceptance criteria of their current stage will be reassigned to an earlier stage of the project lifecycle. Projects may request additional time (up to 12 months) from the TAC to address the deficiency before a reassignment is made, at the discretion of the TAC.
