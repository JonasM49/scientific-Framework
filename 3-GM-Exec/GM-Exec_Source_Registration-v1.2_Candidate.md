# GM-Exec Source Registration

DOCUMENT_IDENTIFIER: GM-Exec_Source_Registration

DOCUMENT_TYPE: NormativeSpecification

VERSION: 1.2

STATUS: Candidate

ARCHITECTURE_LEVEL: GM Execution

NORMATIVE_FOUNDATION:

-   GSL v2.0
-   GM-Core v1.1

LANGUAGE: DSL SPECIFICATION_LINEAGE

AUTHOR: JonasM49

PUBLISHED_AT: 2026-09-19

CANONICAL_REPOSITORY: https://github.com/JonasM49/scientific-Framework

LICENSE: CC-BY-NC-SA-4.0


## 1. Purpose and Scope

### 1.1 Purpose

This Execution SHALL perform one clearly defined scientific source
registration.

The purpose of this Execution is the scientific registration of one
Scientific Source by establishing or reusing one `RegisteredSource`
within the AGRAR.

### 1.2 Scientific Task

The single scientific task of this Execution is the scientific
registration of Scientific Sources within the AGRAR.

The Execution SHALL preserve the distinction between:

-   Scientific Source;
-   Source Representation;
-   `RegisteredSource`;
-   `RegisterEntry`;
-   Register Revision.

### 1.3 Scope

This Execution defines the scientific scope of source registration.

Its scope includes:

-   scientific registration of one Scientific Source from one or more
    Source Representations;
-   establishment or reuse of one `RegisteredSource`;
-   preservation of scientific identity, provenance, traceability, and
    uniqueness throughout source registration;
-   representation of AGRAR membership through `RegisterEntry`;
-   production of a scientifically validated registration result
    eligible for Controlled AGRAR Update.

### 1.4 Out of Scope

This Execution SHALL define only the scientific responsibilities
assigned to its execution-specific scientific task.

-   creation of scientific representations of source content;
-   translation, normalization, interpretation, or reconstruction of
    source content;
-   extraction of genealogical or domain-specific information;
-   creation of execution-specific artifacts assigned to another GM
    Execution;
-   identity resolution or relationship generation;
-   scientific analysis or conclusions derived from registered sources.

### 1.5 Non-Destructive Principle

This Execution SHALL preserve the scientific identity of every
registered Scientific Source throughout the source registration process.

The Execution MAY extend an existing scientific registration where
additional scientifically valid information becomes available.

Such extensions SHALL preserve the inherited `RegisteredSource`
semantics and the execution-specific registration requirements defined
by this Execution.

The Execution SHALL NOT:

-   establish more than one `RegisteredSource` for the same Scientific
    Source;
-   silently replace the scientific identity of a registered Scientific
    Source;
-   remove or invalidate accepted Source Representations without
    explicit scientific justification;
-   compromise the traceability of the scientific registration.

------------------------------------------------------------------------

### 1.6 Scientific Result Completeness Principle

This Execution SHALL complete successfully only when the scientific
registration result is complete.

Scientific completeness SHALL be determined in accordance with the
scientific responsibilities, validation requirements, and execution
contract defined by this Execution.

The Execution SHALL NOT be considered complete merely because all
Scientific Working Methods have been executed.

Completion depends on the scientific completeness of the resulting
source registration.

## 2. Normative Foundation

### 2.1 General Scientific Layer

This Execution SHALL conform to the applicable scientific principles,
integrity requirements, traceability requirements, lifecycle rules, and
authoritative state requirements defined by GSL v2.0.

### 2.2 GM-Core

This Execution SHALL use the Scientific Artifact, Relationship, AGRAR,
RegisterEntry, Register Revision, and project structures defined by
GM-Core.

Inherited Core structures and semantic responsibilities SHALL be
referenced and applied. They SHALL NOT be redefined by this Execution.

### 2.3 Normative Inheritance

The normative inheritance SHALL be:

``` text
GM-Exec Source Registration
    INHERITS GM-Core
    INHERITS GSL
```

This Execution SHALL NOT inherit from another GM Execution.

No horizontal inheritance between Executions is permitted.

------------------------------------------------------------------------

### 2.4 Scientific Preconditions

Before execution begins, the following scientific preconditions SHALL be
satisfied:

-   at least one Source Representation is available;
-   the Source Representation is sufficiently accessible for scientific
    assessment;
-   the applicable project type descriptions are available;
-   the current valid Register Revision is available, unless this
    Execution establishes the initial valid Register Revision;
-   the Scientific Working Methods required by this Execution are
    available.

