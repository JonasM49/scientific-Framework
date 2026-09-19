# GM-Exec Specification Development Template

VERSION: 1.6

DOCUMENT_IDENTIFIER: GM-Exec_Development_Template

ARCHITECTURE_LEVEL: GM Execution

DOCUMENT_TYPE: Template

DEPENDS_ON: GSL-2.0, GM-Core-v1.3

LANGUAGE: DSL SPECIFICATION_LINEAGE

AUTHOR: JonasM49

PUBLISHED_AT: 2026-09-19

CANONICAL_REPOSITORY: https://github.com/JonasM49/scientific-Framework

LICENSE: CC-BY-NC-SA-4.0


------------------------------------------------------------------------

## 0. Document Status

This document is the **Authoritative Baseline v1.6** of the GM-Exec
Specification Development Template, continuing the published Template
version lineage from v1.5 and incorporating the completed validation and
editorial consolidation. Chapters 1--11 and Appendix A contain the
controlled Integration Set application.

The template is an editorial development aid for creating consistent GM
Execution Specifications.

It is not part of the normative dependency hierarchy.

Execution Specifications developed from this template SHALL inherit only
from GSL and GM Core.

The objective of this template is to guide the consistent development of
valid GM Execution Specifications while preserving the validated
architectural structure.

### 0.1 Template Editing Convention

Template placeholders use the following syntax:

    {TYPE Subject LIKE Editorial guidance}

Where:

-   TYPE defines the expected form of the replacement (for example:
    DEFINITION, DESCRIPTION, LIST, RULE, STRUCTURE).

-   Subject identifies the execution-specific element to be replaced.

-   LIKE provides editorial guidance describing the required purpose,
    structure, or an exemplary specialization of the replacement.

The LIKE clause is editorial only.

All placeholders SHALL be replaced before an Execution Specification
reaches Release Candidate status.

### 0.2 Execution Architecture Consolidation Principles

The following principles guide the development and consolidation of GM
Execution Specifications.

These principles are informative. They support the production of
consistent, non-redundant, and maintainable Execution Specifications.

They do not introduce additional scientific requirements.

#### K1 -- Single Point of Scientific Definition

Each scientific property of a scientific object SHOULD be defined
normatively only once within an Execution Specification.

#### K2 -- Single Point of Scientific Responsibility

Each Scientific Working Method SHOULD define exactly one scientific
responsibility.

#### K3 -- Single Point of Scientific Lifecycle

Each scientific lifecycle stage SHOULD be specified only once.
Subsequent stages SHOULD reference, rather than redefine, preceding
stages.

#### K4 -- Reference Profile as Architectural Validation

The Reference Processing Profile SHOULD be used to verify that every
normative requirement is represented exactly once and that no additional
scientific rules are introduced by the Appendix.

#### K5 -- Architectural Layer Separation

Each chapter SHOULD define only its assigned architectural layer and
SHOULD NOT redefine responsibilities assigned to other chapters.

#### K6 -- Contract Minimality

Execution Contracts SHOULD define only execution input, execution output
and contractual obligations. Scientific behavior belongs to later
chapters.

#### K7 -- Artifact-Centric Definition

Scientific properties of execution-specific artifacts SHOULD be defined
only in the artifact chapter. Other chapters SHOULD reference those
definitions.

#### K8 -- Method Minimality

Scientific Working Methods SHOULD define only the scientific
transformation performed by the method. They SHOULD NOT redefine
artifact properties, workflow rules or execution contracts.

#### K9 -- Workflow Minimality

Scientific Processing Profiles SHOULD define only the orchestration of
Scientific Working Methods. They SHOULD reference, rather than redefine,
methods, artifacts and contracts.

### 0.3 Execution Specification Structure

The GM Execution Specification Template is divided into three editorial
parts.

#### Part I --- Execution-specific Scientific Architecture

Chapters 1 through 7 guide definition of the execution-specific
scientific architecture, including purpose and scope, normative
foundation, execution architecture, contract, result representation,
Scientific Working Methods, and Processing Profile Architecture.

These chapters contain editorial placeholders and SHALL be completed or
resolved by reference, specialization, applicability assessment, or an
explicit non-applicability statement as appropriate for each concrete GM
Execution.

#### Part II --- Configuration, Validation, Persistence and Conformance

Chapters 8 through 11 guide the execution-specific application of the
common GM Execution architecture through Processing Profile
Configuration, Validation, conditional Persistence and AGRAR Update, and
Execution Conformance.

These chapters contain both common architectural boundaries and
execution-specific development checkpoints. They SHALL be completed
according to applicability and SHALL reference inherited or previously
defined normative owners rather than redefine their semantics.

#### Part III --- Reference Processing Profiles

Appendix A contains execution-specific Reference Processing Profiles
where such profiles materially support implementation, review, or
third-party development.

These profiles illustrate conforming applications of the normative
execution architecture. They are non-normative and SHALL NOT become the
sole location of any requirement necessary for Execution completeness or
conformance.

## 1. Purpose and Scope

### 1.1 Purpose

This Execution shall own one clearly defined scientific responsibility:

{DEFINITION Execution-specific scientific responsibility LIKE DEFINE why
this Execution exists and identify the scientific responsibility
normatively owned by this Execution. Reference inherited semantics
rather than redefining responsibilities owned by GSL, GM Core, or
another normative specification point.}

{DESCRIPTION Execution-specific purpose LIKE explain the scientific
purpose served by this responsibility and identify the
execution-specific scientific boundary at a high level. Do not duplicate
the detailed Scientific Task, Result Representation, or Processing
Profile definitions of later sections.}

