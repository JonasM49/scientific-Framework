
# GM-Exec Transcription

**Document type:** Release Candidate (RC)
**Version:** RC1
**Status:** Release Candidate
**Architecture level:** GM Execution  
**Normative foundation:** General Scientific Layer (GSL) and GC Core
**AUTHOR** JonasM49
**PUBLISHED_AT** 2026-07-15
**CANONICAL_REPOSITORY** https://github.com/JonasM49/scientific-Framework
**LICENSE** CC-BY-NC-SA 4.0

---

## 0. Document Status

This document is the first **Release Candidate (RC1)** of the GM Execution
for Scientific Document Transcription.

It defines the normative architecture, execution contract, scientific
working methods, scientific processing profiles, validation requirements,
the Controlled GSRAR Update, and the Reference Processing Profile for this
Execution.

The purpose of this Release Candidate is final editorial review prior to
publication.


## 1. Purpose and Scope

### 1.1 Purpose

This Execution shall produce scientifically traceable transcriptions of observable content represented by a Registered Source Artifact (RegisteredSourceArtifact).

It shall transform selected source content into one or more Scientific Observation Artifacts without replacing the observed content through interpretation, normalization, translation, or genealogical reconstruction.

### 1.2 Scientific Task

The single scientific task of this Execution is:

> to observe, localize, transcribe, validate, and represent source content as Scientific Observation Artifacts.

The objective of the Execution is the creation of scientifically sufficient Scientific Observation Artifacts rather than the production of the most detailed transcription possible.

The Execution shall preserve the distinction between source content, transcription result, uncertainty, and later interpretation.

### 1.3 Scope

This Execution shall define:

- the admissible source input;
- selection and localization of a transcription target;
- segmentation of observable source content where required;
- execution-specific transcription methods;
- representation of unreadable, omitted, damaged, continued, or uncertain content;
- validation of the transcription result;
- generation of Scientific Observation Artifacts;
- the project-retained dataset description of the Scientific Observation Artifact type;
- the Controlled GSRAR Update;
- the establishment of one new valid GSRAR Revision.

### 1.4 Out of Scope

This Execution shall not define or perform:

- registration, amendment, replacement, or deletion of GSRAR entries;
- register revision or conflict-resolution procedures;
- semantic interpretation of an observation;
- normalization or translation as a replacement for the observation;
- construction of Person Identity Artifacts, Event Artifacts, or other derived artifacts;
- identity resolution;
- genealogical relationship generation;
- cluster generation;
- OFB generation or publication;
- migration of incompatible artifact structures;
- responsibilities assigned to another GM Execution.

### 1.5 Non-Destructive Principle

This Execution shall not modify the Registered Source Artifact used as input.

Corrections, extensions, or alternative readings shall be represented through new or revised execution results according to the applicable GSL and GC Core rules.

---

### 1.6 Scientific Observation Completeness Principle

The Execution shall complete only when every scientific observation required to satisfy the defined transcription scope has been represented by one or more Scientific Observation Artifacts.

The completion criterion is the scientific completeness of the resulting observation artifacts rather than the completion of a particular transcription method.

## 2. Normative Foundation

### 2.1 General Scientific Layer

This Execution shall conform to the applicable scientific principles, integrity requirements, traceability requirements, and lifecycle rules defined by the GSL.

### 2.2 GC Core

This Execution shall use the artifact, relationship, register, and project structures defined by GC Core.

Core structures shall be referenced and applied. They shall not be redefined in this Execution.

### 2.3 Normative Inheritance

The normative inheritance shall be:

```text
GM-Exec Transcription
    INHERITS GC Core
    INHERITS GSL
```

This Execution shall not inherit from another GM Execution.

No horizontal inheritance between Executions is permitted.

---

### 2.4 Scientific Preconditions

Before execution begins, the following scientific preconditions shall be satisfied:

- the scientific processing scope shall be defined;
- the observable source shall be sufficiently accessible and localizable;
- the selected transcription method shall be appropriate for the source and research objective;
- the Execution shall begin with the least complex applicable transcription method;
- a more detailed transcription method shall only be applied where the preceding method cannot produce scientifically sufficient Scientific Observation Artifacts.

### 2.5 Method Selection Preconditions

Supported transcription methods form a progressive methodological sequence:

```text
1. Scientific Transcription

2. Document Matrix
    INHERITS Scientific Transcription

3. Word Catalogue
    INHERITS Document Matrix

4. Glyph Catalogue
    INHERITS Word Catalogue
```

The following principles apply:

- each method extends the scientific result of the preceding method without replacing it;
- the Glyph Catalogue is not an independent objective, but a supporting analytical method used where required to complete the transcription;
- the Glyph Catalogue shall be be applied only where previous methods cannot achieve a scientifically sufficient observation;
- the objective of every supported method, individually or in combination, is the generation of complete and scientifically reliable Scientific Observation Artifacts.