### 2.5 Scientific Working Method Architecture

The Scientific Working Methods defined by this Execution do not form a
method inheritance hierarchy.

Each Scientific Working Method defines one independent scientific
responsibility.

The execution-specific Scientific Processing Profile determines the
mandatory processing sequence.

No Scientific Working Method inherits from another Scientific Working
Method.

## 3. Execution Architecture

### 3.1 Execution Unit

This document specifies one independent GM Execution.

The Execution SHALL be usable without inheritance from, embedding of, or
direct control by another GM Execution.

### 3.2 Pipe Model

The normative execution pipe SHALL be:

``` text
1. Execution Input
    One or more Scientific Source Representations

2. Execution
    Scientific Source Registration

3. Execution Result
    Validated Scientific Source Registration

    One new valid Register Revision
        established through Controlled AGRAR Update
```

Successful completion of this Execution performs the Controlled AGRAR
Update and establishes one new valid Register Revision.

### 3.3 Pipe Boundary

This Execution defines the scientific processing boundary between
Execution Input and Execution Result.

Scientific processing performed by this Execution SHALL remain
execution-internal until successfully incorporated into the AGRAR
through the Controlled AGRAR Update.

No execution result SHALL become part of the AGRAR before successful
completion of the Controlled AGRAR Update.

### 3.4 Execution Independence

A consuming Execution SHALL NOT require knowledge of:

-   execution-internal processing state;
-   intermediate source identification candidates;
-   temporary source classification assessments;
-   temporary Working Representations;
-   undocumented validation information.

A consuming Execution SHALL rely on:

-   shared GM-Core structures and semantics;
-   the registered `RegisteredSource`;
-   its authoritative AGRAR membership represented by `RegisterEntry`;
-   the current valid Register Revision; and
-   applicable project-retained descriptions or persistent
    Relationships.

### 3.5 No Horizontal Inheritance

This Execution SHALL NOT inherit structure, behavior, or authority from
another GM Execution.

A subsequent Execution SHALL NOT inherit from this Execution.

Compatibility between Executions SHALL be established through shared
Core structures, project-retained type descriptions, and explicit
input/output contracts.

### 3.6 No Hidden State Transfer

Only persistent scientific results conforming to GM-Core and the
resulting authoritative AGRAR state MAY pass through the execution
boundary.

For this Execution this includes:

-   the registered `RegisteredSource`;
-   its `RegisterEntry`; and
-   the resulting valid Register Revision.

A subsequent Execution SHALL NOT depend on undocumented
execution-internal state.

## 4. Execution Contract

### 4.1 Required Input

A conforming execution instance SHALL receive:

-   one or more Source Representations;
-   access to the current valid Register Revision unless this Execution
    establishes the initial revision;
-   the applicable project-retained Source Type Descriptions;
-   the scientific preconditions defined by this Execution.

### 4.2 Conditional Input

Where required by the selected Scientific Processing Profile, the
execution instance MAY additionally receive:

-   existing `RegisteredSource` Artifacts;
-   locator information;
-   project-specific classification information.

Conditional input SHALL NOT silently alter the scientific meaning of the
execution input.

### 4.3 Input Validity

Execution input SHALL be accepted only where the represented Scientific
Source can be scientifically assessed.

Invalid, incomplete, or inaccessible Source Representations SHALL
produce a documented incomplete or rejected processing result.

An execution instance SHALL NOT compensate for invalid input by
inventing scientific evidence.

### 4.4 Required Output

A successful Execution SHALL produce or reuse one validated
`RegisteredSource` Scientific Artifact representing the registered
Scientific Source.

Validated results SHALL be incorporated into the AGRAR through the
Controlled AGRAR Update defined by this Execution.

The resulting Register Revision SHALL become the current authoritative
working state of the AGRAR in accordance with the inherited AWE requirements.

The execution instance SHALL preserve:

-   scientific identity;
-   source traceability;
-   justified uniqueness of the `RegisteredSource`;
-   AGRAR membership integrity;
-   execution provenance.

### 4.5 Persistent Representation Output

The persistent representation of results produced by this Execution
SHALL conform to the applicable inherited GM-Core requirements and any
applicable project-retained or execution-specific construction and
representation requirements.

This Execution SHALL NOT redefine the Core semantics or common structure
of `RegisteredSource`, `RegisterEntry`, or Register Revision.

### 4.6 Output State

The resulting Register Revision SHALL become the current authoritative
working state of the AGRAR in accordance with the inherited AWE requirements.

### 4.7 Prohibited Output

This Execution SHALL NOT produce scientific results that are assigned to
another GM Execution.