### 1.2 Scientific Task

The single scientific task through which this Execution realizes its
scientific responsibility is:

{DESCRIPTION Execution-specific scientific task LIKE DEFINE what
scientific task this Execution performs, including the
execution-specific scientific objective and intended result. Distinguish
the task from the higher-level purpose defined in Section 1.1.}

The Execution shall preserve the distinction between:

{LIST Execution-specific scientific boundary elements LIKE DEFINE the
scientific elements that must remain explicitly distinguishable
throughout this Execution. Reference inherited distinctions where their
semantics are already owned by GSL or GM Core.}

### 1.3 Scope

{LIST Execution-specific scope LIKE ASSESS and identify the scientific
responsibilities and processing activities belonging to this Execution.
Identify applicable result, validation, Relationship, handoff, and
persistence responsibilities without assuming that every such
responsibility applies. Reference inherited semantics where applicable.}

### 1.4 Out of Scope

This Execution shall define only the scientific responsibilities
assigned to its execution-specific scientific task.

{LIST Execution-specific out-of-scope responsibilities LIKE ASSESS
adjacent scientific responsibilities that are intentionally not owned by
this Execution. Identify their normative owner where known, and identify
downstream activities that begin only after the Execution Handoff
Boundary. Include responsibilities that belong to another GM Execution
or exceed the defined scientific boundary.}

### 1.5 Non-Destructive Principle

{ASSESS Execution-specific non-destructive requirements LIKE identify
scientific inputs, established Scientific Artifacts, or authoritative
scientific states whose identity or scientific meaning must not be
silently modified by this Execution. Reference applicable GSL and GM
Core preservation, provenance, lifecycle, and authority rules.}

Where correction, extension, alternative representation, or state change
is scientifically permitted, it SHALL occur only through the applicable
scientific responsibility and normative mechanism.

------------------------------------------------------------------------

### 1.6 Scientific Result Completeness Principle

{REFERENCE Execution Result Completeness LIKE identify the conditions
under which the execution-specific scientific result is complete. Define
the scientific result semantics and detailed completeness requirements
in the applicable Execution Contract and Scientific Result
Representation sections and reference them here rather than redefining
them.}

Execution completion SHALL depend on satisfaction of the applicable
scientific result completeness requirements and SHALL NOT be inferred
solely from completion of a particular Scientific Working Method.

## 2. Normative Foundation

### 2.1 General Scientific Layer

This Execution shall conform to the applicable scientific principles,
integrity requirements, traceability requirements, lifecycle rules, and
other inherited scientific requirements defined by the GSL.

GSL-owned semantics SHALL be referenced and applied. They SHALL NOT be
independently redefined by this Execution.

### 2.2 GM Core

This Execution shall conform to and use the applicable
genealogy-specific scientific architecture defined by GM Core, including
applicable Artifact, Relationship, register, project, and other Core
structures.

GM Core structures and semantics SHALL be referenced and applied. They
SHALL NOT be independently redefined by this Execution.

### 2.3 Normative Inheritance

The normative inheritance shall be:

``` text
{DEFINITION Execution specification name
 LIKE DEFINE the name of the concrete GM Execution}
    INHERITS GM Core
    INHERITS GSL
```

This Execution shall not inherit from another GM Execution.

No horizontal inheritance between Executions is permitted.

Concrete normative foundation versions SHOULD be identified in the
document metadata or applicable project specification without redefining
their semantics in this section.

------------------------------------------------------------------------

### 2.4 Scientific Preconditions

Before execution begins, the following execution-entry scientific
preconditions shall be satisfied:

{LIST Execution-specific scientific preconditions LIKE ASSESS and DEFINE
only scientific conditions that must already be satisfied before this
Execution can begin and that are specific to entry into this Execution.
Do not duplicate input validity owned by the Execution Contract,
applicability or sufficiency owned by Scientific Working Methods,
selection or escalation owned by Processing Profiles, or result validity
owned by Validation.}

Where no additional execution-specific scientific precondition exists
beyond inherited and contract-defined requirements, state that
explicitly.

### 2.5 Method and Processing Profile Foundation

{ASSESS Execution-specific method and profile requirements LIKE
determine whether this Execution requires Scientific Working Methods and
Processing Profile orchestration. Identify the applicable specification
sections in which method semantics and profile-owned selection,
sequencing, combination, escalation, stopping, and completion rules are
defined. Do not define those rules in this section.}

{REFERENCE Applicable method and profile normative owners LIKE reference
the Scientific Working Method and Processing Profile sections that own
the applicable execution-specific method semantics and orchestration
requirements. Where no additional execution-specific requirement
applies, state that explicitly.}

## 3. Execution Architecture

### 3.1 Execution Unit

This document specifies one independent GM Execution.

The Execution SHALL conform to the inherited GM Core requirements
governing Execution independence and absence of horizontal inheritance.

{ASSESS Execution-specific independence requirements LIKE determine
whether this Execution requires additional execution-specific
independence constraints beyond the inherited architecture. Define only
such additional constraints here.}

### 3.2 Pipe Model

The normative execution pipe shall be:

``` text
1. Execution Input
    {DEFINITION Execution-specific input
     LIKE DEFINE the scientific input accepted by this Execution}

2. Execution-specific Scientific Processing
    {DEFINITION Execution-specific scientific task
     LIKE REFERENCE the scientific task defined in Chapter 1 and identify
     its place in the execution pipe without redefining its semantics}

3. Execution Result
    {DESCRIPTION Execution-specific validated scientific result
     LIKE DEFINE the result produced after successful scientific
     processing and validation without assuming Artifact creation,
     Relationship creation, or persistence}

4. Execution Handoff Boundary
    {DESCRIPTION Execution-specific handoff
     LIKE DEFINE what validated result and documented result components
     may be relied upon by subsequent processing}

5. Subsequent Processing [where applicable]
    {ASSESS Subsequent processing
     LIKE identify whether persistence, another Execution, or other
     downstream processing occurs after the Handoff Boundary. Do not
     represent such subsequent processing as part of this Execution
     unless this Execution explicitly owns that responsibility}
```

Successful completion of this Execution SHALL establish the Validated
Execution Result defined by the applicable Execution Contract and
Validation requirements.

Successful completion SHALL NOT by itself imply Artifact creation,
Relationship creation, persistent AGRAR modification, or establishment
of a Register Revision unless the applicable execution-specific
responsibility is explicitly defined.

### 3.3 Execution Handoff Boundary

This Execution SHALL define the boundary at which its Validated
Execution Result becomes available to subsequent processing.

{DESCRIPTION Execution-specific transferable result LIKE DEFINE the
validated result and documented result components that may cross the
Execution Handoff Boundary.}

The following responsibilities SHALL be assessed independently:

{ASSESS Execution-specific result responsibilities LIKE determine
independently whether this Execution: - creates one or more Scientific
Artifacts; - creates or requires Relationships as part of its result; -
owns persistent AGRAR modification or establishment of a Register
Revision. A positive determination for one responsibility SHALL NOT
imply either of the others.}

{DESCRIPTION Execution-specific responsibility boundary LIKE DEFINE
where this Execution ends and identify any subsequent persistence or
downstream processing that lies beyond the Handoff Boundary.}

### 3.4 Execution Independence

A consuming Execution or subsequent scientific process SHALL NOT require
knowledge of:

{LIST Execution-specific internal working information LIKE DEFINE
temporary, intermediate, or undocumented execution-specific working
information that remains internal and does not form part of the
Validated Execution Result or documented Handoff.}

A consuming Execution or subsequent scientific process SHALL rely only
on applicable documented scientific structures and transferable result
components, including where applicable:

-   inherited GSL and GM Core structures;
-   the Validated Execution Result;
-   the documented execution-specific Result Representation;
-   explicitly transferable Relationships or other result components;
-   the defined Execution Handoff Boundary.

The concrete applicable components SHALL be defined by this Execution
and SHALL NOT be inferred merely from the general Template structure.

### 3.5 No Horizontal Inheritance

This Execution SHALL conform to the inherited GM Core rule prohibiting
horizontal inheritance between GM Executions.

Compatibility between Executions SHALL be established through applicable
shared Core structures, documented result representations, and explicit
input/output and Handoff contracts.

{ASSESS Additional execution-specific independence constraints LIKE
determine whether additional constraints are scientifically required
beyond the inherited No Horizontal Inheritance rule. Define only those
execution-specific constraints here.}

### 3.6 No Hidden State Transfer

Only

{LIST Execution-specific transferable scientific results LIKE DEFINE the
documented Validated Execution Result and additional transferable result
components, if any, that may cross the Execution Handoff Boundary}

may pass through the execution pipe.

Temporary, intermediate, or undocumented internal state SHALL NOT become
an implicit dependency of subsequent processing.

A subsequent Execution or scientific process SHALL NOT depend on
undocumented internal state.

------------------------------------------------------------------------

## 4. Execution Contract

### 4.1 Required Input

A conforming execution instance shall receive:

{DESCRIPTION Execution-specific required input LIKE DEFINE all mandatory
scientific input that a conforming execution instance must receive,
including applicable Scientific Artifacts, representations, references,
defined state inputs, or other scientifically required input structures.

Reference execution-entry preconditions defined in Section 2.4 rather
than redefining them here. Define only the execution contract;
scientific behavior belongs to its applicable normative owner.}

### 4.2 Conditional Input

Where required by the applicable Scientific Working Method, Processing
Profile, or documented execution condition, the execution instance may
additionally receive:

{LIST Execution-specific conditional input LIKE ASSESS and DEFINE all
permitted additional scientific input, parameters, profiles, references,
navigation information, or supporting material, and identify the
documented condition under which each becomes applicable.}

Conditional input SHALL NOT silently alter the scientific meaning of the
execution input.

Acceptance of a method- or profile-related parameter as input SHALL NOT
redefine the method or Processing Profile semantics that govern its use.

### 4.3 Input Validity

{DESCRIPTION Execution-specific input validity rules LIKE DEFINE the
conditions under which execution input SHALL be accepted, rejected, or
considered incomplete. Reference inherited scientific integrity
requirements where applicable rather than redefining them.}

An execution instance SHALL NOT compensate for invalid input by
inventing scientific evidence or silently completing missing scientific
information.

### 4.4 Required Output

{DESCRIPTION Execution-specific required output LIKE DEFINE the
Validated Execution Result produced by this Execution and the
contractual obligations that result must satisfy.

Define only the required execution output. Artifact semantics,
Relationship semantics, Validation procedures, Handoff rules, and
persistence semantics SHALL be referenced from their applicable
normative owners rather than redefined here.}

The required output SHALL represent the Validated Execution Result of
this Execution.

Where this Execution owns additional Artifact, Relationship, Handoff, or
persistence responsibilities, those responsibilities SHALL be defined by
their applicable normative sections and referenced here where
contractually required.

