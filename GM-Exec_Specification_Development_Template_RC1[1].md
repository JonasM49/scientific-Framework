
# GM-Exec Specification Development Template

**Document type:** Authoritative Release Candidate (RC1)
**Version:** v0.1
**Status:** Authoritative Working Draft
**Architecture level:** GM Execution  
**Normative foundation:** General Scientific Layer (GSL) and GC Core  

**AUTHOR** JonasM49

**PUBLISHED_AT** 2026-07-15

**CANONICAL_REPOSITORY** https://github.com/JonasM49/scientific-Framework

**LICENSE** CC BY-NC-SA 4.0

---

## 0. Document Status

This document is the initial **Authoritative Working Draft (AWD v0.4)**
of the GM-Exec Specification Development Template.

The template is an editorial development aid for creating consistent
GM Execution Specifications.

It is not part of the normative dependency hierarchy.

Execution Specifications developed from this template SHALL inherit only
from GSL and GC Core.

The objective of this AWD is to guide the consistent development of
valid GM Execution Specifications while preserving the validated
architectural structure.

### 0.1 Template Editing Convention

Template placeholders use the following syntax:

    {TYPE Subject LIKE Editorial guidance}

Where:

- TYPE defines the expected form of the replacement
  (for example: DEFINITION, DESCRIPTION, LIST, RULE, STRUCTURE).

- Subject identifies the execution-specific element to be replaced.

- LIKE provides editorial guidance describing the required purpose,
  structure, or an exemplary specialization of the replacement.

The LIKE clause is editorial only.

All placeholders SHALL be replaced before an Execution Specification
reaches Release Candidate status.


## 1. Purpose and Scope

### 1.1 Purpose

This Execution shall perform one clearly defined

{DEFINITION Execution-specific scientific task
 LIKE define the named scientific task of the Execution}.

{DESCRIPTION Execution-specific scientific task description
 LIKE define the scientific input, the controlled scientific processing,
 the resulting scientific artifact or state, and the execution-specific
 scientific boundary}.

### 1.2 Scientific Task

The single scientific task of this Execution is:

{DESCRIPTION Execution-specific scientific task
 LIKE define the single scientific task performed by this Execution,
 including its scientific objective and intended result.}

The Execution shall preserve the distinction between:

{LIST Execution-specific scientific boundary elements
 LIKE define the scientific elements that SHALL remain explicitly
 distinguishable throughout this Execution.}

### 1.3 Scope

{LIST Execution-specific scope
 LIKE define the scientific responsibilities performed by this
 Execution, including required processing activities, resulting
 artifacts, validation responsibilities, and Controlled GSRAR Update.}

### 1.4 Out of Scope

This Execution shall define only the scientific responsibilities
assigned to its execution-specific scientific task.

{LIST Execution-specific out-of-scope responsibilities
 LIKE define all scientific responsibilities that intentionally remain
 outside the scope of this Execution because they belong to another
 GM Execution or exceed the defined scientific boundary.}


### 1.5 Non-Destructive Principle

This Execution shall not modify the Registered Source Artifact used as input.

Corrections, extensions, or alternative readings shall be represented through new or revised execution results according to the applicable GSL and GC Core rules.

---

### 1.6 Scientific Result Completeness Principle

{RULE Execution-specific completion condition
 LIKE define which scientific results SHALL be present before the
 Execution may complete successfully}.

The completion criterion shall be the scientific completeness of the
execution-specific result rather than the completion of a particular
Scientific Working Method.

## 2. Normative Foundation

### 2.1 General Scientific Layer

This Execution shall conform to the applicable scientific principles, integrity requirements, traceability requirements, and lifecycle rules defined by the GSL.

### 2.2 GC Core

This Execution shall use the artifact, relationship, register, and project structures defined by GC Core.

Core structures shall be referenced and applied. They shall not be redefined in this Execution.

### 2.3 Normative Inheritance

The normative inheritance shall be:

```text
{DEFINITION Execution specification name
 LIKE define the name of the concrete GM Execution}
    INHERITS GC Core
    INHERITS GSL
```

This Execution shall not inherit from another GM Execution.

No horizontal inheritance between Executions is permitted.

---

### 2.4 Scientific Preconditions

Before execution begins, the following scientific preconditions shall be
satisfied:

{LIST Execution-specific scientific preconditions
 LIKE define the required processing scope, availability and validity of
 the scientific input, suitability of the selected Scientific Working
 Methods, and any required conditions for method escalation}.