-   `ScientificObservation`;
-   `PersonIdentity`;
-   `Event`;
-   identity resolution;
-   Relationships whose scientific responsibility lies outside source
    registration;
-   translation, interpretation, or scientific conclusions derived from
    source content.

### 4.8 Failure Output

Where successful source registration is not possible, the Execution MAY
produce a documented incomplete or rejected processing result.

Such a processing result SHALL NOT be represented as a valid
`RegisteredSource` registration result unless it satisfies the
applicable GM-Core and execution-specific requirements.

------------------------------------------------------------------------

## 5. RegisteredSource Responsibilities and Representation

### 5.1 Scientific Role

The primary Scientific Artifact established or reused by this Execution
is `RegisteredSource`.

`RegisteredSource` is a Core Artifact Type defined by GM-Core. This
Execution SHALL NOT redefine its Core semantics.

This Execution defines the controlled formation, identification,
classification, construction, validation, and AGRAR incorporation
required to register one Scientific Source as one persistent
`RegisteredSource`.

A `RegisteredSource` SHALL provide the scientifically validated basis
through which the Scientific Source MAY enter controlled subsequent
scientific processing.

It SHALL NOT by itself represent source content, a
`ScientificObservation`, a `PersonIdentity`, an `Event`, or a scientific
interpretation of source content.

### 5.2 Core Basis and Execution Ownership

`RegisteredSource` SHALL use the common Scientific Artifact structure
and semantic responsibility defined by GM-Core.

This Execution owns only the processing rules required for source
registration, including:

-   assessment of available Source Representations;
-   Scientific Source identification;
-   Scientific Source classification;
-   registration decision;
-   construction or controlled extension of `RegisteredSource`;
-   registration validation;
-   Controlled AGRAR Update.

This Execution MAY define additional construction or representation
requirements where required for reproducible source registration.

Such requirements SHALL remain subordinate to inherited GM-Core
semantics and SHALL NOT redefine common Core structure.

### 5.3 Persistent Artifact Identity

Each `RegisteredSource` established by this Execution SHALL possess a
persistent Scientific Artifact identity according to GM-Core.

Its persistent identity SHALL remain independent of:

-   the identity of the producing actor or tool;
-   the temporary execution workspace;
-   later Scientific Artifacts derived from the source;
-   any subsequent Execution processing the source.

### 5.4 Relationships and Register Membership

Authoritative inclusion of a `RegisteredSource` in AGRAR SHALL be
represented through a `RegisterEntry` according to GM-Core.

This Execution SHALL NOT establish Relationships as part of its
source-registration result.

This restriction defines the scientific boundary of this Execution. It
SHALL NOT redefine or constrain the GM-Core Relationship architecture or
the authority of another conforming GM Execution to establish
Relationships within its own scientific responsibility.

### 5.5 Artifact Independence

The `RegisteredSource` SHALL be scientifically self-contained for the
purpose of source registration and subsequent controlled reuse.

A subsequent GM Execution SHALL require only:

-   the `RegisteredSource`;
-   its authoritative AGRAR membership represented by `RegisterEntry`;
-   the current valid Register Revision; and
-   the applicable project-retained descriptions.

A subsequent GM Execution SHALL NOT depend on:

-   execution-internal processing state;
-   temporary scientific assessments;
-   intermediate source identification candidates;
-   undocumented validation results;
-   execution-specific Working Representations.

The `RegisteredSource` and its authoritative AGRAR membership SHALL
provide the registered source information required for its intended
reuse by subsequent GM Executions.

### 5.6 Scientific Boundary

The `RegisteredSource` established or reused by this Execution SHALL
represent only the scientific registration of the represented Scientific
Source within the semantic responsibility defined by GM-Core.

The `RegisteredSource` SHALL NOT establish:

-   `ScientificObservation` Artifacts;
-   scientific interpretations;
-   genealogical assertions;
-   identity assertions;
-   event assertions;
-   scientific conclusions.

The scientific responsibility of this Execution ends with the successful
registration of the Scientific Source.

Any scientific processing beyond source registration SHALL be performed
by subsequent GM Executions operating on the `RegisteredSource`.

### 5.7 Uncertainty Representation

Scientific uncertainty represented by this Execution SHALL be limited to
uncertainty directly affecting the scientific registration of the
represented Scientific Source.

The `RegisteredSource` SHALL preserve explicit uncertainty where it
affects:

-   identification of the Scientific Source;
-   classification of the Scientific Source;
-   association of accepted Source Representations.

This Execution SHALL NOT introduce uncertainty derived from:

-   `ScientificObservation` Artifacts;
-   scientific interpretation;
-   genealogical analysis;
-   identity resolution;
-   scientific conclusions.

Scientific uncertainty SHALL remain explicitly distinguishable from
scientific facts.

Subsequent GM Executions MAY refine or resolve preserved uncertainty in
accordance with their own scientific responsibilities.

### 5.8 Persistent Representation

Persistent results of this Execution SHALL conform to the inherited
GM-Core Scientific Artifact, AGRAR, RegisterEntry, Register Revision,
Relationship, provenance, uncertainty, and validation requirements.

This Execution MAY define additional source-registration-specific
construction or representation requirements where scientifically
required.

Such requirements SHALL:

-   preserve inherited `RegisteredSource` semantics;
-   remain distinguishable from implementation-specific serialization;
-   preserve scientific identity, provenance, uncertainty, and
    traceability;
-   not redefine GM-Core responsibilities.

Concrete serialization formats SHALL NOT constitute normative scientific
requirements unless explicitly specified.

### 5.9 Derived Scientific Artifacts

The `RegisteredSource` MAY serve as scientific input for subsequent GM
Executions.

Derived Scientific Artifacts SHALL be established exclusively by the GM
Execution responsible for their scientific purpose.

This Execution SHALL NOT establish derived Scientific Artifacts.

Subsequent GM Executions MAY derive, where scientifically justified:

-   `ScientificObservation`;
-   `PersonIdentity`;
-   `Event`;
-   execution-specific Scientific Artifacts defined by the applicable GM
    Execution.

Every derived Scientific Artifact SHALL preserve explicit scientific
traceability to the `RegisteredSource` from which it was derived.

The establishment of derived Scientific Artifacts SHALL NOT modify the
scientific meaning or scientific identity of the `RegisteredSource`.

## 6. Scientific Working Methods

### 6.1 Scientific Working Method Overview

This Execution defines the following Scientific Working Methods:

-   Source Representation Assessment;
-   Scientific Source Identification;
-   Scientific Source Classification;
-   Source Registration Decision;
-   `RegisteredSource` Construction;
-   Registration Validation.

Each Scientific Working Method defines one independent scientific
responsibility.

The Scientific Working Method Architecture of this Execution is defined
in Section 2.5.

The execution-specific Scientific Processing Profile defines the
mandatory execution sequence of these Scientific Working Methods.

### 6.2 Scientific Working Principles

#### 6.2.1 Purpose

Scientific Working Principles define the common scientific principles
that SHALL apply to all Scientific Working Methods defined by this
Execution.

Concrete methods SHALL inherit these principles unless explicitly
strengthened.

#### 6.2.2 Scientific Method Principle

Scientific Working Methods SHALL define reproducible scientific
procedures for achieving their assigned scientific purpose.

Each Scientific Working Method SHALL produce scientifically reproducible
results within its defined scope.

#### 6.2.3 Scientific Integrity Principle

Scientific Working Methods SHALL preserve the scientific integrity of
their assigned scientific task.

They SHALL NOT silently perform scientific responsibilities that are
outside their defined scope or assigned to another Scientific Working
Method or GM Execution.

Scientific uncertainty and scientific limitations SHALL be represented
explicitly where applicable.

#### 6.2.4 Scientific Sufficiency

A Scientific Working Method SHALL achieve scientifically sufficient
quality for the defined processing scope.

The objective SHALL NOT be maximum detail but scientifically sufficient
reproducibility.

#### 6.2.5 Method Escalation

A more detailed Scientific Working Method SHOULD be applied only where
the preceding method cannot achieve scientifically sufficient quality.

Methods SHALL form a progressive scientific refinement.

#### 6.2.6 Working Representations

Scientific Working Methods MAY construct temporary scientific Working
Representations to support the scientific method.

Such Working Representations SHALL NOT constitute persistent Scientific
Artifacts unless explicitly specified by the applicable Scientific
Processing Profile.

#### 6.2.7 Method Completion

A Scientific Working Method is complete when it has achieved
scientifically sufficient results for the defined processing scope.

Subsequent processing belongs to the applicable Scientific Processing
Profile.

### 6.3 Execution-specific Scientific Working Methods

### 6.3.1 Source Representation Assessment

Purpose

Determine whether one or more available Source Representations are
scientifically sufficient to permit reliable registration of a
Scientific Source.

Applicability

This Scientific Working Method SHALL be performed before Scientific
Source Identification.

Inheritance

This Scientific Working Method SHALL inherit the Scientific Working
Principles defined by Section 6.2.

Normative Requirements

The assessment SHALL evaluate whether the available Source
Representations:

-   represent the same Scientific Source;
-   provide sufficient scientific information for reliable source
    identification;
-   preserve sufficient provenance for scientific traceability;
-   satisfy the minimum scientific quality required for source
    registration.

The assessment SHALL NOT:

-   perform scientific interpretation;
-   establish `ScientificObservation` Artifacts;
-   derive genealogical conclusions;
-   reject a Scientific Source solely because a Source Representation is
    incomplete.

Where multiple Source Representations are available, they MAY be
assessed together as scientific evidence for the same Scientific Source.

Completion Criteria

This Scientific Working Method is complete when the available Source
Representations have been determined to be either:

-   scientifically sufficient for Scientific Source Identification; or
-   scientifically insufficient for source registration.

### 6.3.2 Scientific Source Identification

Purpose

Identify the Scientific Source represented by one or more scientifically
sufficient Source Representations.

Applicability

This Scientific Working Method SHALL be performed only after successful
completion of Source Representation Assessment.

Inheritance

This Scientific Working Method SHALL inherit the Scientific Working
Principles defined by Section 6.2.

Normative Requirements

Scientific Source Identification SHALL:

-   identify the represented Scientific Source;
-   preserve the distinction between Scientific Source and Source
    Representation;
-   use all scientifically relevant Source Representations available for
    identification;
-   preserve scientific provenance throughout the identification
    process.

Scientific Source Identification SHALL NOT:

-   perform scientific registration;
-   establish `ScientificObservation` Artifacts;
-   derive scientific interpretations;
-   establish genealogical assertions;
-   resolve scientific identity beyond identification of the Scientific
    Source.

Where multiple Source Representations represent the same Scientific
Source, they SHALL contribute jointly to the identification.

Completion Criteria

This Scientific Working Method is complete when the represented
Scientific Source has been identified with sufficient scientific
certainty to permit Source Classification.

### 6.3.3 Scientific Source Classification

Purpose

Classify the identified Scientific Source according to the applicable
project-retained Source Type Descriptions.

Applicability

This Scientific Working Method SHALL be performed only after successful
completion of Scientific Source Identification.

Inheritance

This Scientific Working Method SHALL inherit the Scientific Working
Principles defined by Section 6.2.

Normative Requirements

Scientific Source Classification SHALL:

-   classify the identified Scientific Source according to the
    applicable project-retained Source Type Descriptions;
-   preserve the scientific identity established during Scientific
    Source Identification;
-   apply only project-retained classification definitions;
-   preserve scientific traceability of the classification.

Scientific Source Classification SHALL NOT:

-   redefine the identified Scientific Source;
-   establish `ScientificObservation` Artifacts;
-   derive scientific interpretations;
-   establish genealogical assertions;
-   establish execution-specific Relationships.

Where more than one classification is scientifically applicable, each
classification SHALL be represented explicitly according to the
applicable Source Type Descriptions.

Completion Criteria

This Scientific Working Method is complete when the identified
Scientific Source has been assigned all applicable scientific
classifications required for Source Registration.

### 6.3.4 Source Registration Decision

Purpose

Determine whether the identified and classified Scientific Source
requires establishment of a new `RegisteredSource` or reuse of an
existing RegisteredSource.

Applicability

This Scientific Working Method SHALL be performed only after successful
completion of Scientific Source Classification.

Inheritance

This Scientific Working Method SHALL inherit the Scientific Working
Principles defined by Section 6.2.

Normative Requirements

Source Registration Decision SHALL:

-   determine whether the Scientific Source has already been registered;
-   preserve the uniqueness of the `RegisteredSource`;
-   prevent duplicate registration of the same Scientific Source;
-   preserve scientific provenance and traceability.

Source Registration Decision SHALL NOT:

-   establish a RegisteredSource;
-   modify an existing `RegisteredSource`;
-   establish `ScientificObservation` Artifacts;
-   derive scientific interpretations;
-   establish execution-specific Relationships.

Where an existing `RegisteredSource` already represents the identified
Scientific Source, that artifact SHALL be selected for reuse.

Where no suitable `RegisteredSource` exists, the Scientific Source SHALL
be designated for new registration.

Completion Criteria

This Scientific Working Method is complete when a scientifically
justified registration decision has been established that permits
`RegisteredSource` Construction.

### 6.3.5 `RegisteredSource` Construction

Purpose

Establish a new `RegisteredSource` or extend an existing
`RegisteredSource` in accordance with the Source Registration Decision.

Applicability

This Scientific Working Method SHALL be performed only after successful
completion of Source Registration Decision.

Inheritance

This Scientific Working Method SHALL inherit the Scientific Working
Principles defined by Section 6.2.