### 4.5 Result Representation Description

{ASSESS Execution-specific result representation description LIKE
determine whether the Validated Execution Result requires a
project-retained Artifact type description, dataset description, or
another persistent result representation description.

If applicable, DEFINE the execution-specific responsibility and
representation requirements. If the representation is inherited or
already established, REFERENCE it. If no additional result
representation description is required, state this explicitly.}

### 4.6 Output State

Successful completion of this Execution SHALL establish a Validated
Execution Result satisfying the applicable Execution Contract,
Scientific Result Representation, and Validation requirements.

{ASSESS Additional execution-specific output state LIKE determine
whether this Execution additionally owns establishment of a persistent
scientific state, AGRAR modification, or Register Revision. If
applicable, REFERENCE the responsible persistence section. Do not infer
persistence from successful validation alone.}

Validation PASS SHALL NOT by itself imply persistent scientific state
modification.

### 4.7 Prohibited Output

This Execution SHALL NOT produce scientific results that are assigned to
another GM Execution or another normative owner.

{LIST Execution-specific prohibited output LIKE DEFINE scientific
results that SHALL NOT be produced by this Execution because they belong
to another GM Execution, another normative owner, or violate the Scope
and Out-of-Scope boundaries established in Chapter 1. Reference those
boundaries rather than redefining them.}

### 4.8 Failure Output

Where the required Validated Execution Result cannot be produced, the
Execution MAY produce a documented incomplete or rejected processing
result.

Such a result SHALL NOT be represented as a successful Validated
Execution Result.

{ASSESS Execution-specific failure representation LIKE determine whether
additional execution-specific information must be retained with an
incomplete or rejected processing result. Define only such additional
requirements and reference applicable Validation and Processing Profile
rules.}

------------------------------------------------------------------------

## 5. Scientific Result Representation

### 5.1 Scientific Role

{DESCRIPTION Execution-specific scientific result representation LIKE
DEFINE the scientific role, purpose, scope, and representation of the
Validated Execution Result.

Identify which result components, if any, are Scientific Artifacts,
Relationships, persistent state representations, or other documented
scientific result structures.

Scientific properties SHOULD be defined here only once and referenced by
subsequent chapters rather than redefined.}

### 5.2 Core Basis

The Scientific Result Representation SHALL use applicable scientific
structures and semantics defined by GM Core.

Inherited structures and semantics SHALL be referenced and applied. They
SHALL NOT be independently redefined by this Execution.

{SPECIALIZE Execution-specific result semantics LIKE DEFINE only the
additional execution-specific semantics required to represent the
Validated Execution Result. Where GM Core already owns the applicable
semantics, REFERENCE them instead.}

### 5.3 Persistent Artifact Identity

{ASSESS Persistent Scientific Artifact Identity LIKE determine whether
this Execution creates or establishes persistent Scientific Artifacts.

If applicable, REFERENCE inherited GM Core Artifact identity semantics
and DEFINE only additional execution-specific constraints. Assess, where
relevant, independence from the producing tool, temporary execution
workspace, later derived Artifacts, and subsequent Executions.

If persistent Scientific Artifacts are not established by this
Execution, state this explicitly.}

### 5.4 Artifact Relationships

{ASSESS Execution-specific Relationships LIKE determine whether
Relationships form part of the Validated Execution Result or are
required to represent its scientific meaning, provenance, or context.

If applicable, REFERENCE inherited GM Core Relationship semantics and
DEFINE only execution-specific requirements. If no additional
Relationship responsibility applies, state this explicitly.}

### 5.5 Result Independence

{RULE Execution-specific result independence LIKE DEFINE the information
and documented representation required for subsequent processing to use
the Validated Execution Result without relying on undocumented internal
execution state.

REFERENCE the Execution Independence and No Hidden State Transfer
requirements in Chapter 3 rather than redefining the Handoff Boundary.}

### 5.6 Scientific Boundary

{RULE Execution-specific scientific boundary LIKE DEFINE which
scientific meaning is represented by the Validated Execution Result and
which transformations, interpretations, or downstream operations SHALL
NOT be treated as part of that result.

REFERENCE the Scope and Out-of-Scope boundaries in Chapter 1 where
applicable rather than redefining them.}

### 5.7 Uncertainty Representation

{ASSESS Execution-specific uncertainty representation LIKE REFERENCE
inherited GSL and GM Core uncertainty semantics and determine whether
the Validated Execution Result requires additional execution-specific
representation rules.

DEFINE only such additional rules. Where no additional
execution-specific uncertainty representation is required, state this
explicitly.}

### 5.8 Result Representation Description

{DESCRIPTION Execution-specific result representation description LIKE
where Section 4.5 establishes that a project-retained Artifact type
description, dataset description, or another persistent result
representation description is required, DEFINE its execution-specific
content and representation requirements here.

Describe the representation only. Scientific behavior belongs to its
applicable normative owner. If no additional retained representation
description is required, state this explicitly.}

### 5.9 Derived Scientific Artifacts

{ASSESS Derived Scientific Artifact responsibility LIKE determine
whether creation of Derived Scientific Artifacts belongs to this
Execution.

If YES: - REFERENCE inherited GM Core derivation semantics; - DEFINE the
execution-specific result types established by this Execution; - DEFINE
only additional execution-specific derivation constraints.

If NO: - state that derivation belongs to subsequent processing; -
REFERENCE the applicable Execution Handoff Boundary; - do not define how
another Execution performs that derivation.}