## 3. Execution Architecture

### 3.1 Execution Unit

This document specifies one independent GM Execution.

The Execution shall be usable without inheritance from, embedding of, or direct control by another GM Execution.

### 3.2 Pipe Model

The normative execution pipe shall be:

```text
1. Execution Input
    RegisteredSourceArtifact

2. Execution
    Scientific Document Transcription

3. Execution Result
    One new valid GSRAR Revision
        established through Controlled GSRAR Update
```

The transcription Execution produces the validated scientific result.

Successful completion of this Execution performs the Controlled GSRAR Update and establishes one new valid GSRAR Revision.

### 3.3 Pipe Boundary

This Execution performs the controlled scientific processing and incorporates validated Scientific Observation Artifacts and their required Relationships into the GSRAR.

Successful completion establishes one new valid GSRAR Revision representing the current scientific working state.

No GSRAR modification shall be implied merely by successful completion of transcription.

### 3.4 Execution Independence

A consuming Execution shall not require knowledge of:

- the internal workflow of this Execution;
- temporary transcription states;
- tools used during transcription;
- rejected readings;
- internal correction history not represented in the resulting GSRAR Revision;
- the identity of the producing implementation.

A consuming Execution shall rely on:

- the shared GC Core structure;
- the project-retained Scientific Observation Artifact type description;
- registered Scientific Observation Artifacts and their valid Relationships.

### 3.5 No Horizontal Inheritance

This Execution shall not inherit structure, behavior, or authority from another GM Execution.

A subsequent Execution shall not inherit from this Execution.

Compatibility between Executions shall be established through shared Core structures, project-retained type descriptions, and explicit input/output contracts.

### 3.6 No Hidden State Transfer

Only explicitly defined artifacts, Relationships, dataset descriptions, validation information, and execution provenance may pass through the pipe.

A subsequent Execution shall not depend on undocumented internal state.

---

## 4. Execution Contract

### 4.1 Required Input

A conforming execution instance shall receive:

- at least one Registered Source Artifact represented in the GSRAR;
- access to the source representation required to observe the selected content;
- an unambiguous reference connecting that representation to the Registered Source Artifact.

The source representation may be an image, scan, page rendering, text-bearing file, or another observable representation permitted by the applicable project context.

### 4.2 Conditional Input

Where required by the selected method or Processing Profile, the execution instance may additionally receive:

- a source locator;
- a defined transcription target;
- page, section, column, line, or region boundaries;
- project-specific transcription parameters;
- an applicable Processing Profile;
- existing non-destructive navigation annotations;
- earlier transcription work used for controlled review or correction.

Conditional input shall not silently alter the scientific meaning of the Registered Source Artifact.

### 4.3 Input Validity

Input shall be rejected or marked incomplete where:

- the Registered Source Artifact cannot be identified;
- the observable source representation cannot be connected to that artifact;
- the transcription target cannot be localized sufficiently;
- the selected Processing Profile cannot be applied;
- required source content is unavailable.

An execution instance shall not compensate for invalid input by inventing source content.

### 4.4 Required Output

A successful Execution SHALL produce validated Scientific Observation Artifacts together with their required Relationships.

Validated results SHALL be incorporated into the GSRAR through the Controlled GSRAR Update defined by this Execution.

The resulting GSRAR Revision SHALL constitute the current valid scientific working state.

The execution instance SHALL preserve:

- source traceability;
- explicit representation of applicable uncertainty;
- required Relationships;
- validation information;
- execution provenance.

### 4.5 Artifact Type Description Output

Where the project does not yet retain the applicable Scientific Observation Artifact dataset description, the Controlled GSRAR Update SHALL incorporate that complete description.

Where the project already retains the description, the produced records shall conform to it.

A change to the dataset description shall not silently invalidate existing records.

### 4.6 Output State

The output of this Execution is one new valid GSRAR Revision established through the Controlled GSRAR Update.

The resulting GSRAR Revision SHALL constitute the current valid scientific working state in accordance with this Execution.

### 4.7 Prohibited Output

The Execution shall not output interpreted genealogical artifacts merely because their meaning appears evident.

In particular, it shall not directly produce:

- Person Identity Artifacts;
- Event Artifacts;
- Place Artifacts formed through interpretation;
- inferred family structures;
- identity Relationships;
- genealogical assertions;
- cluster results;
- OFB entries.

### 4.8 Failure Output

Where successful Scientific Observation Artifact generation is not possible, the Execution may produce a documented incomplete or rejected processing result.

Such a processing result shall not be represented as a valid Scientific Observation Artifact unless it satisfies the applicable artifact contract.

---

## 5. Scientific Observation Artifact Type