Normative Requirements

`RegisteredSource` Construction SHALL:

-   establish one new `RegisteredSource` where required;
-   extend an existing `RegisteredSource` where justified by the Source
    Registration Decision and permitted by inherited GM-Core
    requirements;
-   preserve the scientific identity of the `RegisteredSource`;
-   preserve the uniqueness of the `RegisteredSource`;
-   preserve the traceable association of all accepted Source
    Representations;
-   conform to inherited GM-Core requirements and any applicable
    source-registration-specific construction or representation
    requirements.

`RegisteredSource` Construction SHALL NOT:

-   redefine the inherited semantic responsibility of
    `RegisteredSource`;
-   silently replace the scientific identity of the represented
    Scientific Source;
-   establish `ScientificObservation`, `PersonIdentity`, or `Event`
    Artifacts;
-   establish Relationships;
-   create duplicate `RegisteredSource` Artifacts.

Completion Criteria

This Scientific Working Method is complete when the `RegisteredSource`
has been established or extended in accordance with the Source
Registration Decision and all applicable inherited and
execution-specific requirements are satisfied.

### 6.3.6 Registration Validation

Purpose

Validate the scientific completeness and correctness of the source
registration result before Controlled AGRAR Update.

Applicability

This Scientific Working Method SHALL be performed only after successful
completion of `RegisteredSource` Construction.

Inheritance

This Scientific Working Method SHALL inherit the Scientific Working
Principles defined by Section 6.2.

Normative Requirements

Registration Validation SHALL verify that:

-   the `RegisteredSource` represents exactly one independently
    addressable Scientific Source;
-   the Scientific Source has been sufficiently identified and
    classified for the registration purpose;
-   the `RegisteredSource` conforms to inherited GM-Core requirements
    and any applicable source-registration-specific construction or
    representation requirements;
-   accepted Source Representations remain traceably associated with the
    source registration;
-   uncertainty affecting identification, classification, or association
    is explicitly preserved;
-   all persistent elements required for the complete registration
    result are present and valid.

Registration Validation SHALL NOT:

-   silently modify the `RegisteredSource`;
-   establish scientific responsibilities belonging to another
    Execution;
-   perform Controlled AGRAR Update.

Where validation identifies scientific deficiencies, the registration
result SHALL return to the applicable preceding scientific processing
stage before validation can complete successfully.

Completion Criteria

This Scientific Working Method is complete when the complete source
registration result has been scientifically validated and is eligible
for Controlled AGRAR Update.

## 7. Scientific Processing Profile Architecture

### 7.1 Purpose

#### 7.1.1 Scientific Purpose

Scientific Processing Profiles define reproducible scientific workflows
for applying one or more Scientific Working Methods to a defined
scientific processing task.

A Scientific Processing Profile specifies the scientific workflow,
including the execution sequence, method invocation rules, execution
constraints, completion conditions, and failure handling for applying
Scientific Working Methods to produce scientifically reproducible
execution results.

#### 7.1.2 Architectural Role

Scientific Processing Profiles form the workflow layer of the GM
Execution.

They SHALL:

-   define reproducible scientific processing sequences;
-   select and combine applicable Scientific Working Methods;
-   define the scientific processing scope;
-   define execution-specific processing decisions;
-   define the expected execution result.

They SHALL NOT redefine or weaken the normative requirements of the
referenced Scientific Working Methods.

#### 7.1.3 Relationship to Scientific Working Methods

Scientific Processing Profiles SHALL apply one or more Scientific
Working Methods defined in Chapter 6.

Scientific Working Methods define how scientific work is performed.

Scientific Processing Profiles define when and for which scientific
purpose those methods are applied.

#### 7.1.4 Relationship to Processing Profile Catalogue

Concrete Processing Profiles defined in Chapter 8 SHALL conform to the
requirements of this chapter.

Chapter 7 defines the common Scientific Processing Profile architecture.

Chapter 8 defines Scientific Processing Profile configuration and
boundaries.

### 7.2 Workflow Principles

#### 7.2.1 Purpose

Workflow Principles define the common workflow requirements inherited by
all Scientific Processing Profiles.

Concrete Processing Profiles SHALL inherit these principles unless
explicitly strengthened.

#### 7.2.2 Workflow Principle

Scientific Processing Profiles SHALL transform valid scientific input
into a validated Register Revision through a controlled scientific
workflow.

The workflow SHALL remain non-destructive.

No workflow stage SHALL silently modify the scientific meaning of the
input.

#### 7.2.3 Processing Sequence

Scientific Processing Profiles SHALL apply a controlled processing
sequence.