------------------------------------------------------------------------

## 6. Scientific Working Methods

### 6.1 Purpose

#### 6.1.1 Scientific Purpose

The purpose of the Scientific Working Methods is to define the
scientific methods and working aids that MAY be used by this Execution
to produce scientifically reproducible results.

Scientific Working Methods define how scientific work is performed
within their defined scientific scope.

They SHALL NOT define:

-   execution-wide workflow orchestration;
-   cross-method processing sequences;
-   cross-method selection, combination, escalation, or stopping rules;
-   Execution Result Representation;
-   persistent register modification procedures;
-   project-specific Processing Profile configurations.

These responsibilities belong to their applicable normative owners.

#### 6.1.2 Architectural Role

Scientific Working Methods form the methodological layer of the GM
Execution.

They provide reusable scientific methods that MAY be referenced by one
or more Scientific Processing Profiles.

A Scientific Working Method SHALL define its scientific semantics
independently of a specific Processing Profile.

#### 6.1.3 Scientific Independence

A Scientific Working Method defines a scientific method only.

It SHALL NOT prescribe:

-   when an otherwise applicable method is selected;
-   the cross-method order in which methods are applied;
-   how otherwise applicable methods are combined;
-   cross-method escalation or stopping;
-   the scientific scope of the Execution;
-   the Execution Result Representation.

These responsibilities belong to the applicable normative owner,
including the Processing Profile where orchestration is required.

An intrinsic scientific dependency that forms part of the method itself
MAY be defined by that method in accordance with Section 6.2.5.

#### 6.1.4 Relationship to Scientific Processing Profiles

Scientific Processing Profiles MAY apply one or more Scientific Working
Methods as permitted by the applicable Execution.

A Processing Profile MAY refine the application of a method for a
specific scientific task or context.

It SHALL NOT redefine or weaken the normative scientific requirements of
the referenced Scientific Working Method.

Selection, sequencing, combination, escalation, and stopping across
otherwise applicable methods belong to the Processing Profile.

### 6.2 Scientific Working Principles

#### 6.2.1 Purpose

Scientific Working Principles define the common execution-specific
scientific principles that SHALL apply to Scientific Working Methods
defined by this Execution.

Concrete methods SHALL inherit these principles where applicable unless
explicitly strengthened.

Inherited GSL and GM Core scientific principles SHALL be referenced and
SHALL NOT be independently redefined here.

#### 6.2.2 Scientific Method Principle

Scientific Working Methods SHALL define reproducible scientific
procedures for achieving their assigned scientific purpose.

Each Scientific Working Method SHALL define the conditions under which
its results are scientifically reproducible within its defined scope.

#### 6.2.3 Scientific Integrity Principle

Scientific Working Methods SHALL preserve the scientific integrity of
their assigned scientific task.

They SHALL NOT silently perform scientific responsibilities that are
outside their defined scope or assigned to another Scientific Working
Method, GM Execution, or normative owner.

Inherited scientific uncertainty and limitation requirements SHALL be
preserved. Additional execution-specific requirements MAY be defined
only where necessary.

#### 6.2.4 Scientific Sufficiency

Each Scientific Working Method SHALL define the conditions under which
its result is scientifically sufficient for the method's defined
processing scope.

The objective SHALL NOT be maximum detail but scientifically sufficient
reproducibility for that scope.

Scientific Sufficiency SHALL be defined here for the method and
referenced by Method Completion rather than independently redefined
there.

#### 6.2.5 Method Relationships and Dependencies

{ASSESS Scientific Working Method relationships LIKE determine whether
any Scientific Working Method has an intrinsic scientific dependency on,
refinement of, prerequisite relationship to, or incompatibility with
another method.

DEFINE such a relationship only where it is scientifically inherent to
the method itself.

Selection, sequencing, combination, escalation, and stopping across
otherwise applicable methods belong to the Processing Profile and SHALL
NOT be defined here merely as a preferred workflow.}

### 6.2.6 Working Representations

Scientific Working Methods MAY construct temporary scientific Working
Representations to support the scientific method.

A Working Representation SHALL NOT acquire persistent scientific status
merely because it is used by a Scientific Working Method or Processing
Profile.

Persistent status, where applicable, SHALL be established only by the
applicable Result Representation, Artifact, or persistence
responsibility.

### 6.2.7 Method Completion

A Scientific Working Method is complete when it satisfies the Scientific
Sufficiency conditions defined for that method in Section 6.2.4 and any
additional method-specific completion requirements.

Method Completion SHALL be distinguished from Processing Profile
Completion and Execution Completion.

Subsequent method selection, sequencing, escalation, combination, or
stopping belongs to the applicable Processing Profile where
orchestration is required.

### 6.3 Execution-specific Scientific Working Methods

{DESCRIPTION Execution-specific Scientific Working Methods LIKE DEFINE
each Scientific Working Method required or permitted by this Execution.

For each method ASSESS and document as applicable: - scientific
purpose; - applicability; - required method input; - scientific
capability; - scientific procedure or method principle; - scientific
integrity requirements; - Working Representations; - limitations; -
Scientific Sufficiency; - Method Completion; - intrinsic dependencies or
relationships to other methods.

Do not define Processing Profile-owned selection, sequencing,
combination, escalation, or stopping rules here.}

------------------------------------------------------------------------

## 7. Scientific Processing Profiles

### 7.1 Purpose

#### 7.1.1 Scientific Purpose

Scientific Processing Profiles define reproducible orchestration for
applying applicable Scientific Working Methods to a defined scientific
processing task.

