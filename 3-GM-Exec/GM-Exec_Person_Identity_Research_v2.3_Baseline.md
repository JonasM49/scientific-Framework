# GM-Exec Person Identity Research

STATUS: Baseline

VERSION: 2.3

DOCUMENT_IDENTIFIER: GM-Exec_Person_Identity_Research

ARCHITECTURE_LEVEL: GM Execution

DOCUMENT_TYPE: NormativeSpecification

DEPENDS_ON: GSL-2.0, GM-Core-v1.3

LANGUAGE: DSL SPECIFICATION_LINEAGE

AUTHOR: JonasM49

PUBLISHED_AT: 2026-09-19

CANONICAL_REPOSITORY: https://github.com/JonasM49/scientific-Framework

LICENSE: CC-BY-NC-SA-4.0

---

## 0. Document Status

This document is the **Baseline v2.3** of the GM-Exec Person Identity Research.

This AWD is developed from the GM-Exec Specification Development Template
Baseline v1.1.

It is not part of the normative dependency hierarchy.

This Execution SHALL inherit only from GSL and GM Core.

The objective of this Baseline is to define the GM Execution for
scientific person identity research while preserving the validated
GM-Exec architectural structure.

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



### 0.2 Execution Architecture Consolidation Principles

The following principles guide the development and consolidation of GM
Execution Specifications.

These principles are informative. They support the production of
consistent, non-redundant, and maintainable Execution Specifications.

They do not introduce additional scientific requirements.

#### K1 – Single Point of Scientific Definition

Each scientific property of a scientific object SHOULD be defined
normatively only once within an Execution Specification.

#### K2 – Single Point of Scientific Responsibility

Each Scientific Working Method SHOULD define exactly one scientific
responsibility.

#### K3 – Single Point of Scientific Lifecycle

Each scientific lifecycle stage SHOULD be specified only once.
Subsequent stages SHOULD reference, rather than redefine, preceding
stages.

#### K4 – Reference Profile as Architectural Validation

The Reference Processing Profile SHOULD be used to verify that every
normative requirement is represented exactly once and that no additional
scientific rules are introduced by the Appendix.

#### K5 – Architectural Layer Separation

Each chapter SHOULD define only its assigned architectural layer and
SHOULD NOT redefine responsibilities assigned to other chapters.

#### K6 – Contract Minimality

Execution Contracts SHOULD define only execution input, execution output
and contractual obligations. Scientific behavior belongs to later
chapters.

#### K7 – Artifact-Centric Definition

Scientific properties of execution-specific artifacts SHOULD be defined
only in the artifact chapter. Other chapters SHOULD reference those
definitions.

#### K8 – Method Minimality

Scientific Working Methods SHOULD define only the scientific
transformation performed by the method. They SHOULD NOT redefine
artifact properties, workflow rules or execution contracts.

#### K9 – Workflow Minimality

Scientific Processing Profiles SHOULD define only the orchestration of
Scientific Working Methods. They SHOULD reference, rather than redefine,
methods, artifacts and contracts.


### 0.3 Execution Specification Structure

The GM Execution Specification Template is divided into three editorial
parts.

#### Part I — Execution Development

Chapters 1 through 7 define the execution-specific scientific
specification.

These chapters contain editorial placeholders and SHALL be completed for
each concrete GM Execution.

Development and scientific consolidation primarily take place in this
part of the template.

#### Part II — Framework Stable Architecture

Chapters 8 through 11 define the stable GM Execution Framework.

These chapters normally require only editorial review for consistency,
terminology, chapter responsibility, and architectural conformance.

They SHOULD NOT be modified unless an improvement affects the GM
Execution Framework itself.

#### Part III — Reference Processing Profiles

Appendix A contains the execution-specific Reference Processing
Profiles.

These profiles illustrate conforming applications of the normative
execution architecture and SHALL be completed for each concrete GM
Execution.


## 1. Purpose and Scope

### 1.1 Purpose

This Execution shall perform one clearly defined scientific task:

scientific person identity research.

This Execution shall evaluate Scientific Observation Artifacts referring
to one research focus person, determine whether the scientific evidence
supports association with an existing Person Identity Artifact or the
creation of a new Person Identity Artifact, construct the corresponding
Event Artifacts and required Relationships, and incorporate the validated
scientific result into the GSRAR.

### 1.2 Scientific Task

The single scientific task of this Execution is:

the scientific identification or construction of one Person Identity
from Scientific Observation Artifacts concerning one research focus
person, together with the directly supported Event Artifacts and required
Relationships.

The research focus person is the execution-specific Focus Person and SHALL be
interpreted within the inherited GM Core Research Focus semantics.

The Execution shall preserve the distinction between:

- Scientific Observation Artifacts;
- the research focus person;
- Person Identity Artifacts;
- Event Artifacts;
- Relationships;
- open research points concerning persons outside the current research focus.

### 1.3 Scope

This Execution shall:
- evaluate Scientific Observation Artifacts relating to one research focus person;
- establish an Assessment Scope containing the scientific material admitted to the current person identity assessment;
- use the applicable current Relationship State and inherited Scientific Cluster where structural investigation is scientifically justified;
- compare the admitted scientific evidence with existing or candidate Person Identity Artifacts contained in the current valid GSRAR Revision;
- evaluate Information Artifacts and event-related evidence independently from person identity;
- determine whether existing scientific Artifacts and applicable inherited ObservationReferenceRelationship or EvidenceSupportRelationship semantics sufficiently represent the available scientific evidence;
- construct new Person Identity Artifacts, Information Artifacts, Event Artifacts, and Relationships where scientifically justified;
- establish the applicable inherited observation/evidence Relationships connecting supporting Scientific Observation Artifacts with the corresponding scientific Artifacts;
- preserve unresolved scientific uncertainty and open research points explicitly;
- validate the resulting scientific Artifacts and Relationships;
- perform the Controlled GSRAR Update.

### 1.4 Out of Scope

This Execution shall define only the scientific responsibilities
assigned to its execution-specific scientific task.

- scientific transcription of source material;
- scientific source registration;
- recursive processing of persons outside the current research focus;
- family reconstruction;
- kinship reconstruction extending beyond the directly supported evidence;
- search for potential parents, spouses, children, or other relatives beyond the current research focus;
- construction of Family Artifacts;
- resolution of competing family hypotheses;
- publication-specific representation, including report generation;
- project-specific research strategies extending beyond the defined scientific boundary.

### 1.5 Non-Destructive Principle

This Execution shall not modify the Registered Source Artifact used as input.

Corrections, extensions, or alternative readings shall be represented through new or revised execution results according to the applicable GSL and GM Core rules.

---

### 1.6 Scientific Result Completeness Principle

The Execution shall complete successfully when the scientific evidence relating to the current research focus person has been scientifically evaluated, the resulting Person Identity Artifact, Event Artifacts, and required Relationships have been scientifically validated, unresolved scientific uncertainty has been explicitly preserved, and the validated scientific result has been incorporated into the current valid GSRAR Revision.

The completion criterion shall be the scientific completeness of the
execution-specific result rather than the completion of a particular
Scientific Working Method.

Further Scientific Working Method application or investigation expansion
SHALL be required only where the current execution-specific result is not yet
scientifically sufficient and the additional operation can be scientifically
justified as material to the current person identity assessment.

The existence of additional structurally connected material, open research
points, or possible research paths SHALL NOT by itself prevent scientific
completion.

Where a material question cannot be further resolved from scientifically
available evidence, the unresolved state SHALL be preserved explicitly and
MAY constitute a scientifically complete execution result.

## 2. Normative Foundation

### 2.1 General Scientific Layer

This Execution shall conform to the applicable scientific principles, integrity requirements, traceability requirements, and lifecycle rules defined by the GSL.

### 2.2 GM Core

This Execution shall use the artifact, relationship, register, and project structures defined by GM Core.

Core structures shall be referenced and applied. They shall not be redefined in this Execution.

### 2.3 Normative Inheritance

The normative inheritance shall be:

```text
GM-Exec Person Identity Research
    INHERITS GM Core
    INHERITS GSL
```

This Execution shall not inherit from another GM Execution.

No horizontal inheritance between Executions is permitted.

---

### 2.4 Scientific Preconditions

Before execution begins, the following scientific preconditions shall be
satisfied:

- scientific evidence relating to one research focus person is available;
- the available scientific evidence is sufficiently accessible for scientific assessment;
- the applicable Person Identity Research Processing Profile is available;
- the current valid GSRAR Revision is available;
- the required GM Core structures are available.

### 2.5 Method Selection Preconditions

The applicable Scientific Working Methods for this Execution SHALL form
a coherent scientific assessment process.