### 2.5 Method Selection Preconditions

{STRUCTURE Execution-specific Scientific Working Method structure
 LIKE define the applicable Scientific Working Methods and any
 relationships, sequence, refinement, or escalation between them}.

The following principles apply:

{LIST Execution-specific method selection principles
 LIKE define how the applicable methods contribute to the scientific
 result, when refinement or escalation is permitted, and which
 scientifically sufficient result the methods SHALL achieve}.


## 3. Execution Architecture

### 3.1 Execution Unit

This document specifies one independent GM Execution.

The Execution shall be usable without inheritance from, embedding of, or direct control by another GM Execution.

### 3.2 Pipe Model

The normative execution pipe shall be:

```text
1. Execution Input
    {DEFINITION Execution-specific input artifact
     LIKE define the scientific input accepted by this Execution}

2. Execution
    {DEFINITION Execution-specific scientific task
     LIKE define the named scientific task of the Execution}

3. Execution Result
    {DESCRIPTION Execution-specific execution result
     LIKE define the validated scientific result produced before the
     Controlled GSRAR Update}

    One new valid GSRAR Revision
        established through Controlled GSRAR Update
```

Successful completion of this Execution performs the Controlled GSRAR Update and establishes one new valid GSRAR Revision.

### 3.3 Pipe Boundary

This Execution performs the controlled scientific processing and incorporates validated

{DEFINITION Execution-specific scientific artifact
 LIKE define the persistent scientific artifact produced by this Execution}

together with

{LIST Execution-specific required result relationships
 LIKE define the Relationships required to represent the scientific
 result produced by this Execution}

into the GSRAR.

Successful completion establishes one new valid GSRAR Revision representing the current scientific working state.

No GSRAR modification shall be implied merely by successful completion of execution-specific scientific processing.

### 3.4 Execution Independence

A consuming Execution shall not require knowledge of:

{LIST Execution-specific internal working information
 LIKE define temporary execution-specific working information that SHALL remain internal}.

A consuming Execution shall rely on:

- the shared GC Core structure;
- {DEFINITION Execution-specific artifact type description
   LIKE define the project-retained dataset description of the
   execution-specific result artifact};
- registered

  {DEFINITION Execution-specific scientific artifacts
   LIKE define the persistent scientific artifacts produced by this
   Execution}

  and their valid Relationships.

### 3.5 No Horizontal Inheritance

This Execution shall not inherit structure, behavior, or authority from another GM Execution.

A subsequent Execution shall not inherit from this Execution.

Compatibility between Executions shall be established through shared Core structures, project-retained type descriptions, and explicit input/output contracts.

### 3.6 No Hidden State Transfer

Only

{LIST Execution-specific transferable scientific results
 LIKE define which execution results may be transferred through the execution boundary}

may pass through the pipe.

A subsequent Execution shall not depend on undocumented internal state.

---

## 4. Execution Contract

### 4.1 Required Input

A conforming execution instance shall receive:

{DESCRIPTION Execution-specific required input
 LIKE define all mandatory scientific input required to perform this
 Execution, including required artifacts, references,
 representations, and scientific preconditions.}

### 4.2 Conditional Input

Where required by the selected method or Processing Profile, the execution instance may additionally receive:

{LIST Execution-specific optional input
 LIKE define all optional scientific input, parameters,
 profiles, references, navigation information, or supporting
 material accepted by this Execution.}

Conditional input shall not silently alter the scientific meaning of the execution input.

### 4.3 Input Validity

{DESCRIPTION Execution-specific input validity rules
 LIKE define the conditions under which execution input SHALL
 be accepted, rejected, or considered incomplete.}

An execution instance shall not compensate for invalid input
by inventing scientific evidence.

### 4.4 Required Output

{DESCRIPTION Execution-specific required output
 LIKE define the validated scientific result produced by this
 Execution, including required artifacts, Relationships,
 validation information, provenance, and resulting
 GSRAR state.}

Validated results SHALL be incorporated into the GSRAR through the Controlled GSRAR Update defined by this Execution.

The resulting GSRAR Revision SHALL constitute the current valid scientific working state.

### 4.5 Artifact Type Description Output

{RULE Execution-specific artifact type description
 LIKE define how the project-retained dataset description of
 the execution-specific result artifact SHALL be established,
 reused, or extended.}