### 5.1 Scientific Role

A Scientific Observation Artifact shall represent observable source content produced through a controlled transcription process.

It shall preserve the distinction between:

- observable source content;
- transcription result;
- uncertainty or unreadability;
- later interpretation.

A Scientific Observation Artifact shall not itself represent a person, event, place, family, identity conclusion, or genealogical interpretation.

### 5.2 Core Basis

The Scientific Observation Artifact type shall use the common scientific artifact structure defined by GC Core.

This Execution shall define only the execution-specific dataset description required for transcription observations.

The common Core structure shall not be redefined.

### 5.3 Persistent Artifact Identity

Each Scientific Observation Artifact shall possess a persistent artifact identity according to GC Core.

The artifact identity shall remain independent of:

- the identity of the producing tool;
- the temporary transcription workspace;
- the later artifacts derived from the observation;
- the Execution that subsequently processes the observation.

### 5.4 Mandatory Source Relationship

Each Scientific Observation Artifact shall be accompanied by at least one valid Relationship connecting it to the Registered Source Artifact from which it was produced.

The source Relationship is part of the scientific result of the Execution.

A Scientific Observation Artifact without a valid source Relationship shall not constitute a conforming output of this Execution.

The Relationship shall preserve source traceability without embedding the source artifact as an intrinsic property of the observation where GC Core requires a Relationship.

### 5.5 Relationship Output Principle

This Execution shall produce all Relationships required to represent the scientific provenance and context of each generated Scientific Observation Artifact.

Relationships SHALL be incorporated into the resulting GSRAR Revision together with the corresponding Scientific Observation Artifacts.

An artifact shall not be treated as a complete execution result where the Relationships necessary for its scientific meaning are absent.

### 5.6 Observation Independence

A Scientific Observation Artifact shall be sufficiently self-contained for a subsequent Execution to process it using:

- the common GC Core structure;
- the project-retained Scientific Observation Artifact dataset description;
- the artifact record;
- its valid Relationships.

A subsequent Execution shall not depend on access to:

- the internal transcription workflow;
- temporary matrix states;
- rejected draft readings;
- undocumented tool state;
- undocumented assumptions of the producing Execution.

### 5.7 Interpretation Boundary

A Scientific Observation Artifact shall represent what was observed and transcribed.

It shall not silently replace the observed content through:

- normalized names;
- standardized dates;
- translated text;
- inferred persons;
- constructed events;
- inferred relationships;
- identity conclusions.

Such results shall be created, where justified, by a subsequent Execution as new artifacts and Relationships.

### 5.8 Uncertainty Preservation

Uncertainty belonging to the observation shall be represented explicitly.

Uncertain, damaged, missing, continued, abbreviated, or unreadable content shall not be silently completed.

Later Executions may evaluate uncertainty, but shall not require its absence as a precondition for processing an otherwise valid Scientific Observation Artifact.

### 5.9 Dataset Description

The project shall retain a complete dataset description for the Scientific Observation Artifact type represented in the GSRAR.

The dataset description shall be sufficient for a subsequent Execution to:

- identify records of the type;
- understand the scientific meaning of each field;
- distinguish required and optional fields;
- validate field values;
- interpret references and Relationships;
- identify the representation of uncertainty;
- process the records without knowledge of the producing Execution.

### 5.10 Dataset Description Contents

The Scientific Observation Artifact dataset description shall define at least:

- the artifact type identifier;
- the Core base structure used;
- the record fields;
- field semantics;
- required and optional fields;
- permitted value forms;
- source-localization requirements;
- uncertainty representation;
- required Relationship roles;
- validation constraints.

The exact physical serialization shall be defined separately from the scientific meaning of the dataset.

### 5.11 Version Handling

Individual Scientific Observation Artifacts in the GSRAR shall not require a type-version field.

Changes to the project-retained dataset description should remain backward compatible.

Where an incompatible structural change is required, affected records shall be converted by an applicable transformation or migration Execution before they are processed under the incompatible structure.

Existing records shall not be silently reinterpreted under an incompatible dataset description.

### 5.12 Initial Dataset Areas

The dataset description SHOULD cover at least the following areas:

- artifact identity;
- observed content;
- source localization;
- segmentation reference;
- uncertainty representation;
- omission and damage representation;
- transcription method or Processing Profile reference;
- provenance;
- validation information;
- required source Relationship.


### 5.13 Hypotheses and Other Scientific Results

A hypothesis shall not be embedded as an intrinsic part of a Scientific Observation Artifact.

Where a later Execution creates a hypothesis, it should be represented as a separate scientific artifact and connected through explicit Relationships to the observations and other artifacts on which it depends or which it concerns.

The precise hypothesis artifact contract belongs to the Execution that creates it.

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