A Scientific Processing Profile specifies when, for which scientific
purpose, and through which permitted sequence, combination, escalation,
stopping, or other orchestration applicable Scientific Working Methods
are used.

### 7.1.2 Architectural Role

Scientific Processing Profiles form the orchestration layer of the GM
Execution.

They SHALL, where applicable:

-   select applicable Scientific Working Methods;
-   define reproducible processing sequences;
-   combine applicable Scientific Working Methods;
-   define conditional branching or escalation;
-   define stopping conditions;
-   define workflow stages and stage dependencies;
-   define profile-owned processing decisions;
-   define Processing Profile Completion.

They SHALL NOT redefine or weaken:

-   Scientific Working Method semantics;
-   Execution Result semantics;
-   Scientific Result Representation;
-   inherited Artifact or Relationship semantics;
-   persistence authority.

### 7.1.3 Relationship to Scientific Working Methods

Scientific Processing Profiles MAY apply one or more Scientific Working
Methods permitted by this Execution.

Scientific Working Methods define how a scientific method works.

Scientific Processing Profiles define when, why, in which permitted
sequence or combination, and until when applicable methods are used.

A Processing Profile SHALL NOT redefine or weaken the normative
scientific requirements of a referenced Scientific Working Method.

### 7.1.4 Relationship to Processing Profile Configuration

Concrete Processing Profile configurations defined in Chapter 8 SHALL
conform to the Processing Profile Architecture defined by this chapter.

Chapter 7 defines the common Processing Profile Architecture.

Chapter 8 defines permitted Processing Profile Configuration.

Appendix A MAY provide a Reference Processing Profile demonstrating a
conforming configuration.

### 7.2 Workflow Principles

#### 7.2.1 Purpose

Workflow Principles define the common orchestration requirements
inherited by Scientific Processing Profiles defined by this Execution.

Concrete Processing Profile configurations SHALL conform to these
principles where applicable unless an explicitly permitted refinement
strengthens them without changing their normative scientific meaning.

#### 7.2.2 Workflow Principle

Scientific Processing Profiles SHALL orchestrate valid scientific input
through controlled and reproducible scientific processing toward the
Candidate Execution Result and applicable Validation boundary.

The workflow SHALL remain non-destructive.

No workflow stage SHALL silently modify the scientific meaning of the
input, Scientific Working Methods, or Execution Result.

A Processing Profile SHALL NOT imply persistent AGRAR modification or
establishment of a Register Revision unless that persistence
responsibility is independently owned and defined by this Execution.

#### 7.2.3 Processing Sequence

A Scientific Processing Profile SHALL define a controlled and
reproducible processing sequence where sequencing is required.

The sequence MAY include sequential, parallel, alternative, conditional,
or iterative processing where permitted by the Execution.

Stages defined as mandatory by the applicable Processing Profile SHALL
NOT be omitted.

### 7.2.4 Stage Responsibility

Each workflow stage SHALL possess one clearly defined orchestration
responsibility.

A workflow stage SHALL NOT redefine a Scientific Working Method,
Execution Result, Validation requirement, or other scientific
responsibility owned elsewhere.

Representation of a scientific responsibility as a workflow stage SHALL
NOT by itself create a new normative owner for that responsibility.

### 7.2.5 Traceable Processing

Processing shall be orchestrated in a manner that preserves scientific
traceability across applicable workflow stages and branches.

A stage MAY depend on the documented result or completion state of
another stage where such dependency is defined by the applicable
Processing Profile.

The Processing Profile MAY use sequential, parallel, alternative,
conditional, or iterative orchestration where scientifically appropriate
and reproducibly defined.

### 7.2.6 Workflow Completion

A Scientific Processing Profile is complete when its applicable
mandatory workflow stages and profile-owned stopping conditions have
been satisfied and the processing state required for the applicable
Execution Result and Validation boundary has been reached.

Processing Profile Completion SHALL NOT by itself imply:

-   Validation PASS;
-   Execution Completion;
-   persistent AGRAR modification;
-   establishment of a Register Revision.

### 7.3 Execution-specific Scientific Processing Profiles

{DESCRIPTION Execution-specific Scientific Processing Profile
Architecture LIKE DEFINE the orchestration requirements applicable to
this Execution.

ASSESS and document as applicable: - applicable Scientific Working
Methods; - method selection; - sequencing; - combination; - conditional
branching; - escalation; - stopping; - workflow stages; - stage
responsibilities; - dependencies between stages; - failure handling; -
Validation boundary; - Processing Profile Completion; - relationship to
the Execution Handoff Boundary; - a conditional persistence stage only
where this Execution owns that responsibility.

Do not redefine Scientific Working Method semantics, Execution Result
semantics, Scientific Result Representation, inherited Artifact or
Relationship semantics, or persistence authority.}

------------------------------------------------------------------------

## 8. Processing Profile Configuration

### 8.1 Purpose

A Scientific Processing Profile configuration SHALL define a documented
application of the Processing Profile Architecture for a specific
execution situation without changing the normative scientific meaning of
the Execution, Scientific Working Methods, or Validated Execution
Result.

{ASSESS Execution-specific configurable profile elements LIKE identify
which parameters, method selections, sequencing, combinations,
conditional branches, escalation conditions, stopping conditions,
workflow stages, or other profile-owned orchestration decisions may be
configured for a concrete execution situation.}

### 8.2 Reference Processing Profile

Each GM Execution SHOULD provide one Reference Processing Profile where
a reference configuration materially supports implementation, review, or
third-party development.