### 4.6 Output State

The output of this Execution is one new valid GSRAR Revision established through the Controlled GSRAR Update.

The resulting GSRAR Revision SHALL constitute the current valid scientific working state in accordance with this Execution.

### 4.7 Prohibited Output

This Execution shall not produce scientific results that are assigned
to another GM Execution.

{LIST Execution-specific prohibited output
 LIKE define scientific results that SHALL NOT be produced by this
 Execution because they belong to another GM Execution or violate the
 defined scientific scope.}


### 4.8 Failure Output

Where successful execution-specific scientific artifact generation is not possible, the Execution may produce a documented incomplete or rejected processing result.

Such a processing result shall not be represented as a valid execution-specific scientific artifact unless it satisfies the applicable artifact contract.

---

## 5. Execution-specific Scientific Artifact

### 5.1 Scientific Role

{DESCRIPTION Execution-specific scientific artifact
 LIKE define the scientific role, purpose, and scope of the primary
 scientific artifact produced by this Execution.}

### 5.2 Core Basis

The execution-specific scientific artifact type shall use the common scientific artifact structure defined by GC Core.

This Execution shall define only the execution-specific dataset description required for its scientific artifact.

The common Core structure shall not be redefined.

### 5.3 Persistent Artifact Identity

Each execution-specific scientific artifact shall possess a persistent artifact identity according to GC Core.

The artifact identity shall remain independent of:

- the identity of the producing tool;
- the temporary execution workspace;
- the later artifacts derived from the scientific artifact;
- the Execution that subsequently processes the scientific artifact.

### 5.4 Artifact Relationships

{RULE Execution-specific artifact relationships
 LIKE define the Relationships required to represent the scientific
 meaning, provenance, and context of the execution-specific
 scientific artifact.}

### 5.5 Artifact Independence

{RULE Execution-specific artifact independence
 LIKE define the information required by subsequent Executions to
 process the execution-specific scientific artifact without relying on
 undocumented internal execution state.}

### 5.6 Scientific Boundary

{RULE Execution-specific scientific boundary
 LIKE define which scientific transformations SHALL NOT silently replace
 the scientific evidence represented by this Execution.}

### 5.7 Uncertainty Representation

{RULE Execution-specific uncertainty representation
 LIKE define how execution-specific scientific uncertainty SHALL be
 represented and preserved.}

### 5.8 Artifact Dataset Description

{DESCRIPTION Execution-specific artifact dataset description
 LIKE define the project-retained dataset description required for the
 execution-specific scientific artifact, including semantics,
 validation, Relationships, and compatibility requirements.}

### 5.9 Derived Scientific Artifacts

{RULE Execution-specific derived scientific artifacts
 LIKE define how subsequent Executions may derive additional scientific
 artifacts from the execution-specific scientific artifact.}


## 6. Scientific Working Methods

### 6.1 Purpose

#### 6.1.1 Scientific Purpose

The purpose of the Scientific Working Methods is to define the scientific methods and working aids that MAY be used by GM Executions to produce scientifically reproducible results.

Scientific Working Methods define how scientific work is performed.

They SHALL NOT define:

- execution workflows;
- processing sequences;
- artifact generation;
- register modification procedures;
- project-specific Processing Profiles.

These responsibilities belong to subsequent chapters of the GM Execution.

#### 6.1.2 Architectural Role

Scientific Working Methods form the methodological layer of the GM Execution.

They provide reusable scientific methods that MAY be referenced by one or more Scientific Processing Profiles.

A Scientific Working Method SHALL be applicable independently of a specific Processing Profile.

#### 6.1.3 Scientific Independence

A Scientific Working Method defines a scientific method only.

It SHALL NOT prescribe:

- when a method is selected;
- the order in which methods are applied;
- the scientific scope of an Execution;
- the resulting scientific artifacts.

These decisions belong to the applicable Scientific Processing Profile.

#### 6.1.4 Relationship to Scientific Processing Profiles

Scientific Processing Profiles SHALL apply one or more Scientific Working Methods.

A Processing Profile MAY refine the application of a method for a specific scientific task.

It SHALL NOT redefine or weaken the normative requirements of the referenced Scientific Working Method.

### 6.2 Scientific Working Principles

#### 6.2.1 Purpose
Scientific Working Principles define the common scientific principles that SHALL apply to all Scientific Working Methods defined by this Execution.