#### 6.2.2 Scientific Observation Principle
Scientific Working Methods SHALL operate exclusively on observable source information.

Scientific conclusions SHALL remain distinguishable from scientific observations.

#### 6.2.3 Observation Fidelity
Scientific Working Methods SHALL preserve observable source information faithfully.

They SHALL NOT silently introduce interpretation, normalization, translation, reconstruction, completion of missing content, or genealogical conclusions.

Where uncertainty exists, it SHALL be represented explicitly.

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

### 6.3 Scientific Transcription
*(Abstract Base Method)*

#### 6.3.1 Purpose
Scientific Transcription defines the abstract scientific method for transforming observable source content into a scientifically reproducible transcription.

It provides the common methodological basis for all transcription methods defined by this Execution.

#### 6.3.2 Scope
Scientific Transcription defines how observable source content is transcribed.

It SHALL NOT define:
- execution workflows;
- artifact generation;
- relationship generation;
- GSRAR integration;
- Processing Profile configuration.

These responsibilities belong to subsequent chapters of this Execution.

#### 6.3.3 Observation Fidelity
Scientific Transcription SHALL preserve observable source content faithfully.

It SHALL NOT silently introduce interpretation, normalization, translation, reconstruction, completion of missing content, or genealogical conclusions.

Where uncertainty exists, it SHALL be represented explicitly.

#### 6.3.4 Scientific Sufficiency
Scientific Transcription SHALL achieve scientifically sufficient quality for the defined processing scope.

The objective SHALL be scientific reproducibility rather than maximum transcription detail.

#### 6.3.5 Method Inheritance
All transcription methods defined by this Execution SHALL inherit the requirements of Scientific Transcription.

Concrete methods MAY introduce additional methodological rules.

They SHALL NOT weaken or contradict this abstract method.

#### 6.3.6 Method Objective
The objective of Scientific Transcription is the creation of a scientifically reproducible transcription suitable for subsequent scientific processing.

Scientific Transcription itself does not create persistent scientific artifacts.

#### 6.3.7 Method Completion
Scientific Transcription is complete when the selected transcription method has produced a scientifically sufficient transcription for the defined processing scope.

Subsequent artifact generation belongs to the applicable Scientific Processing Profile.

### 6.4 Linewise Transcription

#### 6.4.1 Purpose

Linewise Transcription defines a concrete refinement of Scientific Transcription by preserving the observable line structure of the source.

It SHALL inherit all requirements defined by Scientific Working Principles and Scientific Transcription.

#### 6.4.2 Applicability

Linewise Transcription SHOULD be applied where line-level representation is scientifically sufficient for the defined processing scope.

Where line-level representation is not scientifically sufficient, Document Matrix Transcription SHOULD be applied.

#### 6.4.3 Line Representation

The transcription SHALL preserve the observable order of the source lines.

Each transcribed line SHALL remain traceable to its observable source location.

The method SHALL preserve observable uncertainty without interpretation.

#### 6.4.4 Method Completion

The method is complete when all observable lines within the defined processing scope have been transcribed with scientifically sufficient quality.

Subsequent scientific processing SHALL be performed by the applicable Scientific Processing Profile.


### 6.5 Document Matrix Transcription

#### 6.5.1 Purpose

Document Matrix Transcription defines a refinement of Linewise Transcription by constructing a Document Matrix that preserves the observable spatial structure of the selected source content.

It SHALL inherit all requirements defined by Scientific Working Principles, Scientific Transcription, and Linewise Transcription.

#### 6.5.2 Applicability

Document Matrix Transcription SHOULD be applied where preservation of the observable spatial structure contributes to the scientific transcription.

#### 6.5.3 Document Matrix

The Document Matrix SHALL represent the observable document structure using Matrix Elements.

Each Matrix Element SHALL contain exactly one observable word or one observable table field.

The Document Matrix SHALL preserve the observable order and spatial arrangement of the source.

The Document Matrix SHALL constitute the authoritative Working Representation for all derived transcription methods.

#### 6.5.4 Matrix Coordinates

The Document Matrix SHALL define the authoritative coordinate system for all derived working representations.

Each Matrix Element SHALL possess a unique and stable coordinate.

The default coordinate syntax SHOULD follow the form:

Sx-Zxx-Wxx

where:

- S identifies the source page.
- Z identifies the line within the page.
- W identifies the word within the line.
- x represents a sequential counting number.

Example:

S2-Z04-W03

#### 6.5.5 Working Representation

The Document Matrix MAY be represented using a UTF-8 Pipe-Separated Value (PSV) structure or another reproducible working representation.

The physical serialization SHALL NOT alter the scientific meaning of the Document Matrix.

#### 6.5.6 Method Completion

The method is complete when all observable Matrix Elements within the defined processing scope have been represented in the Document Matrix.