The execution-specific method architecture SHALL define:

- the applicable Scientific Working Methods;
- their scientific responsibilities;
- permitted refinement relationships;
- permitted execution order where applicable;
- method selection criteria;
- scientific completion criteria.

The concrete Scientific Working Methods SHALL be defined by this
Execution and documented in the corresponding execution-specific method
sections.

The following principles apply:

- the selected Scientific Working Methods SHALL collectively achieve the execution-specific scientific task;
- Scientific Working Methods SHALL be selected according to the available scientific evidence;
- more specialized Scientific Working Methods MAY refine, but SHALL NOT contradict, preceding scientific results;
- only scientifically validated results MAY contribute to the Controlled GSRAR Update;
- unresolved scientific uncertainty SHALL be preserved throughout method selection and execution.


## 3. Execution Architecture

### 3.1 Execution Unit

This document specifies one independent GM Execution.

The Execution shall be usable without inheritance from, embedding of, or direct control by another GM Execution.

### 3.2 Pipe Model

The normative execution pipe shall be:

```text
1. Execution Input
    Scientific Evidence
     relating to one research focus person

2. Execution
    Scientific Person Identity Research

3. Execution Result
    Scientifically validated

        - Person Identity Artifact;
        - Event Artifacts;
        - Relationships

    One new valid GSRAR Revision
        established through Controlled GSRAR Update
```

Successful completion of this Execution performs the Controlled GSRAR Update and establishes one new valid GSRAR Revision.

### 3.3 Pipe Boundary

This Execution performs the controlled scientific processing and incorporates validated

Person Identity Artifacts,
Event Artifacts,
and supporting Relationships

together with

Relationships required to represent:

- scientific identity assignment;
- supported scientific properties;
- supported scientific events;
- scientific provenance;
- supporting scientific evidence.

into the GSRAR.

Successful completion establishes one new valid GSRAR Revision representing the current scientific working state.

No GSRAR modification shall be implied merely by successful completion of execution-specific scientific processing.

### 3.4 Execution Independence

A consuming Execution shall not require knowledge of:

- temporary scientific Working Representations;
- Observation Clusters;
- Person Comparison Workspaces;
- Property and Event Assessment Workspaces;
- temporary candidate artifacts;
- intermediate scientific assessment results.

A consuming Execution shall rely on:

- the shared GM Core structure;
- the project-retained Person Identity Artifact dataset description;
- registered

  Person Identity Artifacts;
  registered Event Artifacts

  and their valid Relationships.

### 3.5 No Horizontal Inheritance

This Execution shall not inherit structure, behavior, or authority from another GM Execution.

A subsequent Execution shall not inherit from this Execution.

Compatibility between Executions shall be established through shared Core structures, project-retained type descriptions, and explicit input/output contracts.

### 3.6 No Hidden State Transfer

Only

- validated Person Identity Artifacts;
- validated Event Artifacts;
- validated Relationships;
- project-retained artifact type descriptions required by this Execution.

may pass through the pipe.

A subsequent Execution shall not depend on undocumented internal state.

---

## 4. Execution Contract

### 4.1 Required Input

A conforming execution instance shall receive:

A conforming execution instance shall receive:

- scientific evidence relating to one research focus person;
- access to the current valid GSRAR Revision;
- the applicable Person Identity Research Processing Profile;
- the project-retained dataset descriptions required by this Execution.

### 4.2 Conditional Input

Where required by the selected method or Processing Profile, the execution instance may additionally receive:

- additional scientific evidence;
- project-specific processing parameters;
- execution-specific navigation information;
- execution-specific supporting material.

Conditional input shall not silently alter the scientific meaning of the execution input.

### 4.3 Input Validity

Execution input SHALL satisfy the following conditions:

- Scientific Evidence SHALL be scientifically accessible;
- the research focus person SHALL be explicitly identified;
- the referenced GSRAR Revision SHALL be valid;
- missing scientific evidence SHALL NOT be invented or silently completed.

An execution instance shall not compensate for invalid input
by inventing scientific evidence.

### 4.4 Required Output

A conforming execution instance shall produce a scientifically validated result consisting of:

- validated Person Identity Artifacts;
- validated Event Artifacts;
- validated Relationships representing the validated scientific result;
- preservation of explicit scientific uncertainty where applicable.

The required execution output SHALL represent the validated scientific result for the current research focus person.