Concrete methods SHALL inherit these principles unless explicitly strengthened.

#### 6.2.2 Scientific Method Principle

Scientific Working Methods SHALL define reproducible scientific procedures
for achieving their assigned scientific purpose.

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
A Scientific Working Method SHALL achieve scientifically sufficient quality for the defined processing scope.

The objective SHALL NOT be maximum detail but scientifically sufficient reproducibility.

#### 6.2.5 Method Escalation
A more detailed Scientific Working Method SHOULD be applied only where the preceding method cannot achieve scientifically sufficient quality.

Methods SHALL form a progressive scientific refinement.

#### 6.2.6 Working Representations

Scientific Working Methods MAY construct temporary scientific Working Representations to support the scientific method.

Such Working Representations SHALL NOT constitute persistent scientific artifacts unless explicitly specified by the applicable Scientific Processing Profile.

#### 6.2.7 Method Completion
A Scientific Working Method is complete when it has achieved scientifically sufficient results for the defined processing scope.

Subsequent processing belongs to the applicable Scientific Processing Profile.

### 6.3 Execution-specific Scientific Working Methods

{DESCRIPTION Execution-specific Scientific Working Methods
 LIKE define all Scientific Working Methods required by this Execution,
 including their scientific purpose, applicability, inheritance,
 refinement hierarchy, normative requirements, and completion criteria.}


## 7. Scientific Processing Profiles

### 7.1 Purpose

#### 7.1.1 Scientific Purpose

Scientific Processing Profiles define reproducible scientific workflows for applying one or more Scientific Working Methods to a defined scientific processing task.

A Scientific Processing Profile specifies how Scientific Working Methods are combined to produce scientifically reproducible execution results.

#### 7.1.2 Architectural Role

Scientific Processing Profiles form the workflow layer of the GM Execution.

They SHALL:

- define reproducible scientific processing sequences;
- select and combine applicable Scientific Working Methods;
- define the scientific processing scope;
- define execution-specific processing decisions;
- define the expected execution result.

They SHALL NOT redefine or weaken the normative requirements of the referenced Scientific Working Methods.

#### 7.1.3 Relationship to Scientific Working Methods

Scientific Processing Profiles SHALL apply one or more Scientific Working Methods defined in Chapter 6.

Scientific Working Methods define how scientific work is performed.

Scientific Processing Profiles define when and for which scientific purpose those methods are applied.

#### 7.1.4 Relationship to Processing Profile Catalogue

Concrete Processing Profiles defined in Chapter 8 SHALL conform to the requirements of this chapter.

Chapter 7 defines the common workflow architecture.

Chapter 8 defines concrete profile implementations.

### 7.2 Workflow Principles

#### 7.2.1 Purpose

Workflow Principles define the common workflow requirements inherited by all Scientific Processing Profiles.

Concrete Processing Profiles SHALL inherit these principles unless explicitly strengthened.

#### 7.2.2 Workflow Principle

Scientific Processing Profiles SHALL transform valid scientific input into a validated GSRAR Revision through a controlled scientific workflow.

The workflow SHALL remain non-destructive.

No workflow stage SHALL silently modify the scientific meaning of the input.

#### 7.2.3 Processing Sequence

Scientific Processing Profiles SHALL apply a controlled processing sequence.

The sequence MAY be refined by a concrete Processing Profile.

Mandatory workflow stages SHALL NOT be omitted.

#### 7.2.4 Stage Responsibility

Each workflow stage SHALL possess one clearly defined scientific responsibility.

A workflow stage SHALL NOT redefine the Scientific Working Methods inherited from Chapter 6.

#### 7.2.5 Progressive Processing

Workflow stages SHALL be performed in an order that preserves scientific traceability.

A subsequent stage MAY depend on the validated result of a preceding stage.

#### 7.2.6 Workflow Completion

A Scientific Processing Profile is complete when all mandatory workflow stages have established one new valid GSRAR Revision representing the current valid scientific working state.

Subsequent Scientific Processing Profiles SHALL continue from that GSRAR Revision.

Subsequent processing belongs to the applicable GM Execution.

### 7.3 Execution-specific Scientific Processing Profiles

{DESCRIPTION Execution-specific Scientific Processing Profiles
 LIKE define the complete execution-specific workflow, including
 processing stages, validation stages, Controlled GSRAR Update,
 failure handling, completion criteria, and any execution-specific
 workflow architecture.}