Subsequent scientific processing SHALL be performed by the applicable Scientific Processing Profile.

### 6.6 Word Catalogue Transcription

#### 6.6.1 Purpose

Word Catalogue Transcription defines a refinement of Document Matrix Transcription by constructing a Word Catalogue from the observable words contained in the Document Matrix.

It SHALL inherit all requirements defined by Scientific Working Principles, Scientific Transcription, Linewise Transcription, and Document Matrix Transcription.

#### 6.6.2 Applicability

Word Catalogue Transcription SHOULD be applied where comparison of recurring observable words contributes to the scientific transcription.

It SHOULD be used before escalation to Glyph Catalogue Transcription.

#### 6.6.3 Word Catalogue

The Word Catalogue SHALL contain all observable words within the defined processing scope.

Each catalogue entry SHALL include:

- the observable word;
- one or more references to the corresponding Matrix Elements using the authoritative Document Matrix coordinate system.

The Word Catalogue SHALL constitute an internal scientific comparison resource.

The Word Catalogue SHALL NOT define an independent coordinate system.

It SHALL NOT modify the authoritative Document Matrix.

#### 6.6.4 Scientific Comparison

Recurring observable words MAY be compared using the Word Catalogue to improve the scientific assessment of partially unreadable words.

Comparisons SHALL remain limited to observable evidence contained within the current Document Matrix.

Where the Word Catalogue does not provide scientifically sufficient evidence, Glyph Catalogue Transcription SHOULD be applied.

#### 6.6.5 Method Completion

The method is complete when all observable words within the defined processing scope have been catalogued and linked to their corresponding Matrix Elements.

Subsequent scientific processing SHALL be performed by the applicable Scientific Processing Profile.

### 6.7 Glyph Catalogue Transcription

#### 6.7.1 Purpose

Glyph Catalogue Transcription defines a refinement of Word Catalogue Transcription by constructing a Glyph Catalogue for selected observable glyphs where the Word Catalogue does not provide scientifically sufficient evidence.

It SHALL inherit all requirements defined by Scientific Transcription, Document Matrix Transcription, and Word Catalogue Transcription.

#### 6.7.2 Applicability

Glyph Catalogue Transcription SHOULD be applied only where the Word Catalogue does not provide scientifically sufficient evidence for the assessment of one or more observable words.

#### 6.7.3 Glyph Catalogue

The Glyph Catalogue SHALL contain multiple observable occurrences of the glyphs required for scientific comparison.

Each catalogue entry SHALL include:

- the observable glyph;
- the corresponding Document Matrix coordinate extended by `-Bxx`, where **B** identifies the glyph position within the referenced word and **x** represents a sequential counting number.

Example:

`S2-Z04-W03-B07`

The Glyph Catalogue SHALL constitute an internal scientific comparison resource.

The Glyph Catalogue SHALL NOT define an independent coordinate system.

#### 6.7.4 Scientific Comparison

Observable glyphs MAY be compared only with other observable glyphs contained within the current processing scope.

Scientific conclusions SHALL remain limited to observable evidence.

#### 6.7.5 Method Completion

The method is complete when all required glyph comparisons have been performed and the scientific transcription has reached scientifically sufficient quality.

Subsequent scientific processing SHALL be performed by the applicable Scientific Processing Profile.


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

### 7.3 Execution Initialization

#### 7.3.1 Purpose

Execution Initialization establishes the controlled scientific processing context for a Scientific Processing Profile.

It SHALL inherit the Workflow Principles defined in Section 7.2.

#### 7.3.2 Initialization Context

Execution Initialization SHALL establish at least:

- the Registered Source Artifact being processed;
- the defined scientific processing scope;
- the applicable Scientific Working Method or methods;
- the selected Scientific Processing Profile;
- the expected GSRAR Revision to be established by successful completion of the workflow;
- the applicable validation requirements.

Initialization SHALL NOT itself create Scientific Observation Artifacts or Relationships.

#### 7.3.3 Required Inputs

Execution Initialization SHALL verify the availability of:

- the Registered Source Artifact;
- the applicable dataset descriptions;
- the selected Scientific Processing Profile;
- applicable execution parameters;
- required scientific context.

Missing required inputs SHALL prevent normal execution.

#### 7.3.4 Initialization Result

Execution Initialization is complete when a controlled scientific processing context has been established.

Subsequent workflow stages SHALL operate within this initialized context.

### 7.4 Source Validation

#### 7.4.1 Purpose

Source Validation verifies that the scientific input satisfies the requirements for controlled scientific processing.

It SHALL inherit the Workflow Principles defined in Section 7.2.

#### 7.4.2 Validation Scope

Source Validation SHALL verify at least:

- identification of the Registered Source Artifact;
- availability of the required source representation;
- applicability of the selected Scientific Processing Profile;
- completeness of the required scientific input;
- suitability of the defined scientific processing scope.

#### 7.4.3 Validation Result

Where validation requirements are not satisfied, the Scientific Processing Profile SHALL NOT continue with normal processing.

The workflow MAY instead produce a documented incomplete or rejected work result.

#### 7.4.4 Stage Completion

Source Validation is complete when the scientific input has been validated for the subsequent workflow stages.

### 7.5 Transcription Target Definition

#### 7.5.1 Purpose

Transcription Target Definition identifies the observable source content that belongs to the scientific processing scope.

It SHALL inherit the Workflow Principles defined in Section 7.2.

#### 7.5.2 Target Definition

The Scientific Processing Profile SHALL define the source content intended for scientific processing before any Scientific Working Method is applied.

The transcription target MAY comprise:

- a complete source representation;
- one or more pages;
- one or more register entries;
- a bounded excerpt;
- a defined visual region;
- another reproducibly identifiable source segment.

#### 7.5.3 Target Requirements

The defined transcription target SHALL:

- be scientifically reproducible;
- be distinguishable from source content outside the processing scope;
- provide sufficient information for subsequent workflow stages.

A partial transcription SHALL NOT be represented as a complete transcription.

#### 7.5.4 Stage Completion

Transcription Target Definition is complete when the scientific processing scope has been defined with scientifically sufficient precision for the subsequent workflow stages.

### 7.6 Source Localization

#### 7.6.1 Purpose

Source Localization identifies the observable position of the scientific processing target within the Registered Source Artifact.

It SHALL inherit the Workflow Principles defined in Section 7.2.

#### 7.6.2 Localization Requirements

Each scientific processing target SHALL be localized with scientifically sufficient precision.

Localization SHALL enable subsequent Scientific Working Methods to identify the observable source content reproducibly.

#### 7.6.3 Localization Methods

Localization MAY use, as applicable:

- page identifiers;
- folio identifiers;
- image identifiers;
- register-entry identifiers;
- line or column references;
- Document Matrix coordinates;
- bounded visual regions;
- other reproducible source locators.

Localization SHALL describe observable source position only.

It SHALL NOT introduce scientific interpretation.

#### 7.6.4 Stage Completion

Source Localization is complete when the scientific processing target has been localized with scientifically sufficient precision for the subsequent workflow stages.

### 7.7 Source Segmentation

#### 7.7.1 Purpose

Source Segmentation defines the observable source segments that shall be processed by the selected Scientific Working Method.

It SHALL inherit the Workflow Principles defined in Section 7.2.

#### 7.7.2 Segmentation Requirements

The Scientific Processing Profile SHALL apply a segmentation strategy appropriate for the observable source representation and the defined scientific processing scope.

The selected segmentation SHALL preserve the observable source structure required for scientific processing.

#### 7.7.3 Segmentation Methods

Segmentation MAY distinguish, as applicable:

- complete documents;
- pages;
- folios;
- register entries;
- sections;
- columns;
- lines;
- words;
- bounded visual regions;
- marginal content;
- continuation segments.

The segmentation strategy SHALL preserve the observable order and context of the source.

It SHALL NOT introduce interpretation or artificial source structure.

#### 7.7.4 Stage Completion

Source Segmentation is complete when the scientific processing target has been divided into scientifically reproducible observable segments suitable for the selected Scientific Working Method.

### 7.8 Scientific Observation Construction

#### 7.8.1 Purpose

Scientific Observation Construction transforms the results of the applied Scientific Working Methods into Scientific Observation Artifacts.

It SHALL inherit the Workflow Principles defined in Section 7.2.

#### 7.8.2 Construction Requirements

Scientific Observation Artifacts SHALL conform to the applicable Scientific Observation Artifact dataset description defined by the GM Core.

Construction SHALL preserve the validated scientific observations independently of temporary Working Representations.

#### 7.8.3 Construction Result

Each Scientific Observation Artifact SHALL remain scientifically traceable to the observable source content from which it was constructed.

#### 7.8.4 Stage Completion

Scientific Observation Construction is complete when all validated scientific observations required by the Scientific Processing Profile have been represented as Scientific Observation Artifacts.

### 7.9 Relationship Construction

#### 7.9.1 Purpose

Relationship Construction establishes the Relationships required to preserve the scientific provenance and context of the Scientific Observation Artifacts.

It SHALL inherit the Workflow Principles defined in Section 7.2.

#### 7.9.2 Relationship Requirements

Relationship Construction SHALL create all Relationships required by the applicable GM Core structures and the Scientific Observation Artifact dataset description.

Required Relationships SHALL preserve at least:

- scientific provenance;
- source traceability;
- scientific context.

#### 7.9.3 Construction Result