The Reference Processing Profile illustrates a conforming application of
the Scientific Working Methods defined in Chapter 6, the Processing
Profile Architecture defined in Chapter 7, and the configuration
boundary defined by this chapter.

The Reference Processing Profile is a conforming demonstration and SHALL
NOT be the sole normative location of an Execution requirement.

Removal of the Reference Processing Profile SHALL leave the normative
Execution specification scientifically complete and independently
developable.

Projects MAY define their own Scientific Processing Profile
configurations within the variability permitted by this Execution.

The Reference Processing Profile MAY be provided in Appendix A.

### 8.3 Processing Profile Boundary

The applicable normative ownership shall remain separated as follows:

-   the Execution Scope and Contract define the scientific task and
    contractual input/output requirements;
-   the Scientific Result Representation defines the scientific meaning
    and representation of the Validated Execution Result;
-   Scientific Working Methods define method semantics;
-   the Processing Profile Architecture defines orchestration semantics;
-   Processing Profile Configuration defines concrete permitted
    orchestration choices;
-   Validation assesses the Candidate Execution Result against
    applicable requirements;
-   persistence is defined only where independently owned by this
    Execution.

A Processing Profile configuration SHALL NOT alter the normative
scientific meaning of the Execution, Scientific Working Method, or
Validated Execution Result.

{ASSESS Execution-specific configuration boundary LIKE DEFINE the
variability permitted for concrete Processing Profile configurations and
REFERENCE the normative owner of any scientific responsibility that the
configuration uses but does not own.}

### 8.4 Profile Boundary

A Scientific Processing Profile configuration MAY configure
execution-specific scientific processing behavior within the variability
permitted by this Execution.

It SHALL NOT:

-   redefine Scientific Working Method semantics;
-   redefine the Execution Result or Scientific Result Representation;
-   weaken applicable Validation requirements;
-   create persistence authority;
-   introduce responsibilities belonging to another GM Execution or
    normative owner;
-   silently change inherited GSL or GM Core semantics.

A configuration outside the variability permitted by this Execution
SHALL NOT be represented as a conforming Processing Profile
configuration merely by project-specific declaration.

### 8.5 Project-specific Processing Profiles

{ASSESS Project-specific profile refinement LIKE determine whether
projects may define Processing Profile configurations beyond the
Reference Processing Profile.

DEFINE as applicable: - permitted configuration variability; - required
inherited constraints; - project-specific parameters; - permitted method
selection or orchestration choices; - conditions requiring a new or
revised Execution specification rather than a project-specific profile.

Project-specific refinement SHALL remain within the normative
variability permitted by this Execution.}

------------------------------------------------------------------------

## 9. Validation

### 9.1 Validation Goal

Validation SHALL determine whether the Candidate Execution Result
satisfies all applicable inherited and execution-specific scientific
requirements required for a Validated Execution Result.

Validation SHALL assess the result and SHALL NOT redefine the scientific
meaning of that result.

Validation PASS SHALL NOT by itself imply persistence.

### 9.2 Validation Areas

{ASSESS Execution-specific Validation Areas LIKE determine all
applicable validation areas, including as relevant:

-   inherited scientific integrity requirements;
-   traceability;
-   preservation of uncertainty;
-   absence of silent completion or invention;
-   conformity with the Execution Contract;
-   conformity with the Scientific Result Representation;
-   conformity with applicable Scientific Working Methods;
-   conformity with the selected Processing Profile;
-   conformity with applicable GM Core structures;
-   Artifact validity, where Artifacts are produced;
-   Relationship validity, where Relationships form part of the result;
-   source or locator completeness, where required by the Execution;
-   scientific reproducibility;
-   conformity with Scope and Scientific Boundary;
-   applicable Handoff requirements.

Do not require a validation area merely because it appears in this
Template when it is not applicable to the concrete Execution.}

### 9.3 Invalid Results

A Candidate Execution Result that fails applicable Validation
requirements SHALL NOT be represented as a Validated Execution Result.

An incomplete or rejected processing result SHALL remain distinguishable
from a successful Validated Execution Result.

The handling of incomplete or rejected processing results SHALL follow
Section 4.8 and the applicable execution-specific Scientific Processing
Profile.

### 9.4 Validation Outcome

{DEFINE Execution-specific Validation Outcome LIKE define the conditions
producing:

PASS → Candidate Execution Result satisfies all applicable Validation
requirements and becomes a Validated Execution Result.

FAIL → one or more applicable Validation requirements are not satisfied
and the Candidate Execution Result remains incomplete or rejected.

Define additional execution-specific outcome information only where
scientifically required.}

### 9.5 Handoff Eligibility

A Validated Execution Result SHALL be eligible for the Execution Handoff
defined in Chapter 3.

{ASSESS Execution-specific Handoff eligibility LIKE determine whether
additional execution-specific conditions must be satisfied after
Validation PASS before the result may cross the Execution Handoff
Boundary.

Do not duplicate Validation requirements and do not infer persistent
AGRAR modification from Handoff eligibility.}

------------------------------------------------------------------------

## 10. Conditional Persistence and AGRAR Update

### 10.1 Persistence Responsibility

{ASSESS Execution-specific persistence responsibility LIKE determine
whether this Execution itself owns a persistent modification of the
AGRAR.

If YES: - DEFINE the Execution-specific persistence operation; -
IDENTIFY the Validated Execution Result eligible for persistence; -
REFERENCE inherited AGRAR and AWE semantics; - DEFINE any additional
execution-specific integrity conditions; - DEFINE the resulting
authoritative register state where applicable.

If NO: - STATE that this Execution does not modify the AGRAR; -
REFERENCE the Execution Handoff Boundary; - do not define an equivalent
persistence procedure.}