The sequence MAY be refined by a concrete Processing Profile.

Mandatory workflow stages SHALL NOT be omitted.

#### 7.2.4 Stage Responsibility

Each workflow stage SHALL possess one clearly defined scientific
responsibility.

A workflow stage SHALL NOT redefine the Scientific Working Methods
inherited from Chapter 6.

#### 7.2.5 Progressive Processing

Workflow stages SHALL be performed in an order that preserves scientific
traceability.

A subsequent stage MAY depend on the validated result of a preceding
stage.

#### 7.2.6 Workflow Completion

A Scientific Processing Profile is complete when all mandatory workflow
stages have established one new valid Register Revision representing the
current authoritative working state of the AGRAR in accordance with the
inherited AWE requirements.

Subsequent Scientific Processing Profiles SHALL continue from that
Register Revision.

Subsequent processing belongs to the applicable GM Execution.

### 7.3 Execution-specific Scientific Processing Profiles

This Execution SHALL define one or more Scientific Processing Profiles
specifying the controlled scientific application of the Scientific
Working Methods defined in Chapter 6.

Each Scientific Processing Profile SHALL define:

-   the applicable Scientific Working Methods;
-   the processing sequence;
-   workflow stages and stage transitions;
-   validation stages;
-   failure handling;
-   completion criteria;
-   the Controlled AGRAR Update.

Scientific Processing Profiles SHALL reference Scientific Working
Methods without redefining their scientific responsibilities.

Scientific Processing Profiles SHALL reference inherited Scientific
Artifact and Relationship types without redefining their semantics.

Project-specific Scientific Processing Profiles MAY refine the execution
sequence provided that they remain conformant with this Execution,
GM-Core, GSL, and the referenced Scientific Working Methods.

## 8. Scientific Processing Profile Configuration

### 8.1 Purpose

A Scientific Processing Profile SHALL define an execution configuration
for a specific execution situation without changing the Execution
Contract.

### 8.2 Reference Processing Profile

This Execution SHOULD provide one reference Scientific Processing
Profile illustrating a conformant application of the Scientific Working
Methods and profile architecture defined by this Execution.

The reference profile is provided in Appendix A.

Projects MAY define project-specific Scientific Processing Profiles
where required.

Project-specific profiles SHALL conform to this Execution, GM-Core, GSL,
and the applicable Scientific Working Methods.

### 8.3 Processing Profile Boundary

A Scientific Processing Profile SHALL define the method-specific rules
for applying the Scientific Working Methods of this Execution.

The Execution Contract SHALL define the scientific stages and result
requirements.

GM-Core SHALL define inherited Scientific Artifact, Relationship, AGRAR,
RegisterEntry, and Register Revision semantics and structures.

This Execution SHALL define only applicable additional construction,
representation, workflow, and validation requirements.

A Scientific Processing Profile SHALL NOT alter the scientific meaning
of inherited Scientific Artifact types, Relationship types, or AGRAR
concepts.

### 8.4 Profile Boundary

A Scientific Processing Profile MAY configure execution-specific
scientific processing behavior.

It SHALL NOT introduce responsibilities belonging to another Execution.

------------------------------------------------------------------------

## 9. Validation

### 9.1 Validation Goal

Validation SHALL determine whether the scientific processing result
satisfies the applicable Scientific Processing Profile and the inherited
scientific requirements.

Successful validation SHALL permit the subsequent Controlled AGRAR
Update.

Failed validation SHALL prevent establishment of a new Register
Revision.

### 9.2 Validation Areas

Validation rules SHALL address:

-   source traceability;
-   locator completeness;
-   preservation of uncertainty;
-   absence of silent completion;
-   conformity with the selected Processing Profile;
-   conformity with the applicable inherited and project-level
    Scientific Artifact type descriptions;
-   scientific consistency of the constructed Artifacts and
    Relationships;
-   conformity with the applicable GM-Core structures;
-   scientific reproducibility of the execution result;
-   conformity with the defined scientific boundary.

### 9.3 Invalid Results

An invalid or incomplete result SHALL NOT be silently converted into a
valid persistent scientific result.

The handling of incomplete or rejected processing results SHALL follow
Section 4.8 and the applicable execution-specific Scientific Processing
Profile.

------------------------------------------------------------------------

## 10. Controlled AGRAR Update

### 10.1 Controlled AGRAR Update

The Execution SHALL incorporate the validated source-registration result
into AGRAR through a controlled scientific update.

The `RegisteredSource` incorporated into AGRAR SHALL be represented
through a `RegisterEntry` according to GM-Core.