Constructed Relationships SHALL connect the corresponding Scientific Observation Artifacts to the required GM Core artifacts.

Relationship Construction SHALL NOT introduce scientific interpretation beyond the applicable GM Core rules.

#### 7.9.4 Stage Completion

Relationship Construction is complete when all mandatory Relationships required for the Scientific Observation Artifacts have been established.

### 7.10 Artifact–Relationship Completeness

#### 7.10.1 Purpose

Artifact–Relationship Completeness verifies that all Scientific Observation Artifacts required by the Scientific Processing Profile possess the mandatory Relationships defined by the applicable GM Core structures.

It SHALL inherit the Workflow Principles defined in Section 7.2.

#### 7.10.2 Completeness Requirements

The workflow SHALL verify that:

- all required Scientific Observation Artifacts have been constructed;
- all mandatory Relationships have been established;
- no mandatory scientific linkage is missing.

#### 7.10.3 Completeness Result

Where mandatory Artifacts or Relationships are missing, the workflow SHALL NOT establish a new valid GSRAR Revision.

The workflow MAY instead terminate as failed or interrupted processing according to Section 7.14.

#### 7.10.4 Stage Completion

Artifact–Relationship Completeness is complete when all mandatory Artifacts and Relationships required by the Scientific Processing Profile have been verified.

### 7.11 Validation

#### 7.11.1 Purpose

Validation verifies that the execution result satisfies the applicable Scientific Processing Profile and the inherited scientific requirements.

It SHALL inherit the Workflow Principles defined in Section 7.2.

#### 7.11.2 Validation Requirements

Validation SHALL verify at least:

- conformity with the applicable Scientific Processing Profile;
- completion of all mandatory workflow stages;
- scientific consistency of the constructed Artifacts and Relationships;
- compliance with the applicable GM Core structures.

#### 7.11.3 Validation Result

Where validation requirements are satisfied, the workflow MAY proceed to the Controlled GSRAR Update defined in Section 7.12.

Where validation requirements are not satisfied, the workflow SHALL produce a documented validation result indicating the identified deficiencies.

#### 7.11.4 Stage Completion

Validation is complete when the execution result has been scientifically evaluated against the applicable Scientific Processing Profile.
### 7.12 Controlled GSRAR Update

#### 7.12.1 Purpose

Controlled GSRAR Update establishes one new valid GSRAR Revision by incorporating the validated Scientific Observation Artifacts and their required Relationships into the persistent GSRAR.

#### 7.12.2 Update Requirements

Only validated Artifacts and Relationships SHALL be incorporated into the GSRAR.

The update SHALL preserve:

- artifact identity;
- relationship integrity;
- scientific traceability;
- the continuity of the current valid scientific working state.

#### 7.12.3 Incremental Persistence

A Scientific Processing Profile MAY persist validated results after scientifically complete processing units, including individual lines, source sections, pages, or complete documents.

Each such update SHALL produce a valid and internally consistent GSRAR Revision.

#### 7.12.4 GSRAR Revision

Each successful Controlled GSRAR Update SHALL create one new valid GSRAR Revision.

The new GSRAR Revision SHALL constitute the current valid scientific working state of the project.

The previous GSRAR Revision SHALL remain reproducible according to the applicable GSL and GM Core requirements.

#### 7.12.5 Stage Completion

Controlled GSRAR Update is complete when one new valid GSRAR Revision has been established through incorporation of the validated Artifacts and Relationships.


### 7.13 GSRAR Revision Result

#### 7.13.1 Purpose

GSRAR Revision Result defines the scientific result produced by a successfully completed Scientific Processing Profile.

It SHALL inherit the Workflow Principles defined in Section 7.2.

#### 7.13.2 Result Definition

A successfully completed Scientific Processing Profile SHALL produce one new valid GSRAR Revision.

The new revision SHALL constitute the current valid scientific working state of the project.

#### 7.13.3 Result Properties

The resulting GSRAR Revision SHALL:

- preserve all previously valid scientific information unless explicitly revised;
- incorporate the validated Artifacts and Relationships produced during the execution;
- preserve scientific traceability;
- remain internally consistent;
- remain suitable as the authoritative working state for subsequent scientific processing.

#### 7.13.4 Scientific Continuation

Subsequent Scientific Processing Profiles SHALL use the latest valid GSRAR Revision as their scientific starting point.

Earlier GSRAR Revisions SHALL remain reproducible according to the applicable GSL and GM Core requirements.

#### 7.13.5 Stage Completion

GSRAR Revision Result is complete when the new valid GSRAR Revision has been established as the current scientific working state.

### 7.14 Failed or Interrupted Processing

#### 7.14.1 Purpose

Failed or Interrupted Processing defines the scientific handling of a Scientific Processing Profile that cannot be completed successfully.