Artifact semantics, scientific validation procedures, and execution-specific scientific behavior are defined by subsequent chapters and SHALL NOT be redefined by this Execution Contract.

Validated results SHALL be incorporated into the GSRAR through the Controlled GSRAR Update defined by this Execution.

The resulting GSRAR Revision SHALL constitute the current valid scientific working state.

### 4.5 Artifact Type Description Output

The project-retained dataset descriptions for Person Identity Artifacts, Event Artifacts, and required Relationships SHALL be established, reused, or extended in accordance with GM Core and the applicable project type descriptions.

### 4.6 Output State

The output of this Execution is one new valid GSRAR Revision established through the Controlled GSRAR Update.

The resulting GSRAR Revision SHALL constitute the current valid scientific working state in accordance with this Execution.

### 4.7 Prohibited Output

This Execution shall not produce scientific results that are assigned
to another GM Execution.

- Family Artifacts;
- publication-specific reports;
- scientific results assigned to another GM Execution;
- undocumented execution-internal Working Representations.


### 4.8 Failure Output

Where successful execution-specific scientific artifact generation is not possible, the Execution may produce a documented incomplete or rejected processing result.

Such a processing result shall not be represented as a valid execution-specific scientific artifact unless it satisfies the applicable artifact contract.

---

## 5. Execution-specific Scientific Artifact

### 5.1 Scientific Role

The primary scientific role of this Execution is to establish, reuse, or extend scientifically validated Person Identity Artifacts, Information Artifacts, Event Artifacts, other GM Core-conformant Artifacts, and the Relationships required to represent the validated scientific result for one research focus person.

The purpose of these scientific Artifacts is to preserve the validated scientific representation derived from the available scientific evidence for the current research focus person.

The scientific scope of these Artifacts is limited to the validated scientific result produced by this Execution. Specialized scientific interpretation assigned to other GM Executions SHALL NOT be established by this Execution.

Scientific properties of the execution-specific Artifacts SHALL be defined only once and referenced by subsequent chapters rather than redefined.

### 5.2 Core Basis

The execution-specific scientific artifact type shall use the common scientific artifact structure defined by GM Core.

This Execution shall define only the execution-specific dataset description required for its scientific artifact.

The common Core structure shall not be redefined.

### 5.3 Persistent Artifact Identity

Each execution-specific scientific artifact shall possess a persistent artifact identity according to GM Core.

The artifact identity shall remain independent of:

- the identity of the producing tool;
- the temporary execution workspace;
- the later artifacts derived from the scientific artifact;
- the Execution that subsequently processes the scientific artifact.

### 5.4 Artifact Relationships

Execution-specific scientific Artifacts SHALL be connected through
explicit Relationships sufficient to represent their scientific meaning,
provenance, context, and evidentiary support.

The required Relationships SHALL, where applicable:

- use the inherited GM Core Relationship model, endpoint semantics,
  Relationship Context, and Current Relationship State;
- use ParticipationRelationship for scientifically represented event
  participation;
- use ObservationReferenceRelationship or EvidenceSupportRelationship
  according to the scientific meaning of the observation/evidence connection;
- use ReferenceRelationship where a general reference semantic is sufficient;
- use the execution-specific Relationship Expression
  `InformationAttribution` where an Information Artifact is scientifically
  attributed to one represented Person Identity;
- preserve the distinction between identity assignment, scientific
  information, event participation, provenance, evidentiary support, and
  specialized scientific interpretation;
- remain scientifically traceable.

`InformationAttribution` SHALL connect exactly one Person Identity Artifact
and one Information Artifact. Endpoint position alone SHALL NOT determine the
attribution semantics. It SHALL be established only where the applicable PIR
scientific assessment justifies the attribution and SHALL NOT substitute for
the observation or evidence Relationships required to preserve its scientific
basis.

No execution-specific scientific Artifact SHALL be treated as a complete
result where the Relationships required for its scientific meaning,
provenance, or context are absent.

### 5.5 Artifact Independence

Execution-specific scientific Artifacts SHALL be sufficiently
self-contained for subsequent GM Executions to process them using:

- the common GM Core structure;
- the applicable project-retained Dataset Descriptions;
- the registered scientific Artifacts;
- their applicable current Relationship State;
- their explicit provenance, evidentiary support, and uncertainty.

A subsequent GM Execution SHALL NOT depend on access to:

- temporary Observation Assessment Representations;
- Focus-Centred Orientation Projections;
- Person Comparison Workspaces;
- Information and Event Assessment Workspaces;
- temporary candidate Artifacts;
- intermediate scientific assessment results;
- undocumented execution-internal decision state.

### 5.6 Scientific Boundary

The scientific representation established by this Execution SHALL remain
scientifically distinguishable from subsequent specialized scientific
interpretation.

Execution-specific scientific Artifacts SHALL NOT be silently replaced,
reinterpreted, or structurally modified solely because additional
scientific knowledge becomes available through another GM Execution.

Subsequent GM Executions MAY establish additional GM Core-conformant
Artifacts and Relationships representing specialized scientific
interpretation, provided that the scientific representation established
by this Execution remains preserved and scientifically traceable.

### 5.7 Uncertainty Representation

Execution-specific scientific uncertainty SHALL be represented
explicitly and preserved throughout the scientific lifecycle of the
execution-specific Artifacts.

Execution-specific scientific uncertainty SHALL:

- remain explicitly distinguishable from validated scientific
  information;
- remain traceable to the supporting scientific evidence;
- be preserved when scientific Artifacts are reused by subsequent
  GM Executions;
- not be silently removed, replaced, or converted into scientific
  certainty.

Subsequent GM Executions MAY establish additional scientific Artifacts
and Relationships reducing or resolving previously represented
uncertainty where justified by sufficient scientific evidence.

The original execution-specific uncertainty representation SHALL remain
scientifically traceable.

### 5.8 Artifact Dataset Description

The project-retained dataset description SHALL define the persistent
scientific representation of the execution-specific Artifacts produced
by this Execution.

The dataset description SHALL define, where applicable:

- Person Identity Artifacts;
- Information Artifacts;
- Event Artifacts;
- other GM Core-conformant Artifacts established by this Execution;
- the Relationships required to represent their scientific association,
  provenance, and supporting scientific evidence.

The dataset description SHALL describe only the persistent scientific
representation.

Scientific processing behavior, assessment procedures, scientific
derivation, validation methods, and execution workflow SHALL be defined
by other chapters and SHALL NOT be represented within the dataset
description.

### 5.9 Derived Scientific Artifacts

Subsequent GM Executions MAY derive additional scientifically validated
GM Core-conformant Artifacts from the execution-specific Artifacts
established by this Execution, provided that such derivation is
scientifically justified by sufficient scientific evidence.

Derived scientific Artifacts SHALL:

- preserve explicit scientific traceability to the execution-specific
  Artifacts from which they were derived;
- preserve the supporting scientific evidence;
- establish additional scientific meaning through explicit
  Relationships;
- represent an additional scientific interpretation layer;
- not silently replace, reinterpret, or invalidate the execution-specific
  Artifacts.

The execution-specific Artifacts established by this Execution SHALL
remain valid scientific representations unless explicitly revised in
accordance with the applicable GSL and GM Core lifecycle rules.


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

The following Scientific Working Methods define the minimum execution-specific
methods required by this Execution. They inherit the common Scientific Working
Principles of Section 6.2.

#### 6.3.1 Assessment Scope

The Assessment Scope defines the scientific material admitted to the current
person identity assessment.

Material MAY be discovered through Scientific Observations, inherited
Scientific Cluster investigation, candidate comparison, or another
scientifically valid input path.

Admission into the Assessment Scope SHALL be explicit and scientifically
justified. Structural connection alone SHALL NOT constitute evidence of person
identity, kinship, or another scientific conclusion.

Persons or Artifacts inspected within the Assessment Scope SHALL NOT become a
new Focus Person merely through inspection.

The Assessment Scope is a temporary execution-specific method boundary and
SHALL NOT constitute a persistent Scientific Artifact.

#### 6.3.2 Focus-Centred Orientation Projection

A Scientific Working Method MAY construct a temporary Focus-Centred
Orientation Projection to present the current Focus Person together with
scientifically relevant neighboring Artifacts, persons, Events, Information
Artifacts, open comparison points, or investigation boundaries.

The projection is an optional Working Representation.

It SHALL NOT establish scientific facts, identity, kinship, or persistent
project state.

A fieldtest-specific projection depth or genealogical range SHALL NOT be
required by this Execution.

Navigation within the projection SHALL NOT constitute a Focus Person change.
Where another person becomes the subject whose identity is scientifically
assessed, the Focus Person change SHALL be explicit and conform to the
inherited GM Core Research Focus rules and the applicable Processing Profile.

