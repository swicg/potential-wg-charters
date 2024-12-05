# CG/WG Proposal Stages

Author: @bumblefudge, @samuelgoto
Created: 09/26/2024
Last update: 09/26/2024
Status: proposed CG charter amendment

This is a proposal to break proposals into 5 stages of maturity, with clear guidelines and requirements to advance them:

* [Stage 0](#stage-0-exploration): **Exploration** of a Problem Space and/or
  user stories
* [Stage 1](#stage-1-incubation-community-andor-community-group): **Incubation**
  of targeted candidate solutions
* [Stage 2](#stage-2-formalization-community-group): **Formalization** a
  preferred Proposal
* [Stage 3](#stage-3-implementation-and-normative-draft-working-group):
  **Implementation** of the preferred Proposal
* [Stage 4](#stage-4-publication-or-re-publication-working-group):
  **Publication** of a Proposed Recommendation

These stages support the W3C process. If there is ever any question between W3C
process requirements and how the groups will progress their work, the W3C
process has precedent.

It is recommended that work undertaken intending to be adopted 
by this staging process consider beginning its unofficial work already
under the [W3C Software and Document License](https://www.w3.org/copyright/software-license-2023/),
or similar license from the W3C.

Note: As this process focuses on documents and deliverables, it is
"individualistic" and refers to champions (usually one of the editors and/or
primary authors of deliverable) as its primary control structure. In practice,
the community group has a marked preference for collaborative work, and the
formation of a "task force" to collect contributions is the default working
mode. There is no requirement that a task force be lead by a work item's
champion, and in many cases a task force is best convened by a "problem expert"
or, e.g., a usability researcher rather than an implementer of a given solution,
particularly if multiple solutions are being debated and compared by the group.
Task Forces are not required but recommended, and can be formed at any stage,
although typically community group conversation about forming one coincides with
the adoption of a Stage 1 work item.

## Stage 0: Exploration

The purpose of Stage 0 proposals is to allow anyone to raise and explore the
Problem Space without asking for permission.

* What's needed from individuals?
  * [ ] Typically, a detailed (but IP-safe, high-level) issue describing a user
    story or problem
    * Minimally, a personal repo, a blog post with examples, a mock-up, etc.
    * Maximally, an end-to-end prototype worked on in community venues
* Who is involved?
  * CG meeting time should be minimally requested except in the form of
    "announcements" about progress at this stage
  * CG Mailing List is an appropriate place for high-level or user-story
    discussion.
  * It is also recommended that community venues like
    [SocialHub](https://socialhub.activitypub.rocks/), [Indieweb.org
    Brainstorming](https://indieweb.org/wiki#Brainstorming), [Fediverse
    Ideas](https://codeberg.org/fediverse/fediverse-ideas/), or the social web
    itself be used to gather more input and to poll interest.
  * Descriptive specifications of a prototype (whether as a drafting exercise or
    as an invitation to prototype interoperability) can be hosted on git forges,
    including community venues like [the Fediverse Enhancement
    Proposals](https://codeberg.org/fediverse/fep/).
    * The CG may request this kind of preliminary community and implementer
      feedback according to the pre-existing [3-stage Standardization Process
      Proposal], particularly for extensions to the protocol's required
      Vocabularies (see the [ActivityPub/ActivityStreams-specific Vocabulary
      Extension Policy])
    * Other [Social Web Protocols] may also ask for implementer feedback at this
      stage
* What's the optimal outcome?
  * Objective, open description of a problem or user story [set] that is within
    scope of the CG
  * IP Safety of work done outside the CG (best insured by keeping discussions
    and prototyping high-level and application-specific, and postponing
    considerations of protocol engineering and efficiency)
  * A champion to gather and synthesis feedback, from outside the CG and to
    coordinate with the CG for review and future stages of work

## Stage 1: Incubation (Community and/or Community Group)

The purpose of Stage 1 proposals is to explore the Solution Space and evaluate
multiple candidate solutions fairly. This is where most of the work gets done
because it involves exploring alternatives, understanding tradeoffs, gathering
implementation experience, incubating alternatives, gathering evidence of demand
and fitness for purpose, and finally, identifying the best out of the many
alternatives.

**Great care** should be taken to avoid substantial technical/design discussions
happening outside the "IPR" (intellectual property rights) boundary of the
Community Group members if normative status beyond stage 1 is desired; further
standardization MUST be rejected if "clean IPR" cannot be achieved (e.g. by
post-facto IP grants from all substantial contributors).

* What's needed from champions?
  * [ ] Public identification of one or more
    [champions](https://github.com/tc39/how-we-work/blob/main/champion.md)
  * [ ] An understanding of the problem space (need not be *deeply* technical)
  * [ ] Familiarity with prior art and related parallel work
* What's asked of the **Community Group**?
  * [ ] The Community Group consensus that the problem is worth spending the
    Community Group’s time working on
  * [ ] A home for incubating the proposal. Small features will incubate in
    issues. If and when the champions are ready to more thoroughly document
    their proposal, the WG chairs will create a repo for the champions to
    develop the feature or proposal (e.g.,
    [example](https://github.com/swicg/activitypub-http-signature)).
  * [ ] If there is enough interest and diversity of contributors, a CG Task
    Force can often be helpfully proposed at this point to house and track
    discussions, but is not a requirement. Particularly for features with IPR
    consequences, task forces can be helpful for pushing sensitive discussions
    inside the IPR boundaries of the community group.

## Stage 2: Formalization (Community Group)

The purpose of Stage 2 Proposals is to formally specify one or more (workable)
candidate solutions identified in the prior step: handle corner cases, integrate
with other parts, reconcile with other proposals, and resolve the concerns
identified at the entrance. The Proposal enters Stage 2 with a list of blocking
issues to advance to the next stage and exits with all of the issues resolved
and CG consensus on a CG Report.

* What's needed from champions?
  * [ ] An [explainer](https://tag.w3.org/explainers/)
  * [ ] Alternatives and trade-offs considered (an overview of useful
    discussions on and off CG venues appreciated)
  * [ ] A specific preferred proposal, e.g., a Report draft, which can include
    code samples, examples, etc.
  * [ ] Developer implementation experience (e.g., a prototype, interop
    experiments, etc)
  * [ ] Confidence of developer demand and fitness for purpose (e.g. a developer
    or forker of a complete implementation that needs this proposal)
* What's asked of the **Working Group**?
  * [ ] Working Group consensus to adopt the proposal as the basis for their
    work as a [Working Draft](https://www.w3.org/policies/process/#RecsWD).
  * [ ] Working Group identification of the list of (seemingly resolvable)
    issues that have to be addressed before [Stage
    3](#stage-3-implementation-and-normative-draft-working-group).
  * [ ] An [Editor's Draft](https://www.w3.org/policies/process/#editors-draft)
    can be used to get PRs merged between [Working
    Draft](https://www.w3.org/policies/process/#RecsWD) revisions.

## Stage 3: Implementation and Normative Draft (Working Group)

The purpose of Stage 3 Proposals is to increase implementation and deployment
confidence in order to move from CG report to a complete draft of a [Candidate
Recommendation](https://www.w3.org/policies/process/#RecsCR).

* What's needed from champions?
  * [ ] Expanded Report (i.e. first draft of a Recommendation) and/or PR to
    extend or update Social Web normative specs
    * [ ] Conformance sections and initial Privacy and Security Considerations
  * [ ] Runnable Tests and test case documentation (ideally more formal than
    pseudocode)
  * [ ] Further implementation experience, ideally diverse and external
* What's asked of the **Working Group**?
  * [ ] Working Group consensus that the [Working
    Draft](https://www.w3.org/policies/process/#RecsWD) sufficiently resolves
    all of the issues raised at [Stage
    2](#stage-2-formalization-community-group)
  * [ ] Working Group consensus to publish the [Working
    Draft](https://www.w3.org/policies/process/#RecsWD) as the Working Group's
    [Candidate Recommendation](https://www.w3.org/policies/process/#RecsCR)
  
## Stage 4: Publication or Re-publication (Working Group)

 The purpose of Stage 4 Proposals is to produce a new [W3C
 Recommendation](https://www.w3.org/policies/process/#RecsW3C) or a new minor or
 major version of a prior one.

* What's needed from champions?
  * [ ] Sufficient [implementation
    experience](https://www.w3.org/policies/process/#implementation-experience)
  * [ ] Two or more independent and complete implementations
    * [ ] Implementation reports and corresponding conformance reports for each
* What's asked of the **Working Group**?
  * [ ] Working Group consensus that the [Candidate
    Recommendation](https://www.w3.org/policies/process/#RecsCR)'s
    implementation experience is complete and
  * [ ] Working Group consensus to publish it as a [Proposed
    Recommendation](https://www.w3.org/policies/process/#RecsPR)

## Prior Art

* Social CG precedents:
  * Evan Promodorou's [ActivityPub/ActivityStreams-specific Vocabulary Extension
    Policy]
  * A. Schrijver [3-stage Standardization Process Proposal]
  * Indieweb [Living Standard Process] (see [github discussion
    here](https://github.com/w3c/strategy/issues/435#issuecomment-1751403081))
* TC39  
  * [TC39 Proposals]
  * [TC39 Process Document]
  * Examples  
    * [TC39 Decorators Proposal]
    * [TC39 Temporal Proposal]
* Immersive Web CG/WG
  * [IW Proposals]
  * [IW Stage 0 Proposals]
  * Examples  
    * [IW Model Element Proposal]
    * [IW Depth Sensing Proposal]
* WebAssembly  
  * [WA Proposals]
  * Examples:  
    * [WA Tail Call Proposal]
    * [WA GC Proposal]

[ActivityPub/ActivityStreams-specific Vocabulary Extension Policy]:
    https://swicg.github.io/extensions-policy/
[3-stage Standardization Process Proposal]:
    https://socialhub.activitypub.rocks/t/3-stage-standards-process-guaranteeing-an-open-and-decentralized-ecosystem/3602
[Living Standard Process]: https://indieweb.org/specifications
[Social Web Protocols]: https://www.w3.org/TR/social-web-protocols/
[TC39 Proposals]: https://github.com/tc39/proposals
[TC39 Process Document]: https://tc39.es/process-document/
[TC39 Decorators Proposal]: https://github.com/tc39/proposal-decorators
[TC39 Temporal Proposal]: https://github.com/tc39/proposal-temporal
[IW Proposals]: https://github.com/immersive-web/proposals
[IW Stage 0 Proposals]: https://github.com/immersive-web/proposals/issues
[IW Model Element Proposal]: https://github.com/immersive-web/model-element
[IW Depth Sensing Proposal]: https://github.com/immersive-web/depth-sensing
[WA Proposals]: https://github.com/WebAssembly/proposals
[WA Tail Call Proposal]: https://github.com/WebAssembly/tail-call
[WA GC Proposal]: https://github.com/WebAssembly/gc
