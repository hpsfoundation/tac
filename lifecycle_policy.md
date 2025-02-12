# High Performance Software Foundation Project Lifecycle Policies

## I. Overview

*This governance policy describes how an open source project can formally join the High Performance Software Foundation via the Project Proposal Process. It describes the Stages a project may be admitted under and what the criteria and expectations are for a given stage, as well as the acceptance criteria for a project to move from one stage to another. It also describes the Periodic Review Process (PRP) to reassess project stage assignments.*

Project progression - movement from one stage to another - allows projects to participate at the level that is most appropriate for them given where they are in their lifecycle. Regardless of stage, all High Performance Software Foundation projects benefit from a deepened alignment with existing projects, and access to mentorship, support, and foundation resources.

Capitalized terms not otherwise defined in this Project Lifecycle Policy have the meanings ascribed to them in the Charter of the High Performance Software Foundation.


## II. Project Proposal Process

### Introduction
This governance policy sets forth the proposal process for projects to be accepted into the High Performance Software Foundation. The process is the same for both existing projects which seek to move into the High Performance Software Foundation and new projects to be formed within the High Performance Software Foundation.

### Project Proposal Requirements
Projects must be formally proposed via GitHub. Project proposals submitted to the High Performance Software Foundation should provide the following information to the best of their ability:

* name of project
* project description (what it does, why it is valuable, origin and history)
* statement on alignment with the High Performance Software Foundation mission as expressed in the [HPSF Roles and Values](https://hpsf.io/#goals)
* link to *current* Code of Conduct (if one is adopted already)
* project license
* source control (e.g., GitHub, Gitlab)
* issue tracker (e.g., GitHub, Gitlab)
* external dependencies (including licenses)
* release methodology and mechanics
* brief description of current leadership team and decision-making process
* list of the project members with access to commit to the mainline of the project
* link to a documented governance practice
* list of project's official communication channels (E.g., slack, irc, mailing lists)
* link to project's website
* links to social media accounts
* brief description of current user community
* brief description of current contributor community
* existing financial sponsorship and funding institutions
* existing legal entity, if any
* sponsor from the TAC, if identified (a sponsor helps mentor projects)
* preferred project lifecycle stage to enter HPSF (see stages below)
* infrastructure needs or requests (there will be opportunities to change this after joining HPSF)

### Project Acceptance Process
* Projects are required to present their proposal at a TAC meeting
* The TAC may ask for changes to bring the project into better alignment with the High Performance Software Foundation (adding a governance document to a repository or adopting a Code of Conduct, for example).
* The project will need to make these changes in order to progress further.
* Projects are accepted by a 2/3 majority of the TAC.
* Vote majorities will be calculated as a percentage of the votes received
* The TAC will determine the appropriate initial stage for the project. The project can apply for a different stage via the Periodic Review Process.

#### Poll TAC Voting Members
The Linux Foundation conducts a poll of all TAC voting members.
The Linux Foundation creates the poll by filling in the "PROJECT NAME" field in the following poll template.

* Question 1: That PROJECT NAME meets all requirements to be a Linux Foundation project.
* Question 2: That PROJECT NAME has 2 TAC sponsors to champion the project and provide mentorship as needed.
* Question 3: That PROJECT NAME has a charter document with an intellectual property policy that leverages open licenses, including, in the case of contributions of code, the use of one or more licenses approved as "open" by the Open Source Initiative.
* Question 4: That PROJECT NAME has a code of conduct.
* Question 5: The PROJECT NAME has a publicly available governance document.
* Question 6: That PROJECT NAME has documented that the project is being used successfully in production by at least three independent end users which, in the TAC's judgment, are of adequate quality and scope.
* Question 7: That PROJECT NAME has demonstrated development processes (e.g., use of pull requests, code review, testing, CI) that lower barriers to contribution and ensure software quality necessary for increased adoption.
* Question 8: That PROJECT NAME has demonstrated a substantial ongoing flow of commits and merged contributions.

#### Vote
TAC voting members may respond to each poll question with one of three options: Approve, Against, or Abstain.
The poll ends when all TAC voting members respond to the poll, or the poll expires.

#### Aggregate Poll Results
After the poll ends, The Linux Foundation applies the following rules to determine the result of each poll question.

If the total votes received is not greater than zero, then the result of all questions is Against.
Otherwise, if the total Approve responses for a question is at least two thirds of the votes received, then the result of that question is Approve.
Otherwise, the result of a question is Against.

#### Determine Project Stage
If the poll yields an Approve result for poll questions 1 through 8, then the Project is conditionally approved for HPSF membership at the Established Stage.
Otherwise, if the poll yields an Approve result for poll questions 1 through 5, then the Project is conditionally approved for HPSF membership at the Sandbox Stage.
Otherwise, the Project is not approved for HPSF membership, and the acceptance process does not proceed to the next step.

#### Join The Linux Foundation
If the Project is a Linux Foundation project, then The Linux Foundation notifies the TAC that the Project is a Linux Foundation project.

If the Project is not a Linux Foundation project, then the Project seeks to become a Linux Foundation project.
After the Project becomes a Linux Foundation project, The Linux Foundation notifies the TAC that the project is a Linux Foundation project.

#### Formally Accept the Project
After The Linux Foundation notifies the TAC that the Project is a Linux Foundation project, the TAC formally accepts the Project as an HPSF project at the stage that it was conditionally approved for.

## III. Stages - Definitions & Expectations
Every High Performance Software Foundation project has an associated maturity level.

All projects may attend TAC meetings and contribute work regardless of their stage.

### Sandbox Projects
**Definition**

Sandbox projects are projects which the TAC believes are, or have the potential to be, important to the ecosystem of Technical Projects or the High Performance Software Foundation ecosystem as a whole. The Sandbox stage provides a beneficial, neutral home for these projects. The Sandbox stage is intended as a low barrier of entry to the HPSF, which fosters collaborative development and provides a path to deeper alignment with other HPSF projects via the graduation process.

**Possible Characteristics**

* New projects that are designed to extend one or more High Performance Software Foundation projects with functionality or interoperability libraries.
* Independent projects that fit within the Foundation mission and provide potential for a novel approach to existing functional areas or are an attempt to meet an unfulfilled need.
* Projects commissioned or sanctioned by the High Performance Software Foundation.
* Any project that realistically intends to join the Established or later stages in the future and wishes to lay the foundations for that transition.

**Expectations**

End users should evaluate Sandbox projects with care, as this stage does not set requirements for community size, governance, or production readiness. Sandbox projects will receive minimal support from the Foundation. Projects will participate in the Periodic Review Process; they may also request a status review by submitting a report to the TAC.

**Acceptance Criteria**

To be considered for the Sandbox Stage, the project must meet the following requirements:
* Meet all requirements to be a [Linux Foundation project](https://www.linuxfoundation.org/projects/hosting)
* Have 2 TAC sponsors to champion the project & provide mentorship as needed
* Submit a proposal for membership and present it at a meeting of the TAC
* Have a charter document with an intellectual property policy that leverages open licenses, including, in the case of contributions of code, the use of one or more licenses approved as “open” by the Open Source Initiative.  The staff of the High Performance Software Foundation can assist projects in preparing a technical charter following the High Performance Software Foundation’s standard template.
* Have a code of conduct (part of default governance for LF – there is a template)
* Have a publicly available governance document — even if your governance is somewhat ad hoc, state what it is, including the project's technical leadership and roles
* Upon acceptance, projects must list their status prominently on their website/README


### Established Stage
**Definition**

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

To be considered for Established Stage, the project must meet the Sandbox requirements as well as the following:

* Document that it is being used successfully in production by at least three independent end users which, in the TAC’s judgment, are of adequate quality and scope.
* Demonstrate development processes (e.g., use of pull requests, code review, testing, CI) that lower barriers to contribution and ensure software quality necessary for increased adoption.
* Demonstrate a substantial ongoing flow of commits and merged contributions.
* Since these metrics can vary significantly depending on the type, scope and size of a project, the TAC has final judgment over the level of activity that is adequate to meet these criteria.
* Receive a 2/3 majority vote of the TAC to move to the Established Stage.

### Core Stage
**Definition**

The Core Stage is for projects that are on a sustaining cycle of development, maintenance, and long-term support. Core Stage projects are used commonly in production environments and have large, well-established project communities. Projects in the Core stage have a higher level of access to foundation resources. Projects will participate in the Periodic Review Process.

**Possible characteristics**

* Projects that are essential to the HPC software ecosystem.
* Projects that have publicly documented release cycles and plans for Long Term Support ("LTS").
* Projects that are widely used and receive major contributions from multiple institutions
* Projects that are widely used and developed by a wide array of individual developers

**Expectations**

Like Established projects, Core Stage projects are expected to participate actively in TAC proceedings, and as such have a binding vote on TAC matters requiring a formal vote, such as the election of TAC representatives to the governing board. They receive ongoing financial and marketing support from the Foundation, and are expected to cross promote the foundation along with their activities.

**Acceptance Criteria**

To graduate from Sandbox or Established status, or for a new project to join as a Core project, a project must meet the Established stage criteria plus:

* Have a defined governing body of at least 4 or more members (owners and core maintainers), of which no more than 1/2 of whom are affiliated with the same employer. No single institution may control a voting majority of the governing body.
* Have a documented and publicly accessible description of the project's governance, decision-making, and release processes.
* Have a healthy number of committers from at least two organizations. A committer is defined as someone with the commit bit; i.e., someone who can accept contributions to some or all of the project.
* Explicitly defined security reporting and incident mitigation processes, as appropriate to the security risks of the project
* Explicitly defined project governance and committer process.
* Provide evidence of widespread adoption in the HPC ecosystem or in some important component thereof.
* Receive a 2/3 majority vote from the TAC to move to Core stage. Projects can move directly from Sandbox to Core, if they can demonstrate sufficient maturity and have met all requirements.


### Emeritus Stage
**Definition**

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