## 8. Processing Profiles

### 8.1 Purpose

A Scientific Processing Profile shall define an execution configuration for a specific execution situation without changing the execution-specific scientific artifact contract unnecessarily.

### 8.2 Reference Processing Profile

Each GM Execution SHOULD provide one reference Processing Profile.

The reference Processing Profile illustrates a conformant application of
the Scientific Working Methods defined in Chapter 6 and the Scientific
Processing Profile architecture defined in Chapter 7.

It serves as a specification template for project-specific Scientific Processing
Profiles.

Projects MAY define their own Scientific Processing Profiles according
to their scientific requirements.

Project-specific Processing Profiles SHALL conform to the requirements
of this chapter and the applicable Scientific Working Methods.

The reference Processing Profile is provided in Appendix A.

### 8.3 Processing Profile Boundary

The Scientific Processing Profile shall define the method-specific rules for applying the execution-specific Scientific Working Methods.

The Execution contract shall define the scientific stages and result requirements.

The execution-specific scientific artifact dataset description shall define the representation of the resulting scientific artifact.

Accordingly:

- the Execution defines the scientific task;
- the Processing Profile defines the applied method;
- the dataset description defines the persistent result structure.

A Scientific Processing Profile shall not alter the scientific meaning of the execution-specific scientific artifact type.


### 8.4 Profile Boundary

A Scientific Processing Profile may configure execution-specific scientific processing behavior.

It shall not introduce responsibilities belonging to another Execution.

---

## 9. Validation

### 9.1 Validation Goal

Validation SHALL determine whether the scientific processing result satisfies the applicable Scientific Processing Profile and the inherited scientific requirements.

Successful validation SHALL permit the subsequent Controlled GSRAR Update.

Failed validation SHALL prevent establishment of a new GSRAR Revision.

### 9.2 Validation Areas

Validation rules shall address:

- source traceability;
- locator completeness;
- preservation of uncertainty;
- absence of silent completion;
- conformity with the selected Processing Profile;
- conformity with the execution-specific scientific artifact type description;
- scientific consistency of the constructed Artifacts and Relationships;
- conformity with the applicable GM Core structures;
- scientific reproducibility of the execution result;
- conformity with the defined scientific boundary.

### 9.3 Invalid Results

An invalid or incomplete result shall not be silently converted into a valid execution-specific scientific artifact.

The handling of incomplete or rejected processing results SHALL follow Section 4.8 and the applicable execution-specific Scientific Processing Profile.

---

## 10. Controlled GSRAR Update

### 10.1 Controlled GSRAR Update

The Execution SHALL incorporate validated execution-specific scientific artifacts together with their required Relationships into the GSRAR through a controlled scientific update.

Only validated scientific results SHALL be incorporated.

Each successful update SHALL establish one new valid GSRAR Revision.

### 10.2 Current Valid GSRAR Revision

Each successful Controlled GSRAR Update SHALL establish one new valid GSRAR Revision.

The resulting revision SHALL constitute the current valid scientific working state of the project.

Earlier GSRAR Revisions SHALL remain reproducible according to the applicable GSL and GM Core requirements.

### 10.3 Project Type Description

Where the execution-specific scientific artifact type description is not yet available in the project, the resulting GSRAR Revision shall provide the complete description required for its project-level retention.

Where the description already exists, the Execution shall use a compatible structure.

---

## 11. Execution Conformance

A conforming implementation of this Execution shall:

- accept only defined input structures;
- preserve the registered source artifact;
- perform the execution-specific scientific task within the defined scientific boundary;
- produce execution-specific scientific artifacts conforming to the project-retained dataset description;
- produce and transfer the required execution-specific Relationships with every execution result;
- preserve explicit uncertainty;
- provide source traceability;
- validate its output before Controlled GSRAR Update;
- avoid horizontal inheritance from another Execution;
- avoid hidden dependencies on internal workflow state.


---

## Appendix A — Reference Processing Profiles

### A.1 Purpose

This Appendix is non-normative.

It provides one or more reference Processing Profiles illustrating
conforming implementations of this Execution.

### A.2 Reference Processing Profiles

{DESCRIPTION Execution-specific reference Processing Profiles
 LIKE provide one or more complete reference Processing Profiles
 illustrating conforming implementations of this Execution,
 including scientific purpose, applicability, processing scope,
 profile-specific rules, applied Scientific Working Methods,
 and expected scientific results.}