This Execution SHALL NOT establish Relationships as part of the
Controlled AGRAR Update.

Only validated scientific results SHALL be incorporated.

Each successful update SHALL establish one new valid Register Revision.

### 10.2 Current Valid Register Revision

Each successful Controlled AGRAR Update SHALL establish one new valid
Register Revision.

The resulting revision SHALL become the current authoritative working
state of the AGRAR in accordance with the inherited AWE requirements.

Earlier Register Revisions SHALL remain reproducible according to the
applicable GSL and GM-Core requirements.

### 10.3 Project Type Description

Inherited GM-Core Artifact Types, Relationship Types, and AGRAR concepts
SHALL NOT be re-described as execution-specific types.

Where this Execution or the genealogy project defines additional
source-classification, construction, or representation descriptions
required for reproducible source registration, the applicable project
state SHALL preserve those descriptions.

Where a compatible project-level description already exists, the
Execution SHALL reuse it.

------------------------------------------------------------------------

## 11. Execution Conformance

A conforming implementation of this Execution SHALL:

-   accept only defined and scientifically assessable input;
-   preserve the scientific identity and provenance of the Scientific
    Source and its Source Representations;
-   perform only the source-registration scientific responsibility
    defined by this Execution;
-   establish or reuse `RegisteredSource` in conformance with GM-Core;
-   represent AGRAR membership through `RegisterEntry`;
-   establish no Relationships as part of the source-registration
    result;
-   preserve explicit uncertainty and source traceability;
-   validate the registration result before Controlled AGRAR Update;
-   establish one new valid Register Revision for each successful
    Controlled AGRAR Update;
-   avoid horizontal inheritance from another Execution;
-   avoid hidden dependencies on execution-internal workflow state;
-   avoid redefining GM-Core Scientific Artifact, Relationship, AGRAR,
    RegisterEntry, or Register Revision semantics.

## Appendix A --- Reference Processing Profiles

### A.1 Purpose

This Appendix is non-normative.

It provides one or more reference Processing Profiles illustrating
conforming implementations of this Execution.

### A.2 Reference Processing Profiles

#### Profile Name

Reference Source Registration Profile

#### Scientific Purpose

Provide one complete reference implementation of the GM-Exec Source
Registration by applying the Scientific Working Methods defined by this
Execution in a reproducible scientific workflow.

The profile demonstrates one conforming implementation of this
Execution.

It does not introduce additional scientific responsibilities or modify
the normative requirements defined by this Execution.

#### Applicability

This Reference Processing Profile applies where one Scientific Source is
to be scientifically registered from one or more Source Representations.

The Source Representations SHALL satisfy the scientific preconditions
defined by this Execution.

This Reference Processing Profile SHALL produce exactly one Registered
Source Artifact representing one Scientific Source.

The profile SHALL preserve:

-   scientific identity;
-   scientific provenance;
-   scientific traceability;
-   uniqueness of the `RegisteredSource`.

The profile SHALL NOT perform scientific tasks assigned to another GM
Execution.

The profile SHALL NOT establish Relationships.

#### Execution Input

The Reference Processing Profile receives:

-   one or more Source Representations;
-   access to the current valid Register Revision, unless the initial
    revision is established by this Execution;
-   the applicable project-retained Source Type Descriptions;
-   the Scientific Working Methods defined by this Execution.

The input SHALL satisfy the scientific preconditions defined in Section
2.4 before scientific processing begins.

No additional execution-specific input is required by this Reference
Processing Profile.

#### Scientific Working Methods

The Reference Processing Profile applies the following Scientific
Working Methods:

1.  Source Representation Assessment
2.  Scientific Source Identification
3.  Scientific Source Classification
4.  Source Registration Decision
5.  `RegisteredSource` Construction
6.  Registration Validation

#### Processing Sequence

The Reference Processing Profile applies the Scientific Working Methods
in the following sequence:

1.  Source Representation Assessment

    Determine whether the available Source Representations are
    scientifically sufficient for source registration.

2.  Scientific Source Identification

    Identify the Scientific Source represented by the accepted Source
    Representations.

3.  Scientific Source Classification

    Classify the identified Scientific Source according to the
    applicable project-retained Source Type Descriptions.

4.  Source Registration Decision

    Determine whether the Scientific Source requires establishment of a
    new `RegisteredSource` or reuse of an existing `RegisteredSource`
    Artifact.

5.  `RegisteredSource` Construction

    Establish or update the `RegisteredSource` according to the Source
    Registration Decision.

6.  Registration Validation

    Validate the resulting `RegisteredSource` before Controlled AGRAR
    Update.