#### 6.3.3 Relationship- and Cluster-Assisted Research

PURPOSE

Use the applicable Current Relationship State and inherited Scientific Cluster
to identify structurally connected scientific material relevant to the current
person identity assessment.

RULES

- structural connection SHALL support investigation only and SHALL NOT by
  itself constitute evidence of person identity, kinship, or another
  scientific conclusion;
- material discovered through structural investigation SHALL enter the
  Assessment Scope only through explicit scientific assessment;
- structural expansion SHALL use a scientifically justified investigation
  boundary;
- no universal traversal depth SHALL be required;
- Relationships SHALL NOT be created solely to increase structural
  connectivity;
- conflicts, unresolved points, and scientifically relevant evidence gaps
  revealed by the investigation SHALL remain explicit;
- absence of a Relationship SHALL NOT automatically be interpreted as evidence
  that the corresponding historical relationship did not exist.

The method MAY inspect scientifically represented shared Events, source or
observation context, locations, Information Artifacts, or other valid common
context where relevant to the Focus Person assessment.

The method is complete when structural investigation is scientifically
sufficient for the applicable PIR assessment or when further expansion cannot
be scientifically justified from the available scientific state.

#### 6.3.4 Person Identity Comparison

PURPOSE

Compare scientifically relevant evidence across existing or candidate Person
Identity representations to support reproducible person identity assessment.

RULES

- the method SHALL distinguish represented scientific information from its
  assessment for the current identity question;
- each material comparison dimension SHALL preserve traceability to its
  scientific basis;
- material comparison results SHALL distinguish agreement, conflict,
  unresolved assessment, and missing information where applicable;
- missing information SHALL remain distinguishable from conflicting
  information;
- where multiple candidates remain scientifically plausible, material
  dimensions SHALL be compared across those candidates where applicable;
- material conflicts and unresolved points SHALL remain explicit;
- the method SHALL NOT require a numeric similarity score, fixed weighting, or
  automatic identity threshold.

A comparison dimension MAY concern names, dates or ages, places, Information
Artifacts, event participation, scientifically represented Relationships,
provenance, supporting or conflicting Scientific Observations, or another
scientifically relevant person-identity characteristic.

No fixed comparison-dimension catalogue or tabular representation is required.

The method is complete when the relevant comparison dimensions have been
assessed to a scientifically sufficient degree for the applicable PIR
scientific result, or when the available evidence does not permit further
scientifically justified resolution.

#### 6.3.5 Information and Event Assessment

Information and event-related evidence SHALL be assessed independently from
person identity before the corresponding persistent Information Artifacts,
Event Artifacts, ParticipationRelationships, InformationAttributions, or
evidence Relationships are established or reused.

The method SHALL preserve the distinction between:

- source-supported observation;
- scientific assessment;
- persistent Information or Event representation;
- attribution to a Person Identity;
- event participation; and
- evidentiary support.

Agreement with a person identity candidate SHALL NOT by itself convert an
observed statement into validated persistent information.

The method MAY use a temporary Information and Event Assessment Workspace.
Such a workspace SHALL remain a nonpersistent Working Representation.

#### 6.3.6 Temporary Working Representations

The methods defined by this Execution MAY use:

- Observation Assessment Representations;
- Focus-Centred Orientation Projections;
- Person Comparison Workspaces;
- Information and Event Assessment Workspaces;
- temporary candidate Artifacts;
- intermediate scientific assessment results.

These Working Representations SHALL remain nonpersistent and
non-authoritative unless an applicable persistent scientific result is
separately validated and established through the artifact and Relationship
semantics of this Execution.

No consuming or subsequent GM Execution SHALL depend on these Working
Representations.


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
 LIKE define one or more Scientific Processing Profiles specifying the
 application of the Scientific Working Methods, including the processing
 sequence, workflow stages, validation, failure handling, and completion
 criteria. Do not redefine Scientific Working Methods or artifact
 semantics.}


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
 LIKE provide one or more complete reference Processing Profiles using
 the following editorial structure:

 #### Profile Name

 #### Scientific Purpose

 #### Applicability

 #### Execution Input

 #### Scientific Working Methods

 #### Processing Sequence

 #### Expected Scientific Result

 #### Validation

 #### Failure Handling

 #### Completion Criteria}