It SHALL inherit the Workflow Principles defined in Section 7.2.

#### 7.14.2 Processing Requirements

Where a Scientific Processing Profile cannot be completed, the workflow SHALL preserve the current valid GSRAR Revision unchanged.

The workflow SHALL document the processing status and the reason for the incomplete execution.

Unvalidated Artifacts or Relationships SHALL NOT be incorporated into the GSRAR.

#### 7.14.3 Interrupted Processing Result

A failed or interrupted execution SHALL NOT establish a new GSRAR Revision.

The latest valid GSRAR Revision SHALL remain the current scientific working state.

The workflow MAY retain temporary working representations outside the persistent GSRAR where permitted by the applicable Scientific Processing Profile.

#### 7.14.4 Scientific Continuation

Scientific work MAY resume from the latest valid GSRAR Revision after the causes of interruption have been resolved.

Continuation SHALL preserve scientific traceability and reproducibility.

#### 7.14.5 Stage Completion

Failed or Interrupted Processing is complete when the execution outcome has been documented and the integrity of the persistent GSRAR has been preserved.



## 8. Processing Profiles

### 8.1 Purpose

A Scientific Processing Profile shall define an execution configuration for a specific transcription situation without changing the Scientific Observation Artifact contract unnecessarily.

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

The Scientific Processing Profile shall define the method-specific rules for segmentation and transcription.

The Execution contract shall define the scientific stages and result requirements.

The Scientific Observation Artifact dataset description shall define the representation of the resulting observation.

Accordingly:

- the Execution defines the scientific task;
- the Processing Profile defines the applied method;
- the dataset description defines the persistent result structure.

A Scientific Processing Profile shall not alter the scientific meaning of the Scientific Observation Artifact type.


### 8.4 Profile Boundary

A Scientific Processing Profile may configure transcription behavior.

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
- conformity with the Scientific Observation Artifact type description;
- scientific consistency of the constructed Artifacts and Relationships;
- conformity with the applicable GM Core structures;
- reproducibility of the observation;
- separation from interpretation.

### 9.3 Invalid Results

An invalid or incomplete result shall not be silently converted into a valid Scientific Observation Artifact.

The handling of incomplete or rejected processing results SHALL follow Section 4.8 and Section 7.14.

---

## 10. Controlled GSRAR Update

### 10.1 Controlled GSRAR Update

The Execution SHALL incorporate validated Scientific Observation Artifacts together with their required Relationships into the GSRAR through a controlled scientific update.

Only validated scientific results SHALL be incorporated.

Each successful update SHALL establish one new valid GSRAR Revision.

### 10.2 Current Valid GSRAR Revision

Each successful Controlled GSRAR Update SHALL establish one new valid GSRAR Revision.

The resulting revision SHALL constitute the current valid scientific working state of the project.

Earlier GSRAR Revisions SHALL remain reproducible according to the applicable GSL and GM Core requirements.

### 10.3 Project Type Description

Where the Scientific Observation Artifact type description is not yet available in the project, the resulting GSRAR Revision shall provide the complete description required for its project-level retention.

Where the description already exists, the Execution shall use a compatible structure.

---

## 11. Execution Conformance

A conforming implementation of this Execution shall:

- accept only defined input structures;
- preserve the registered source artifact;
- perform transcription without genealogical interpretation;
- produce Scientific Observation Artifacts conforming to the project-retained dataset description;
- produce and transfer the required source Relationships with every observation;
- preserve explicit uncertainty;
- provide source traceability;
- validate its output before Controlled GSRAR Update;
- avoid horizontal inheritance from another Execution;
- avoid hidden dependencies on internal workflow state.


---

## Appendix A — Reference Processing Profile

### A.1 Purpose

This Appendix provides the reference Processing Profile defined by
Section 8.2.

The reference Processing Profile serves as a specification template for
project-specific Scientific Processing Profiles.

### A.2 Tabular Document Transcription

#### A.2.1 Purpose

Defines a reference Processing Profile for structured tabular source
documents.

#### A.2.2 Applicability

Applicable where the observable table structure contributes to the
scientific transcription.

#### A.2.3 Processing Scope

The profile applies to the defined transcription target without changing
the scientific scope of the Execution.

#### A.2.4 Profile-specific Rules

- Identify the table header where present.
- Where no readable header exists, the project MAY define the expected
  column identities before transcription.
- Preserve the observable column order.
- Preserve empty table cells.
- Represent each observable table cell as one Matrix Element.

#### A.2.5 Applied Scientific Working Methods

- Scientific Transcription
- Document Matrix
- Word Catalogue (where required)
- Glyph Catalogue (where scientifically necessary)

#### A.2.6 Expected Scientific Result

Validated Scientific Observation Artifacts incorporated into one new
valid GSRAR Revision.