### 10.2 Controlled AGRAR Update

Where this Execution owns AGRAR persistence, only a Validated Execution
Result eligible under the applicable persistence contract MAY enter the
Controlled AGRAR Update.

The Controlled AGRAR Update SHALL preserve inherited AGRAR, AWE,
provenance, traceability, integrity, and authoritative-state
requirements.

The Execution SHALL define only those additional persistence conditions
that are specific to its own scientific responsibility.

### 10.3 Authoritative Register State

Where a Controlled AGRAR Update is performed, the resulting
authoritative register state SHALL be established in accordance with the
inherited AGRAR and AWE requirements.

This Execution SHALL NOT independently redefine:

-   Register Revision semantics;
-   authoritative-state succession;
-   predecessor relationships;
-   reproducibility requirements;
-   authority transfer;
-   recovery semantics.

{DEFINE only additional Execution-specific requirements for the
resulting register state, where scientifically necessary.

Where persisted results require an execution-specific type, dataset, or
Result Representation description, REFERENCE its normative definition in
Chapter 5 rather than redefining it here.}

### 10.4 Non-Persistent Execution

Where this Execution does not own persistent AGRAR modification,
successful Execution Completion SHALL end at the applicable Execution
Handoff Boundary.

A subsequent Execution or other authorized processing architecture MAY
consume the Validated Execution Result according to its own applicable
contract.

The absence of persistence responsibility SHALL NOT be interpreted as
authorization for this Execution to create an alternative persistence
procedure.

------------------------------------------------------------------------

## 11. Execution Conformance

### 11.1 Aggregate Conformance Principle

A conforming implementation of this Execution SHALL satisfy all
applicable normative requirements inherited from GSL and GM Core and all
applicable normative requirements defined by this Execution.

This chapter summarizes conformance obligations and SHALL NOT
independently redefine scientific responsibilities owned elsewhere in
this specification.

### 11.2 Scientific Behavior over Implementation Form

Conformance SHALL be determined by observable scientific behavior and
satisfaction of applicable normative requirements, not by a particular
software architecture, storage technology, internal workflow
representation, or implementation mechanism unless such a mechanism is
itself explicitly required for scientific reasons.

### 11.3 Applicable Requirement Conformance

A requirement applies only where its normative applicability conditions
are satisfied.

An implementation SHALL NOT be considered non-conforming merely because
a conditional capability, Artifact, Relationship, Working Method,
Processing Profile element, or persistence operation is not applicable
to the concrete Execution situation.

Where a conditional requirement becomes applicable, all normative
requirements governing that condition SHALL be satisfied.

### 11.4 Execution Conformance Checklist

{DEFINE Execution Conformance Checklist LIKE verify, as applicable, that
the implementation:

-   accepts only valid Execution Input;
-   performs only the scientific task owned by this Execution;
-   remains within the defined Scope and Scientific Boundary;
-   preserves inherited provenance, traceability, and uncertainty;
-   applies applicable Scientific Working Methods conformingly;
-   applies the selected Processing Profile conformingly;
-   produces the defined Candidate Execution Result;
-   performs all applicable Validation;
-   represents Validation PASS only as a Validated Execution Result;
-   preserves incomplete or rejected results as distinguishable states;
-   respects the Execution Handoff Boundary;
-   creates Artifacts only where this Execution owns or requires them;
-   creates Relationships only where applicable;
-   performs persistence only where this Execution owns that
    responsibility;
-   conforms to inherited AGRAR/AWE requirements where persistence
    applies;
-   avoids horizontal inheritance;
-   avoids hidden dependencies on undocumented internal state;
-   satisfies all additional execution-specific normative requirements.

Include only applicable requirements in the concrete conformance
determination.}

------------------------------------------------------------------------

## Appendix A --- Reference Processing Profiles

### A.1 Purpose

This Appendix is non-normative.

It provides one or more Reference Processing Profiles illustrating
conforming configurations of this Execution.

A Reference Processing Profile demonstrates one conforming configuration
of the applicable normative architecture.

It SHALL NOT establish a normative requirement that is not defined in
the normative body of this Execution.

Removal of this Appendix or of an individual Reference Processing
Profile SHALL NOT remove a normative scientific requirement from the
Execution specification.

### A.2 Reference Processing Profiles

{DESCRIPTION Execution-specific Reference Processing Profiles LIKE
provide one or more complete conforming reference configurations
demonstrating the application of Chapters 6--10.

A Reference Processing Profile SHOULD make applicable choices explicit
without creating new normative requirements.

Use the following editorial structure as applicable:

\#### Profile Name \#### Scientific Purpose \#### Applicability \####
Execution Input \#### Scientific Working Methods \#### Method Selection
\#### Processing Sequence and Orchestration \#### Conditional Branching
/ Escalation / Stopping {WHERE APPLICABLE} \#### Candidate Execution
Result \#### Validation \#### Validated Execution Result \#### Failure
Handling \#### Processing Profile Completion \#### Execution Handoff
\#### Persistence / AGRAR Update {WHERE APPLICABLE}

A Reference Processing Profile SHALL include only configuration elements
applicable to the demonstrated execution situation.

Conditional elements SHALL be included where applicable and MAY be
explicitly identified as not applicable where doing so improves the
explanatory value of the reference configuration.}
