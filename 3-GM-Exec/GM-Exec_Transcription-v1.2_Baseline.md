# GM-Exec Transcription

STATUS: Baseline

VERSION: 1.2

DOCUMENT_IDENTIFIER: GM-Exec-Transcription

DOCUMENT_TYPE: GM Execution

DEPENDS_ON: GSL-2.0, GM-Core-v1.2

LANGUAGE: DSL SPECIFICATION_LINEAGE

AUTHOR: JonasM49

PUBLISHED_AT: 2026-09-19

CANONICAL_REPOSITORY: https://github.com/JonasM49/scientific-Framework

LICENSE: CC-BY-NC-SA-4.0


------------------------------------------------------------------------

## 1. Purpose and Scope

### 1.1 Purpose

This Execution shall produce scientifically traceable transcriptions of
observable content represented by a Registered Source
(RegisteredSource).

It shall transform selected research-relevant source content into one or
more Scientific Observation Artifacts without replacing the observed
information through scientific interpretation, translation, genealogical
reconstruction, or other assessment beyond the transcription boundary.

Resolved transcription information MAY be represented in a structured
form where that representation preserves the established informational
content, remains traceable to the transcription basis, and does not
imply a scientific assessment beyond transcription.

### 1.2 Scientific Task

The single scientific task of this Execution is:

> to observe, localize, transcribe, validate, select, and represent
> research-relevant source information as Scientific Observation
> Artifacts.

The objective of the Execution is the creation of scientifically
sufficient Scientific Observation Artifacts rather than the production
of the most detailed transcription possible.

The Execution shall preserve the distinction between source content,
transcription result, remaining uncertainty, and later scientific
assessment.

A Scientific Observation Artifact represents observed information
established through controlled transcription. It SHALL NOT by its
existence imply the truth, completeness, or final scientific validity of
that information.

### 1.3 Scope

This Execution shall define:

-   the admissible source input;
-   selection and localization of a transcription target;
-   segmentation of observable source content where required;
-   execution-specific transcription methods;
-   representation of unreadable, omitted, damaged, continued, or
    uncertain content;
-   persistent transcription working state where required by the
    applicable Processing Profile;
-   controlled selection of research-relevant observed information from
    the progressed transcription;
-   temporary review representations where used;
-   validation of the transcription result and Observation Construction;
-   generation of Scientific Observation Artifacts;
-   the execution-level dataset description used, where required, to
    realize the GM Core `ScientificObservation` model;
-   construction and validation of the applicable Relationships connecting
    generated Scientific Observation Artifacts to their Registered Source;
-   establishment of a validated, registration-ready scientific result;
-   the Execution Handoff Boundary to subsequent persistent register
    modification.

### 1.4 Out of Scope

This Execution shall not define or perform:

-   registration, amendment, replacement, or deletion of Registered
    Source Artifacts;
-   scientific reconciliation of competing observations or persistent
    scientific states;
-   semantic interpretation of an observation beyond representational
    resolution required for transcription;
-   translation as a replacement for the observation;
-   assessment of historical truth or source reliability;
-   construction of Person Identity Artifacts, Event Artifacts, or other
    derived artifacts;
-   identity resolution;
-   genealogical relationship generation;
-   cluster generation;
-   OFB generation or publication;
-   migration of incompatible artifact structures;
-   responsibilities assigned to another GM Execution.

### 1.5 Non-Destructive Principle

This Execution shall not modify the Registered Source used as input.

Corrections, extensions, alternative readings, or newly constructed
observations shall be represented through controlled execution results
according to the applicable GSL and GM Core rules.

Existing scientific information shall not be silently overwritten,
harmonized, invalidated, or rejected merely because a newly processed
source differs from it or does not contain corresponding information.

### 1.6 Scientific Observation Completeness Principle

The Execution shall complete only when every research-relevant
scientific observation required to satisfy the defined transcription
scope has been represented by one or more Scientific Observation
Artifacts.

The completion criterion is the scientific sufficiency of the resulting
observation artifacts for the defined scope rather than complete
reproduction of the Document Matrix, calibration state, or any
particular transcription method.

## 2. Normative Foundation

### 2.1 General Scientific Layer

This Execution shall conform to the applicable scientific principles,
integrity requirements, traceability requirements, and lifecycle rules
defined by GSL v2.0.

### 2.2 GM Core

This Execution shall use the artifact, relationship, register, and
project structures defined by the applicable GM Core normative foundation.

Core structures shall be referenced and applied. They shall not be
redefined in this Execution.

### 2.3 Normative Inheritance

GM-Exec Transcription SHALL inherit the applicable normative
requirements of:

-   GM Core;
-   GSL.

This Execution shall not inherit from another GM Execution.

No horizontal inheritance between Executions is permitted.

### 2.4 Scientific Preconditions

Before execution begins, the following scientific preconditions shall be
satisfied:

-   the scientific processing scope shall be defined;
-   the observable source shall be sufficiently accessible and
    localizable;
-   the selected transcription method or combination of methods shall be
    appropriate for the source and research objective;
-   the applicable Processing Profile shall define or permit the method
    application required for the selected source and scope;
-   formal decryption refinement shall be applied only where the
    preceding transcription and calibration state cannot produce
    scientifically sufficient results for the defined scope.

No universal requirement exists to apply every available transcription
method or to apply all methods in a fixed sequence.

### 2.5 Scientific Working Method Architecture

Scientific Transcription provides the common methodological basis.

Depending on source structure and the applicable Processing Profile,
transcription MAY use Linewise Transcription or Document Matrix
Transcription.

Document Matrix Transcription MAY be refined iteratively through
Transcription Calibration. Transcription Calibration does not require
formal catalogue escalation.

Where systematic decryption requires more detailed addressable
comparison, formal refinement MAY proceed from the Document Matrix
through a Word Catalogue and, where word-level refinement remains
insufficient, through a Glyph Catalogue.

The following principles apply:

-   applicable methods MAY be selected, combined, and iterated according
    to the Processing Profile;
-   Transcription Calibration is a documented working method and not a
    mandatory escalation stage;
-   Word Catalogue and Glyph Catalogue provide a formal decryption
    refinement path where required;
-   each formal refinement shall preserve traceability to the
    transcription state from which it was developed;
-   the Glyph Catalogue is not an independent objective, but a
    supporting analytical method used where required;
-   the objective of every supported method, individually or in
    combination, is a scientifically sufficient transcription basis for
    the construction of conforming Scientific Observation Artifacts.

## 3. Execution Architecture

### 3.1 Execution Unit

This document specifies one independent GM Execution.

The Execution shall be usable without inheritance from, embedding of, or
direct control by another GM Execution.

### 3.2 Pipe Model

The normative execution pipe shall consist of the following stages:

1.  Execution Input: The Execution receives a Registered Source, an
    observable Source Representation, and applicable Processing Profile
    context where required.
2.  Scientific Document Transcription: The Execution establishes and
    progresses the controlled transcription working state required by
    the applicable Processing Profile.
3.  Scientific Observation Construction: Research-relevant observed
    information is represented as conforming Scientific Observations and
    required Relationships.
4.  Validation: The resulting Scientific Observations and Relationships
    are validated according to this Execution.
5.  Execution Handoff Preparation: The validated Scientific Observations,
    applicable Source–Observation Relationships, preserved uncertainty,
    and required provenance are established as a registration-ready
    scientific result.
6.  Execution Result: Successful completion establishes that validated,
    registration-ready scientific result for transfer across the Execution
    Handoff Boundary defined by Section 10.

The transcription Execution produces transcription-conforming Scientific
Observation Artifacts and required Relationships.

The term `validated` in this Execution denotes conformity with the
applicable transcription process and representation requirements. It
does not denote historical truth or final genealogical validity.

Successful completion establishes a validated, registration-ready
scientific result. Persistent incorporation and establishment of a new
Register Revision belong to the applicable register-modification Execution.

### 3.3 Pipe Boundary

This Execution performs controlled scientific transcription processing and
produces validated Scientific Observation Artifacts together with the
applicable Relationships required for their scientific provenance and
context.

Successful completion establishes a registration-ready scientific result.
Persistent incorporation into the applicable scientific register, including
the establishment of a new valid Register Revision, belongs to the applicable
register-modification Execution and SHALL NOT be performed by this Execution.

Completion of a transcription method, progression of a Document Matrix,
or construction of a temporary review representation SHALL NOT by itself
imply modification of the AGRAR.

### 3.4 Execution Independence

A consuming Execution shall not require knowledge of:

-   the internal workflow of this Execution;
-   the complete transcription working state;
-   temporary review or comparison representations;
-   tools used during transcription;
-   rejected readings;
-   internal correction history not required by the resulting persistent
    scientific state;
-   the identity of the producing implementation.

A consuming Execution shall rely on:

-   the shared GM Core structure;
-   the project-retained Scientific Observation Artifact dataset
    description;
-   registered Scientific Observation Artifacts and their valid
    Relationships;
-   applicable persistent provenance and validation information.

A persistent Document Matrix AWD MAY remain available for transcription
continuation, review, or recovery, but a consuming Execution SHALL NOT
depend on it unless another applicable contract explicitly requires that
working representation.

### 3.5 No Horizontal Inheritance

This Execution shall not inherit structure, behavior, or authority from
another GM Execution.

A subsequent Execution shall not inherit from this Execution.

Compatibility between Executions shall be established through shared GM
Core structures, project-retained dataset descriptions, and explicit
input/output contracts.

### 3.6 No Hidden State Transfer

Only explicitly defined Scientific Artifacts, Relationships, dataset
descriptions, validation information, execution provenance, and other
persistent structures permitted by the applicable GM Core or project
contract may cross an Execution boundary.

A subsequent Execution shall not depend on undocumented internal state.

Persistent transcription Working Representations remain working state
unless an independent applicable contract explicitly defines them as an
input to another process.

## 4. Execution Contract

### 4.1 Required Input

A conforming execution instance shall receive:

-   at least one Registered Source represented in the AGRAR;
-   access to the observable source representation required for the
    defined transcription scope;
-   an unambiguous reference connecting that representation to the
    Registered Source.

The source representation may be an image, scan, page rendering,
text-bearing file, or another observable representation permitted by the
applicable project context.

### 4.2 Conditional Input

Where required by the selected method or Processing Profile, the
execution instance may additionally receive:

-   a source locator;
-   a defined transcription target;
-   page, section, column, line, field, word, or region boundaries;
-   project-specific transcription parameters;
-   an applicable Processing Profile;
-   existing non-destructive navigation annotations;
-   earlier transcription working state used for controlled
    continuation, review, correction, or calibration;
-   existing persistent scientific state required for the Existing
    Scientific State Check.

Conditional input shall remain distinguishable from observable source
content and shall not silently alter the scientific meaning of the
Registered Source.

### 4.3 Input Validity

Input shall be rejected or marked incomplete where:

-   the Registered Source cannot be identified;
-   the observable source representation cannot be connected to that
    artifact;
-   the transcription scope or target cannot be localized sufficiently;
-   a required Processing Profile cannot be applied;
-   required source content is unavailable.

An execution instance shall not compensate for invalid or incomplete
input by inventing source content or by treating contextual expectation
as observation.

### 4.4 Required Output

A successful Execution SHALL produce:

-   validated Scientific Observation Artifacts required by the defined
    research-relevant transcription scope;
-   all Relationships required for their provenance and scientific
    context;
-   applicable validation information;
-   execution provenance;
-   a validated, registration-ready scientific result suitable for transfer
    to the applicable register-modification Execution.

`Validated` SHALL have the meaning defined by Section 9: conformity with
this Execution and the applicable Processing Profile, not proof of
historical truth.

The execution instance SHALL preserve:

-   source and transcription-basis traceability;
-   relevant remaining uncertainty;
-   required Relationships;
-   distinguishability of representational resolution from later
    scientific assessment;
-   material distinctions from potentially corresponding existing
    scientific information;
-   validation information;
-   execution provenance.

### 4.5 Observation Representation Description Output

Where an execution-level Observation dataset description is required to
realize the GM Core `ScientificObservation` model, the project SHALL
retain a description sufficient for the operational representation
defined by Sections 5.9--5.12.

Where such a description already exists, produced records SHALL conform
to the applicable representation.

The description SHALL remain subordinate to the normative
`ScientificObservation` structure and semantics defined by GM Core.

A change to the execution-level representation shall not silently
invalidate or reinterpret existing Scientific Observations.

### 4.6 Working-State Output

Where the applicable Processing Profile requires persistent
transcription working state, the Execution SHALL preserve the required
progressed Working Representation independently of the Scientific
Observation Artifact output.

For a Document Matrix profile, this MAY include the progressed Document
Matrix AWD and scientifically material calibration state.

Persistent transcription working state:

-   supports continuation, review, and recovery;
-   does not become a Scientific Artifact merely through persistence;
-   does not replace Scientific Observation Construction;
-   need not be consumed by subsequent Executions.

Temporary review or comparison representations need not persist where
they can be regenerated without scientific loss.

### 4.7 Registration-Ready Scientific Output State

The scientific output of successful completion is a validated,
registration-ready result containing the Scientific Observation Artifacts,
applicable Relationships, validation information, and execution provenance
required by the defined scope.

Persistent incorporation of that result into the applicable scientific
register and establishment of a new Register Revision belong to the
applicable register-modification Execution.

Completion of this Execution SHALL NOT imply that persistent registration
has occurred.

### 4.8 Prohibited Output

The Execution shall not output interpreted genealogical artifacts or
Research Processing conclusions merely because their meaning appears
evident.

In particular, it shall not directly produce:

-   Person Identity Artifacts;
-   Event Artifacts formed through genealogical interpretation;
-   Place Artifacts formed through interpretation;
-   inferred family structures;
-   identity Relationships;
-   genealogical assertions;
-   reconciliation decisions concerning competing historical claims;
-   source-reliability conclusions;
-   cluster results;
-   OFB entries.

### 4.9 Failure or Incomplete Output

Where successful Scientific Observation Artifact generation, validation, or
preparation of the registration-ready scientific result is not possible, the
Execution MAY preserve a documented incomplete processing state.

Where the applicable Processing Profile requires persistent
transcription working state, that state MAY remain available for
continuation or recovery.

An incomplete or rejected processing result SHALL NOT be represented as
a valid Scientific Observation Artifact unless it independently
satisfies the applicable artifact contract.

An interrupted or failed processing attempt SHALL NOT be represented as a
successfully completed, registration-ready Transcription result. It SHALL NOT
by itself establish persistent register modification or a new Register
Revision.

## 5. Scientific Observation Artifact Type

### 5.1 Scientific Role

A Scientific Observation Artifact shall represent research-relevant
information established from observable source content through a
controlled transcription process.

It shall preserve sufficient provenance to distinguish observed source
information from subsequent scientific assessment.

It shall preserve the distinction between:

-   observable source content;
-   transcription result;
-   representational resolution performed within the transcription
    boundary;
-   remaining uncertainty or unreadability;
-   later scientific assessment.

A Scientific Observation Artifact shall not itself represent a person,
event, place, family, identity conclusion, or genealogical
interpretation.

The existence of a Scientific Observation Artifact SHALL NOT imply the
truth, completeness, or final scientific validity of the information it
represents.

### 5.2 Core Basis

The Scientific Observation Artifact type shall use the common scientific
artifact structure defined by GM Core.

This Execution shall define only the execution-specific operational
representation required to realize transcription observations.

The normative `ScientificObservation` structure and semantics defined by
GM Core shall be referenced and realized, not redefined.

### 5.3 Persistent Artifact Identity

Each Scientific Observation Artifact shall possess a persistent artifact
identity according to GM Core.

The artifact identity shall remain independent of:

-   the identity of the producing tool;
-   the temporary transcription workspace;
-   the persistent transcription working state from which it was
    constructed;
-   the later artifacts derived from the observation;
-   the Execution that subsequently processes the observation.

### 5.4 Mandatory Source–Observation Relationship

Each Scientific Observation Artifact shall be accompanied by at least
one valid Relationship connecting it to the Registered Source from which
it was produced.

The Source–Observation Relationship is part of the scientific result of the
Execution.

A Scientific Observation Artifact without a valid Source–Observation Relationship
shall not constitute a conforming output of this Execution.

The Source–Observation Relationship shall preserve source traceability without embedding
the source artifact as an intrinsic property of the observation where GM
Core requires a Relationship.

### 5.5 Relationship Output Principle

This Execution shall produce all Relationships required to represent the
scientific provenance and context of each generated Scientific
Observation Artifact.

The applicable Relationships SHALL be included in the validated,
registration-ready scientific result together with the corresponding
Scientific Observation Artifacts.

An artifact shall not be treated as a complete execution result where
the Relationships necessary for its scientific meaning are absent.

### 5.6 Observation Independence

A Scientific Observation Artifact shall be sufficiently self-contained
for a subsequent Execution to process it using:

-   the common GM Core structure;
-   the project-retained Scientific Observation Artifact dataset
    description;
-   the artifact record;
-   its valid Relationships.

A Scientific Observation Artifact need not reproduce the complete
Document Matrix, calibration material, rejected reading paths, or other
transcription working state.

A subsequent Execution shall not depend on access to:

-   the internal transcription workflow;
-   temporary review representations;
-   the complete transcription working state;
-   rejected draft readings;
-   undocumented tool state;
-   undocumented assumptions of the producing Execution.

### 5.7 Interpretation and Representational Resolution Boundary

A Scientific Observation Artifact shall represent observed information
established through controlled transcription.

Transcription MAY resolve and structurally represent information where
the resolution is supported by the observable source and the resulting
representation preserves the established informational content and
traceability.

Such representational resolution MAY include, for example, representing
an established written date expression in a structured date field while
retaining sufficient provenance to the observed source information.

Representational resolution SHALL remain distinguishable from later
scientific assessment.

This Execution shall not silently replace or extend observed information
through:

-   normalization that changes the observed informational content;
-   translation as a substitute for the observed information;
-   assessment of source reliability;
-   resolution of competing historical claims;
-   inferred persons;
-   constructed events;
-   inferred genealogical relationships;
-   identity conclusions.

Such scientific results shall be created, where justified, by an
applicable subsequent Execution as new artifacts and Relationships.

### 5.8 Uncertainty Preservation

Relevant uncertainty remaining after transcription processing and
Observation Construction shall be represented explicitly.

Uncertain, damaged, missing, continued, abbreviated, or unreadable
content shall not be silently completed.

Where an uncertainty has been sufficiently resolved within the
transcription boundary through traceable assessment of observable source
form, the resolved reading need not remain represented as unresolved
merely because an earlier working state contained uncertainty.

Later Executions may scientifically assess remaining uncertainty, but
shall not require its absence as a precondition for processing an
otherwise valid Scientific Observation Artifact.

### 5.9 Observation Dataset Description

Where implementation-specific representation, persistence, or
serialization requires an execution-level dataset description, the
project SHALL retain a description sufficient to realize the GM Core
`ScientificObservation` model for transcription output.

The dataset description SHALL NOT redefine the normative scientific
semantics, minimum structure, provenance responsibilities, uncertainty
model, Processing Profile responsibilities, or other requirements of
`ScientificObservation` established by GM Core.

Its purpose is to define the operational representation by which this
Execution realizes those Core requirements.

Scientific Observation output produced by this Execution SHALL represent each
source-derived Observation Element in a manner that is unambiguously
addressable under the applicable project-retained dataset description.

Structural organization of the Observation output SHALL NOT by itself encode
genealogical relationships, person identity, event participation, or other
interpreted semantic associations. Where such semantics are scientifically
required, they SHALL be represented through the applicable downstream
scientific model rather than inferred from structural nesting.

The dataset description shall be sufficient for a subsequent conforming
Execution to:

-   identify Scientific Observation records;
-   map represented fields to the applicable GM Core requirements;
-   distinguish required and optional execution-level representations;
-   validate permitted value forms;
-   interpret references and Relationships;
-   identify the representation of remaining uncertainty;
-   distinguish structured representational resolution from later
    scientific assessment;
-   process the records without knowledge of undocumented internal
    transcription state.

### 5.10 Observation Dataset Description Contents

The execution-level Observation dataset description shall define, where
applicable:

-   the mapping to the GM Core `ScientificObservation` structure;
-   implementation-specific record fields;
-   field representation and permitted value forms;
-   required and optional execution-level fields;
-   source-localization representation;
-   segmentation-reference representation;
-   uncertainty representation;
-   representation of resolved structured observed information where
    used;
-   Relationship representation required by this Execution;
-   execution-level validation constraints;
-   persistence and serialization realization.

Requirements already defined normatively by GM Core SHALL be referenced
and realized rather than redefined.

The exact physical serialization may be specified independently from the
scientific meaning established by GM Core.

### 5.11 Version Handling

Individual Scientific Observation Artifacts in AGRAR shall not require
an additional execution-specific type-version field unless required by
an applicable implementation contract.

Changes to the execution-level Observation dataset description SHOULD
remain backward compatible.

Where an incompatible implementation-specific structural change is
required, affected records shall be transformed or migrated through a
controlled process before they are processed under the incompatible
representation.

Existing Scientific Observations SHALL NOT be silently reinterpreted
through a changed execution-level representation.

### 5.12 Initial Representation Areas

The execution-level Observation dataset description SHOULD cover the
operational representation needed for at least the following areas where
they are applicable to this Execution:

-   artifact identity;
-   observed information;
-   input and source localization;
-   segmentation reference;
-   remaining uncertainty;
-   omission and damage representation;
-   structured representation of resolved observed information;
-   Processing Profile and processing provenance references;
-   validation information;
-   required Relationships.

This list describes execution-level representation areas only. The
normative scientific requirements governing `ScientificObservation`
remain those of GM Core.

### 5.13 Hypotheses and Other Scientific Results

A scientific hypothesis extending beyond the transcription boundary
shall not be embedded as an intrinsic part of a Scientific Observation
Artifact.

Transcriptional candidate readings and calibration hypotheses MAY exist
within the controlled transcription working state before Observation
Construction.

Where a later Execution creates a scientific hypothesis concerning
historical interpretation, identity, relationship, reliability, or
another research conclusion, it should be represented as a separate
scientific artifact and connected through explicit Relationships to the
observations and other artifacts on which it depends or which it
concerns.

The precise hypothesis artifact contract belongs to the Execution that
creates it.

## 6. Scientific Working Methods

### 6.1 Purpose

#### 6.1.1 Scientific Purpose

The purpose of the Scientific Working Methods is to define scientific
methods and working aids that MAY be used by this Execution to produce
scientifically reproducible transcription results.

Scientific Working Methods define how scientific work is performed.

They SHALL NOT define:

-   execution workflows;
-   processing sequences;
-   artifact generation;
-   register modification procedures;
-   project-specific Processing Profiles.

These responsibilities belong to the applicable Scientific Processing
Profile and subsequent processing rules.

#### 6.1.2 Architectural Role

Scientific Working Methods form the methodological layer of this
Execution.

They provide reusable methods that MAY be referenced, selected,
combined, or iterated by one or more Scientific Processing Profiles.

A Scientific Working Method SHALL remain scientifically understandable
independently of a particular Processing Profile.

#### 6.1.3 Method Implementation Principle

Scientific Working Methods defined in this Section specify scientific
functions, assessment boundaries, and reproducibility requirements
rather than mandatory user-interface conventions or notation systems.

A Processing Profile or project MAY define alternative notation,
symbols, visual encodings, segmentation conventions, or comparison
representations, provided that:

-   their meaning is documented;
-   relevant uncertainty remains distinguishable;
-   the scientific distinctions required by the applicable method remain
    reproducible;
-   the representation does not silently convert a candidate or
    descriptive form into a resolved reading.

Examples in this Section are illustrative implementations and SHALL NOT
establish mandatory notation unless explicitly stated otherwise.

#### 6.1.4 Relationship to Scientific Processing Profiles

A Scientific Processing Profile SHALL select the Scientific Working
Methods required for its task.

A Processing Profile MAY refine the application of a method for a
specific scientific task.

It SHALL NOT redefine or weaken the normative scientific requirements of
the referenced method.

### 6.2 Scientific Working Principles

#### 6.2.1 Purpose

Scientific Working Principles define the common scientific principles
that SHALL apply to all Scientific Working Methods defined by this
Execution.

Concrete methods SHALL inherit these principles unless explicitly
strengthened.

#### 6.2.2 Scientific Observation Principle

Scientific Working Methods SHALL operate on observable source
information.

Contextual or prior information MAY generate or constrain transcription
candidates where an applicable method permits it.

Such information SHALL NOT replace assessment of the observable source
form.

Scientific conclusions extending beyond the transcription boundary SHALL
remain distinguishable from transcription observations and working
hypotheses.

#### 6.2.3 Observation Fidelity

Scientific Working Methods SHALL preserve observable source information
faithfully.

They SHALL NOT silently introduce interpretation, translation,
genealogical reconstruction, completion of missing content, or
normalization that changes the observed informational content.

Representational resolution permitted by Section 5.7 remains admissible.

Where relevant uncertainty remains, it SHALL be represented explicitly.

#### 6.2.4 Scientific Sufficiency

A Scientific Working Method SHALL achieve scientifically sufficient
quality for the defined processing scope.

The objective SHALL NOT be maximum detail but scientifically sufficient
reproducibility.

#### 6.2.5 Method Selection and Formal Refinement

Where systematic decryption requires a more formal addressable
comparison structure, refinement MAY proceed from the Document Matrix to
a Word Catalogue.

Where word-level refinement remains insufficient, refinement MAY proceed
from the Word Catalogue to a Glyph Catalogue.

A more detailed formal refinement SHOULD be applied only where the
preceding method does not provide sufficient scientific resolution.

#### 6.2.6 Working Representations

Scientific Working Methods MAY construct Working Representations to
support scientific processing.

Working Representations MAY be temporary or persistent according to the
applicable Processing Profile.

A Working Representation SHALL NOT constitute a Scientific Artifact
merely because it is persistent, versionable, or required for recovery.

Where a Processing Profile requires a persistent transcription working
state, the relevant Working Representation SHALL preserve sufficient
scientifically material state for continuation, review, and recovery.

#### 6.2.7 Method Completion

A Scientific Working Method is complete when it has achieved
scientifically sufficient results for the defined processing scope.

Completion of a method SHALL NOT by itself imply completion of the
Execution.

### 6.3 Scientific Transcription

#### 6.3.1 Purpose

Scientific Transcription defines the abstract scientific method for
transforming observable source content into a scientifically
reproducible transcription.

It provides the common methodological basis for all transcription
methods defined by this Execution.

#### 6.3.2 Scope

Scientific Transcription defines how observable source content is
transcribed.

It SHALL NOT define:

-   execution workflows;
-   artifact generation;
-   relationship generation;
-   AGRAR incorporation;
-   Processing Profile configuration.

These responsibilities belong to subsequent chapters of this Execution.

#### 6.3.3 Observation Fidelity

Scientific Transcription SHALL preserve observable source content
faithfully.

It SHALL NOT silently introduce interpretation, translation,
genealogical reconstruction, completion of missing content, or
normalization that changes observed informational content.

Representational resolution permitted by Section 5.7 remains admissible.

Where relevant uncertainty remains, it SHALL be represented explicitly.

#### 6.3.4 Scientific Sufficiency

Scientific Transcription SHALL achieve scientifically sufficient quality
for the defined processing scope.

The objective SHALL be scientific reproducibility rather than maximum
transcription detail.

#### 6.3.5 Method Inheritance

All transcription methods defined by this Execution SHALL inherit the
requirements of Scientific Transcription.

Concrete methods MAY introduce additional methodological rules.

They SHALL NOT weaken or contradict this abstract method.

#### 6.3.6 Working-State Boundary

Scientific Transcription MAY create or progress Working Representations.

Such Working Representations do not become Scientific Artifacts solely
through their use or persistence.

Persistent scientific artifact generation belongs to the applicable
Scientific Processing Profile.

#### 6.3.7 Method Completion

Scientific Transcription is complete when the selected method or
combination of methods has produced a scientifically sufficient
transcription for the defined processing scope.

### 6.4 Linewise Transcription

#### 6.4.1 Purpose

Linewise Transcription defines a concrete refinement of Scientific
Transcription by preserving the observable line structure of the source.

It SHALL inherit all requirements defined by Scientific Working
Principles and Scientific Transcription.

#### 6.4.2 Applicability

Linewise Transcription SHOULD be applied where line-level representation
is scientifically sufficient for the defined processing scope.

Where preservation of more detailed spatial or word-level addressability
contributes materially to the scientific task, Document Matrix
Transcription SHOULD be applied.

#### 6.4.3 Line Representation

The transcription SHALL preserve the observable order of the source
lines.

Each transcribed line SHALL remain traceable to its observable source
location.

The method SHALL preserve relevant observable uncertainty without
scientific interpretation beyond the transcription boundary.

#### 6.4.4 Method Completion

The method is complete when the observable lines required by the defined
processing scope have been transcribed with scientifically sufficient
quality.

### 6.5 Document Matrix Transcription

#### 6.5.1 Purpose

Document Matrix Transcription defines a refinement of Scientific
Transcription by constructing an addressable Document Matrix that
preserves the observable structure of selected source content.

It SHALL inherit all requirements defined by Scientific Working
Principles and Scientific Transcription.

#### 6.5.2 Applicability

Document Matrix Transcription SHOULD be applied where word-level or
field-level addressability, spatial structure, iterative calibration, or
recoverable transcription progression contributes to the scientific
task.

#### 6.5.3 Document Matrix

The Document Matrix SHALL represent the selected observable document
structure using Matrix Elements.

Each Matrix Element SHALL contain one observable word or one observable
table field unless the applicable Processing Profile documents a
scientifically equivalent segmentation required by the source structure.

The Document Matrix SHALL preserve the observable order and
scientifically relevant spatial arrangement of the source.

It SHALL provide the authoritative addressable Working Representation
for transcription calibration and formal catalogue refinement derived
from the Matrix.

#### 6.5.4 Matrix Coordinates

The Document Matrix SHALL define the authoritative coordinate system for
its addressable elements.

Each Matrix Element SHALL possess a unique and stable coordinate within
the working state.

The default coordinate syntax SHOULD follow the form:

`Sx-Zxx-Wxx`

where:

-   S identifies the source page;
-   Z identifies the line within the page;
-   W identifies the word within the line;
-   x represents a sequential counting number.

Example:

`S2-Z04-W03`

A Processing Profile MAY define an equivalent documented coordinate
convention where required by the source structure.

#### 6.5.5 Working Representation and Persistence

The Document Matrix MAY be represented using a UTF-8 Pipe-Separated
Value (PSV) structure or another reproducible representation.

The physical serialization SHALL NOT alter its scientific meaning.

Where the applicable Processing Profile requires the Document Matrix as
persistent transcription working state, the progressed Matrix SHALL
preserve sufficient scientifically material reading, localization,
uncertainty, and calibration state for continuation, review, and
recovery.

Persistence of the Document Matrix SHALL NOT by itself make the Matrix a
Scientific Artifact.

#### 6.5.6 Calibration Basis

Resolved or sufficiently supported addressable Matrix Elements MAY serve
as comparison material for other unresolved elements where permitted by
an applicable Transcription Calibration method.

Material calibration that changes or materially supports a reading SHALL
remain sufficiently documented in the transcription working state to
preserve reproducibility.

A separate log of every resolved word or glyph is not required where the
progressed Document Matrix and associated calibration state already
preserve the scientifically relevant progression.

#### 6.5.7 Method Completion

The method is complete when the Matrix Elements required by the defined
processing scope have been represented and the Document Matrix provides
scientifically sufficient transcription state for subsequent processing.

### 6.6 Transcription Calibration Toolkit

#### 6.6.1 Purpose

Transcription Calibration defines low-threshold, documented methods for
developing and testing transcription readings against observable source
form.

Calibration MAY proceed iteratively and in parallel with Document Matrix
progression.

It SHALL NOT constitute a mandatory escalation to a Word Catalogue or
Glyph Catalogue.

The methods in this Section form an extensible toolkit. A Processing
Profile MAY select one or more applicable methods.

#### 6.6.2 Common Calibration Boundary

Calibration MAY use:

-   source-local recurring forms;
-   securely or sufficiently resolved readings;
-   constrained vocabularies;
-   known source metadata;
-   likely formula language;
-   visual comparison;
-   writer-specific form characteristics.

Such information MAY generate, constrain, support, weaken, or reject a
transcription candidate.

It SHALL NOT establish a reading solely because the candidate is
contextually expected.

Calibration SHALL preserve material uncertainty and SHALL remain within
the transcription boundary.

#### 6.6.3 Bracketed Reading

Purpose: Bracketed Reading provides a reproducible way to distinguish
unresolved, partial, alternative, or descriptively captured readings
from sufficiently resolved transcription.

Applicability: It MAY be used whenever a source element cannot yet be
represented as a sufficiently supported plain reading.

Procedure: The working representation records the unresolved state and
MAY contain:

-   a candidate reading;
-   alternative character or word candidates;
-   a partial reading;
-   a visual or form-oriented description.

The reading is reassessed as additional source-local evidence becomes
available.

Representation: Square brackets are an illustrative implementation, for
example:

``` text
[Wur?er]
[o/u?]
[f-artig]
[enge n]
```

A project MAY use another documented notation with equivalent scientific
distinctions.

Assessment Boundary: The notation SHALL distinguish an unresolved
working state from a resolved reading.

Removal or replacement of the uncertainty notation means only that the
transcription reading has become sufficiently resolved within the
transcription boundary. It SHALL NOT imply that the represented
historical information is true.

Completion / Result: A bracketed reading MAY progress from a descriptive
form such as `[f-artig]` to a narrowed candidate such as `[s?]` and,
where sufficiently resolved, to a plain reading such as `s`.

No separate solved-word log is required where the progressed working
state preserves the relevant change.

#### 6.6.4 Descriptive Glyph Calibration

Purpose: Descriptive Glyph Calibration records observable form
characteristics before or without prematurely assigning a character
identity.

Applicability: It SHOULD be used where character identity is uncertain
but repeatable visual features can be described and compared.

Procedure: A glyph or sequence is described phenomenologically, linked
to its source location, and compared with other addressable occurrences.

Examples include:

``` text
[f-artig]
[o oben offen]
[o/u schwer unterscheidbar]
```

Representation: Descriptions MAY refer to form, openness, loops,
connections, relative stroke position, or another observable
characteristic.

Assessment Boundary: Writer-specific calibration SHALL remain
distinguishable from a universal character rule.

For example, if a securely read occurrence shows that a writer uses an
`[f-artig]` form for `s`, that observation MAY support another
occurrence by the same writer. It SHALL NOT establish the universal rule
`[f-artig] = s`.

Completion / Result: The method produces a documented comparison basis
capable of supporting, narrowing, or leaving unresolved one or more
candidate readings.

#### 6.6.5 Number and Formula Anchor Calibration

Purpose: Number and Formula Anchor Calibration uses constrained textual
domains to generate and test transcription candidates.

Applicability: It MAY be used where observable source structure suggests
a constrained class of expressions, including:

-   written year values;
-   day-number words;
-   month words;
-   age-number words;
-   recurring documentary formulae.

A date may be represented numerically or otherwise. A known date value
is useful as a written-text anchor only where the observable source form
supports the hypothesis that a corresponding written expression is
present.

Procedure: A known or constrained value generates one or more
candidates. Those candidates are compared against the observable word or
glyph form.

Further occurrences, such as age statements or recurring formula
elements, MAY then be used to expand the source-local calibration basis.

Representation: For example, a known year such as `1854` MAY provide a
constrained candidate for a written-year expression. The candidate is
compared against the observable source form. The comparison result is
assessed as supported, uncertain, or rejected.

A month word MAY similarly be compared against the constrained set of
possible month words, after which a preceding day-number word may be
assessed against plausible number-word candidates.

Assessment Boundary: Expected content SHALL NOT replace observable
source evidence.

A seemingly familiar formula SHALL NOT be used as a textual template
from which unread source content is completed.

Formula comparison MAY generate or constrain transcription candidates.
Each candidate remains subject to assessment against observable source
form.

Apparent conformity with an expected document type SHALL NOT establish
that document type.

Completion / Result: The method produces one or more supported,
uncertain, or rejected candidates and MAY create anchors for subsequent
source-internal calibration.

#### 6.6.6 Stroke-Pattern Comparison

Purpose: Stroke-Pattern Comparison assesses recurring handwriting
characteristics at a finer visual level without requiring immediate
formal Glyph Catalogue construction.

Applicability: It MAY be used where candidate glyphs remain ambiguous
after word-level comparison.

Procedure: Comparison MAY consider:

-   entry stroke;
-   exit stroke;
-   loop direction;
-   ascender or descender form;
-   open or closed construction;
-   connections to neighboring glyphs;
-   repeated stroke sequences;
-   relative line position.

Representation: The comparison SHOULD describe observable form before
assigning character identity where identity remains uncertain.

Assessment Boundary: Similarity supports comparison but SHALL NOT by
itself establish glyph identity.

Completion / Result: The method yields a documented form comparison
sufficient to support, narrow, reject, or preserve uncertainty among
candidate readings.

#### 6.6.7 Visual Glyph Segmentation

Purpose: Visual Glyph Segmentation separates visually complex words or
sequences into comparable glyph or stroke regions.

Applicability: It MAY be used where connected handwriting makes
boundaries or recurring forms difficult to compare.

Procedure: The source representation or a reproducible working copy MAY
be marked to distinguish relevant visual segments and corresponding
occurrences.

Representation: Illustrative implementations include:

-   different colors;
-   outlines;
-   labels;
-   overlays;
-   numbered regions.

Colors SHALL NOT possess fixed semantic meaning unless the applicable
Processing Profile documents such meaning.

Assessment Boundary: Segmentation is a comparison aid. It SHALL NOT
silently alter the underlying source representation or establish
character identity by visual marking alone.

Completion / Result: The method produces reproducibly identifiable
visual segments for comparison with other source-local occurrences.

#### 6.6.8 Same-Writer Comparison

Purpose: Same-Writer Comparison uses recurring forms produced by the
same writer as high-value calibration material.

Applicability: It SHOULD be preferred where sufficiently resolved
same-writer occurrences are available and materially relevant to an
unresolved reading.

Procedure: An unresolved form is compared with one or more addressable
occurrences from the same writer, considering word context, glyph form,
and stroke characteristics as applicable.

Representation: The compared occurrences SHALL remain traceable to their
source locations.

Assessment Boundary: Similarity MAY support a candidate but SHALL NOT
alone establish identity.

Writer-specific findings SHALL remain writer-specific unless
independently supported beyond that context.

Completion / Result: The method strengthens, weakens, or leaves
unresolved a candidate reading using documented same-writer evidence.

#### 6.6.9 Small-Window and Overlap Comparison

Purpose: Small-Window and Overlap Comparison reduces visual complexity
while preserving enough context to compare difficult source segments.

Applicability: It MAY be used for dense handwriting, repeated
structures, or source areas where full-page comparison obscures relevant
detail.

Procedure: Small source excerpts are assessed independently or
comparatively. Adjacent excerpts SHOULD overlap sufficiently to preserve
continuity and localization.

Where overlapping source segments are used, the overlap MAY serve as a
continuation and comparison anchor. Processing of an overlapping source
portion SHALL NOT result in duplicate persistent representation of the
same source element in the applicable Document Matrix. Material
differences identified through the overlap SHALL be processed under the
applicable Comparative Refinement rules.

The method MAY be combined with Bracketed Reading, Descriptive Glyph
Calibration, Stroke-Pattern Comparison, Visual Glyph Segmentation, or
Same-Writer Comparison.

Representation: Each excerpt or window SHALL remain traceable to its
source location.

Assessment Boundary: Cropping or windowing SHALL NOT remove
scientifically relevant context without preserving a route back to the
source representation.

Completion / Result: The method produces localized comparison evidence
while maintaining source continuity and traceability.

#### 6.6.10 Calibration State

Transcription Calibration MAY establish reusable Calibration State within
the Scientific Working Context.

Calibration State represents source-near knowledge established for
comparative transcription processing, including applicable reference
forms, glyph characteristics, connections, stroke patterns, anchors,
alternatives, and known transfer limitations.

Calibration State is Working State and SHALL NOT constitute an independent
Scientific Artifact.

Where formally retained, applicable existing Working Representations,
including the Authoritative Working Draft, Word Catalogue, Glyph Catalogue,
or Document Matrix, MAY preserve the information required to reproduce or
continue that Calibration State.

Calibration State SHALL NOT directly modify a target transcription element.
Any material change to the current transcription state SHALL pass through
the applicable Transcription Processing defined in Chapter 7.

### 6.7 Word Catalogue Transcription

#### 6.7.1 Purpose

Word Catalogue Transcription defines a formal refinement of Document
Matrix Transcription by constructing a systematic Word Catalogue from
observable words contained in the Document Matrix.

It SHALL inherit all applicable requirements defined by Scientific
Working Principles, Scientific Transcription, and Document Matrix
Transcription.

#### 6.7.2 Applicability

Word Catalogue Transcription SHOULD be applied where systematic
comparison of recurring observable words is required and low-threshold
calibration does not provide scientifically sufficient evidence.

It forms the first formal catalogue stage before Glyph Catalogue
Transcription.

#### 6.7.3 Word Catalogue

The Word Catalogue SHALL contain the observable words required by the
defined formal refinement scope.

Each catalogue entry SHALL include:

-   the observable word or unresolved word representation;
-   one or more references to corresponding Matrix Elements using the
    authoritative Document Matrix coordinate system.

The Word Catalogue SHALL constitute an internal scientific comparison
resource.

It SHALL NOT define an independent coordinate system.

It SHALL NOT silently modify the authoritative Document Matrix.

#### 6.7.4 Scientific Comparison

Recurring observable words MAY be compared using the Word Catalogue to
improve assessment of partially unreadable words.

Comparisons SHALL remain traceable to observable source occurrences.

Where the Word Catalogue does not provide scientifically sufficient
evidence for the required formal refinement, Glyph Catalogue
Transcription SHOULD be applied.

#### 6.7.5 Relationship to Transcription Calibration

Individual word comparisons performed during ordinary Transcription
Calibration do not require construction of a Word Catalogue.

The Word Catalogue is a systematic formal refinement structure and SHALL
remain distinguishable from low-threshold iterative calibration.

#### 6.7.6 Method Completion

The method is complete when the words required by the formal refinement
scope have been catalogued, linked to their Matrix Elements, and
assessed sufficiently for the defined processing objective.

### 6.8 Glyph Catalogue Transcription

#### 6.8.1 Purpose

Glyph Catalogue Transcription defines a formal refinement of Word
Catalogue Transcription by constructing a systematic Glyph Catalogue for
selected observable glyphs where word-level evidence remains
insufficient.

It SHALL inherit all applicable requirements defined by Scientific
Transcription, Document Matrix Transcription, and Word Catalogue
Transcription.

#### 6.8.2 Applicability

Glyph Catalogue Transcription SHOULD be applied only where the preceding
transcription, calibration, and Word Catalogue state does not provide
scientifically sufficient evidence for one or more required readings.

#### 6.8.3 Glyph Catalogue

The Glyph Catalogue SHALL contain multiple observable occurrences of the
glyphs required for systematic scientific comparison where such
occurrences are available.

Each catalogue entry SHALL include:

-   the observable glyph or descriptive glyph representation;
-   the corresponding Document Matrix coordinate extended by `-Bxx`,
    where B identifies the glyph position within the referenced word and
    x represents a sequential counting number.

Example:

`S2-Z04-W03-B07`

The Glyph Catalogue SHALL constitute an internal scientific comparison
resource.

It SHALL NOT define an independent coordinate system.

#### 6.8.4 Scientific Comparison

Observable glyphs MAY be compared with other traceable observable glyph
occurrences within the applicable processing scope.

Comparison MAY use the calibration methods defined in Section 6.6.

Scientific conclusions SHALL remain within the transcription boundary.

#### 6.8.5 Relationship to Transcription Calibration

Descriptive glyph comparison, visual segmentation, stroke comparison, or
same-writer comparison performed during ordinary calibration SHALL NOT
by itself require construction of a Glyph Catalogue.

The Glyph Catalogue is the formal systematic escalation for cases
requiring fine-grained addressable glyph analysis.

#### 6.8.6 Method Completion

The method is complete when the required systematic glyph comparisons
have been performed and the transcription has reached scientifically
sufficient quality for the defined scope.

## 7. Scientific Processing Profiles

### 7.1 Purpose

Scientific Processing Profiles define the controlled processing logic by
which this Execution applies Scientific Working Methods to a particular
class of transcription task.

A Processing Profile SHALL define how applicable methods are selected,
combined, sequenced, iterated, or applied in parallel.

A Processing Profile SHALL preserve the scientific boundaries defined by
this Execution and SHALL NOT weaken the requirements of the referenced
methods.

### 7.2 Processing Profile Responsibility

A Processing Profile SHALL define at least:

-   the applicable source and transcription scope;
-   the selected Scientific Working Methods;
-   the required Working Representations;
-   whether a persistent transcription working state is required;
-   applicable segmentation and localization rules;
-   the conditions for iterative calibration;
-   the conditions for formal catalogue refinement where applicable;
-   the construction and review of research-relevant Scientific
    Observations;
-   Validation;
-   preparation of the registration-ready scientific result and the
    Execution Handoff Boundary.

A Processing Profile MAY define additional operational detail provided
that it remains within the Execution boundary.

### 7.3 Method Application

Scientific Working Methods MAY be applied sequentially, iteratively, or
in parallel where scientifically appropriate.

The Processing Profile SHALL ensure that the resulting transcription
remains traceable and that material changes introduced through
calibration or comparative assessment remain sufficiently reproducible.

Low-threshold Transcription Calibration SHALL NOT require formal Word
Catalogue or Glyph Catalogue construction unless the conditions for
formal refinement are met.

### 7.4 Transcription Element State

Transcription Element State represents the current source-near transcription
state of an identifiable portion of the Source Representation against which
new source-near information may be scientifically assessed.

A Transcription Element State MAY be represented by:

-   an addressed element of a persistent Document Matrix; or
-   an unambiguously identifiable temporary element within the Scientific
    Working Context.

Persistence SHALL NOT be a precondition for Transcription Processing.

Where the Processing Profile requires a persistent Document Matrix, the
applicable progressed Matrix Element SHALL remain the authoritative persistent
transcription representation for that source portion. The progressed Document
Matrix AWD SHALL preserve sufficient scientifically material information for:

-   continuation after interruption;
-   review of unresolved readings;
-   review of material calibration;
-   recovery of the current transcription state; and
-   traceability of Observation Construction.

Persistence SHALL NOT by itself make the Document Matrix AWD, a temporary
Transcription Element State, or another Working Representation a Scientific
Artifact.

Temporary comparison views, review summaries, image excerpts, or other aids
MAY be regenerated from the persistent working state where their scientific
function does not require independent persistence.

Transcription Element State SHALL remain source-near. It MAY preserve proposed
or established readings, segmentation information, glyphic or lexical
information, alternatives, uncertainty, applicable calibration information,
and source location or working references required for controlled assessment.
It SHALL NOT encode genealogical interpretation, person identity, event
participation, normalized genealogical meaning, or other downstream Research
Processing conclusions.

New source-near information SHALL NOT silently replace an existing
Transcription Element State. A material state transition SHALL result from the
applicable assessment and comparative refinement defined by this Processing.
The resulting state MAY retain, extend, refine, revise, or leave unresolved the
applicable source-near content.

A material state transition SHALL preserve the traceability required by the
inherited scientific principles to the applicable Source Representation,
identifiable source portion, and scientifically material basis of the change.
This requirement SHALL NOT establish a separate revision-history architecture
for Transcription Element State.

### 7.5 Collaborative Assessment

Where multiple source segments, repeated expressions, or mutually informative
occurrences are expected to be compared, each relevant segment SHOULD first be
assessed independently to the extent scientifically practicable.

The purpose of initial independent assessment is to reduce premature
propagation of an assumed reading from one occurrence to another. This
requirement SHALL NOT be interpreted as a mandatory blind-test procedure or as
requiring a fixed Human–AI participant sequence.

Where Transcription Processing is performed collaboratively, applicable
Transcription Scientific Working Methods MAY be performed by either Human or AI
participants under the inherited GSL Collaboration Model. The Processing SHALL
NOT require a fixed allocation of transcription methods to particular
participant types.

Collaborative Assessment SHALL provide meaningful counter-assessment of
material source-near readings before they are treated as sufficiently assessed
for downstream processing. It SHALL NOT require every assessment operation to
be independently duplicated by every participant.

Assessment MAY include, as scientifically applicable, glyphic assessment,
lexical assessment, hypothesis or alternative formation, source-near
comparison, calibration, counter-reading, segmentation assessment, and
reassessment following material revision. Applicable operations MAY occur
iteratively and in different orders. Lexical plausibility SHALL NOT override
contradictory observable glyphic evidence.

Assessment SHALL be sufficiently performed for the intended Transcription
Processing before the assessed source-near content is treated as sufficiently
established for the applicable downstream transcription step.

Sufficient assessment SHALL NOT imply certainty, exhaustive decipherment, or
resolution of every alternative. Unresolved readings, alternatives, or
uncertainty MAY remain after sufficient assessment and SHALL be preserved where
scientifically material.

Processing MAY pause assessment of one element while calibration or assessment
proceeds elsewhere in the Source Representation. Such interruption SHALL NOT be
treated as a processing failure.

Where material revision invalidates or materially weakens the preceding
assessment basis, applicable assessment SHALL be performed again.

### 7.6 Comparative Refinement

After applicable assessment, new source-near information MAY be compared with
an identifiable existing Transcription Element State where such comparison is
scientifically applicable.

Comparison MAY use any applicable method defined in Section 6 and SHALL conform
to the inherited requirements for preservation of evidence, uncertainty,
material differences, and scientific traceability.

Comparison SHALL NOT silently replace an existing reading, conceal material
uncertainty or disagreement, or force resolution where the available
source-near evidence remains insufficient.

Where Comparative Refinement supports a material change to an existing
Transcription Element State, the resulting state transition SHALL preserve the
scientifically material basis and distinctions required by the inherited
scientific principles. The transition MAY retain, extend, refine, revise, or
leave unresolved the applicable source-near content.

Where a persistent Document Matrix is required by the Processing Profile, a
materially changed Transcription Element State SHALL be reflected in the
applicable Matrix Element with sufficient traceability for scientific review.

### 7.7 Iterative Transcription Loop

Transcription Processing MAY iteratively combine assessment, Comparative
Refinement, and applicable Scientific Working Methods defined in Section 6.

Calibration State MAY provide comparison evidence during this Processing but
SHALL NOT directly modify a Transcription Element State. Material changes
supported by calibration SHALL proceed through the applicable assessment and
Comparative Refinement.

A progressed Transcription Element State MAY provide the basis for further
assessment or calibration. New anchors, unresolved forms, later occurrences,
material contradictions, or revised readings MAY cause calibration or
assessment to be re-entered where scientifically applicable.

This iterative process MAY continue until the transcription is scientifically
sufficient for the defined scope or until formal catalogue refinement is
required.

Where formal refinement is required, processing MAY proceed through the Word
Catalogue and, where word-level refinement remains insufficient, the Glyph
Catalogue. This SHALL NOT be interpreted as requiring a universally fixed or
linear method sequence.

### 7.8 Research-Relevant Observation Construction

Scientific Observation Construction SHALL proceed from sufficiently assessed
source-near Transcription Element State through controlled selection of
research-relevant observed information.

Source-near content SHALL NOT be used for Scientific Observation Construction
solely on the basis of an unassessed raw reading or lexical plausibility.
Before such content is used for Scientific Observation Construction, it SHALL
have undergone the assessment applicable to the intended Transcription
Processing and SHALL not be contradicted by observable source-near evidence
that has not been scientifically accounted for.

Unresolved or uncertain source-near content MAY be used for Scientific
Observation Construction where the applicable assessment has been sufficiently
performed and the unresolved or uncertain state is preserved.

The Processing Profile SHALL distinguish:

-   the complete or progressed transcription working state;
-   selected research-relevant information;
-   any temporary review representation; and
-   the resulting Scientific Observation Artifacts.

Scientific Observation Construction SHALL proceed through the following
logical stages:

1.  Research-relevant observed information is selected from sufficiently
    assessed Transcription Element State.
2.  A temporary review representation MAY be constructed where required by the
    Processing Profile.
3.  The selected information and, where used, the temporary review
    representation are reviewed and corrected within the transcription
    boundary.
4.  Conforming Scientific Observations are constructed from the reviewed
    research-relevant information.

Selection SHALL preserve sufficient provenance to trace the resulting
Observation to its transcription basis.

The review SHALL concern faithful selection, representation, provenance, and
remaining uncertainty. It SHALL NOT establish historical truth, source
reliability, person identity, genealogical relationship, or another Research
Processing conclusion.

A Temporary Observation View MAY be constructed from applicable Transcription
Element State where required for the preparation of Scientific Observation
Artifacts.

The Temporary Observation View is a non-persistent Working Representation used
to select, assemble, organize, review, and prepare source-near transcription
content for Observation Construction.

Where information required for the intended Observation is missing from the
current View, applicable source-near content MAY be added from the controlled
Transcription Element State. Content SHALL NOT be added through genealogical
interpretation, normalization, reconstruction, or unsupported inference.

The Temporary Observation View has no independent Scientific Artifact identity,
SHALL NOT serve as a persistent reference target, and MAY be discarded and
regenerated from the applicable Transcription Element State.

### 7.9 Relationship Construction

The Processing Profile SHALL construct all Relationships required by
Section 5 for the resulting Scientific Observation Artifacts.

At least one valid Source–Observation Relationship SHALL connect each Scientific
Observation Artifact to the Registered Source from which it was
produced.

Additional Relationships MAY be constructed only where they remain
within the transcription and provenance responsibilities of this
Execution.

### 7.10 Processing Completeness

Processing completeness SHALL be assessed against the defined
research-relevant transcription scope.

The Processing Profile SHALL NOT require complete transfer of all
Document Matrix content, calibration material, rejected readings, or
temporary working information into Scientific Observation Artifacts.

Processing is complete only when all Scientific Observation Artifacts
and Relationships required by the defined scope have been constructed
and are ready for Validation.

### 7.11 Validation

The Processing Profile SHALL validate the transcription result,
Observation Construction, and required Relationships according to
Section 9.

Validation establishes conformity with this Execution and the applicable
Processing Profile.

It SHALL NOT establish historical truth or final genealogical validity.

### 7.12 Execution Handoff Preparation

After applicable Validation has passed, the Processing Profile SHALL prepare
the resulting Scientific Observation Artifacts and applicable Relationships
as a registration-ready scientific result.

The result SHALL preserve source-derived distinctions, relevant unresolved
uncertainty, source and transcription-basis traceability, validation
information, and execution provenance required for subsequent scientific
processing.

The Transcription Execution SHALL NOT reconcile its resulting Scientific
Observations with potentially corresponding persistent scientific
information.

### 7.13 Execution Handoff Boundary

Completion of Transcription processing SHALL transfer only the validated,
registration-ready scientific result across the Execution Handoff Boundary.

Comparison with potentially corresponding persistent scientific state for
register modification, persistent incorporation, and establishment of a new
Register Revision belong to the applicable register-modification Execution.

A persistence decision SHALL NOT be converted into a scientific
reconciliation decision by this Execution.

### 7.14 Interruption and Recovery

Where the Processing Profile requires persistent transcription working
state, interrupted work SHALL be recoverable from that state without
requiring reconstruction from undocumented tool context.

The recoverable state SHOULD include, where scientifically material:

-   progressed Document Matrix content;
-   unresolved readings;
-   relevant calibration findings;
-   localization and addressing;
-   the state required to continue Observation Construction.

Temporary review or comparison representations need not be persisted
where they can be regenerated without scientific loss.

### 7.15 Processing Profile Completion

A Processing Profile is complete when:

-   the defined transcription scope has been processed;
-   required Scientific Observation Artifacts and applicable Relationships
    have been constructed;
-   applicable Validation has passed;
-   the validated result has been prepared as registration-ready according
    to Section 7.12;
-   the Execution Handoff Boundary defined by Section 7.13 has been reached.

Persistent incorporation and establishment of a Register Revision are not
completion conditions of this Execution.

## 8. Processing Profiles

### 8.1 Purpose

This Section defines the project-retained description requirements for
Scientific Processing Profiles used by this Execution.

A Processing Profile operationalizes the processing architecture defined
by Section 7 for a defined class of transcription tasks.

It SHALL remain subordinate to this Execution and SHALL NOT redefine its
scientific boundaries.

### 8.2 Reference Processing Profile

Appendix A defines the Reference Processing Profiles for this Execution.

A project-specific Processing Profile MAY derive from a Reference
Processing Profile or define an alternative conforming profile.

A project-specific profile SHALL document all deviations or additional
operational rules required to make its processing reproducible.

### 8.3 Processing Profile Description

A Processing Profile description SHALL define at least:

-   profile identifier and purpose;
-   applicable source or source class;
-   transcription scope;
-   selected Scientific Working Methods;
-   method selection and combination rules;
-   permitted iterative or parallel method application;
-   required Working Representations;
-   persistence requirements for transcription working state;
-   segmentation and localization conventions;
-   calibration rules and permitted calibration methods where
    applicable;
-   conditions for formal Word Catalogue or Glyph Catalogue refinement;
-   Observation selection rules;
-   temporary Observation review representation where used;
-   Validation requirements;
-   construction and validation of applicable Source–Observation
    Relationships;
-   registration-ready result and Execution Handoff requirements;
-   interruption and recovery requirements where persistent working
    state is used.

### 8.4 Method and Profile Boundary

A Processing Profile MAY specify when, where, and in what combination a
Scientific Working Method is applied.

It MAY define project-specific notation, visual encodings, segmentation
conventions, or comparison representations where permitted by Section
6.1.3.

It SHALL NOT:

-   redefine the scientific function of a method;
-   weaken uncertainty preservation;
-   treat illustrative notation as mandatory unless the profile
    explicitly adopts it;
-   convert contextual expectation into observed source content;
-   convert a transcriptional comparison into scientific reconciliation;
-   assign Research Processing responsibilities to Transcription.

### 8.5 Persistent Working State

A Processing Profile SHALL explicitly state whether a persistent
transcription working state is required.

Where a persistent Document Matrix AWD is required, the profile SHALL
define sufficient persistence for continuation, review, recovery, and
traceability according to Section 7.4.

Where no persistent working state is required, the profile SHALL still
ensure that the resulting Scientific Observation Artifacts remain
independently reproducible according to this Execution.

### 8.6 Observation Construction

A Processing Profile SHALL define how research-relevant information is
selected from the progressed transcription state and transformed into
Scientific Observation Artifacts.

The profile MAY define a Temporary Observation View according to Section 7.8.

Such a View SHALL remain distinguishable from:

-   the persistent transcription working state;
-   Scientific Observation Artifacts;
-   the AGRAR.

### 8.7 Execution Handoff

A Processing Profile SHALL define how the validated Scientific Observation
Artifacts and applicable Relationships are prepared as a registration-ready
scientific result according to Sections 7.12--7.13.

The Processing Profile SHALL NOT assign comparison with persistent register
state, persistent incorporation, or Register Revision establishment to this
Execution.

### 8.8 Dataset Description Boundary

The Processing Profile description and the Scientific Observation
Artifact dataset description serve different purposes.

The Processing Profile defines how scientific processing is performed.

The dataset description defines the execution-level representation,
persistence, and serialization realization of resulting Scientific
Observations where such a description is required.

The normative scientific meaning of `ScientificObservation` remains
defined by GM Core.

Neither SHALL substitute for the other or for the applicable GM Core
requirements.

### 8.9 Processing Profile Conformity

A Processing Profile conforms to this Execution only where its complete
processing logic preserves:

-   the scientific task defined by Section 1;
-   the method boundaries defined by Section 6;
-   the processing boundaries defined by Section 7;
-   the Observation requirements defined by Section 5;
-   Validation requirements defined by Section 9;
-   Execution Handoff requirements defined by Sections 7.12--7.13 and 10.

## 9. Validation

### 9.1 Purpose

Validation shall establish the scientific conformity of the
transcription result, its construction, and the required execution
outputs.

Validation SHALL NOT establish:

-   historical truth;
-   source reliability;
-   final genealogical validity;
-   person identity;
-   genealogical relationship;
-   resolution of competing scientific claims.

### 9.2 Source Traceability Validation

Validation SHALL confirm that each Scientific Observation Artifact is
traceable to:

-   the applicable Registered Source;
-   the relevant source localization;
-   the transcription basis from which its observed information was
    selected.

Where a persistent Document Matrix is used, the Observation SHALL remain
traceable to the applicable progressed Matrix state or addressable
transcription basis.

### 9.3 Observation Construction Validation

Validation SHALL confirm that:

-   the Observation represents research-relevant information within the
    defined scope;
-   selected information is faithfully represented;
-   sufficient provenance is preserved;
-   structured representational resolution remains within the boundary
    defined by Section 5.7;
-   the Observation does not imply scientific assessment beyond
    transcription;
-   applicable Source–Observation Relationships are present.

Validation SHALL NOT require the Observation to reproduce the complete
transcription working state.

### 9.4 Uncertainty Validation

Validation SHALL confirm that relevant uncertainty remaining after
transcription processing and Observation Construction has not been
silently removed.

Earlier working uncertainty that has been sufficiently resolved through
traceable transcription assessment need not remain represented as
unresolved.

Uncertain, unreadable, damaged, omitted, or incomplete source content
SHALL NOT be silently completed.

### 9.5 No Silent Completion Validation

Validation SHALL confirm that contextual plausibility, known metadata,
formula expectations, constrained vocabularies, same-writer comparison,
or other calibration aids have not been used as substitutes for
observable source evidence.

Such information MAY support candidate generation and assessment
according to Section 6.

It SHALL NOT by itself establish a reading.

### 9.6 Working-State Traceability Validation

Where the applicable Processing Profile requires persistent
transcription working state, Validation SHALL confirm that
scientifically material state required for continuation, review,
recovery, and reproducibility has been preserved as required.

This includes, where applicable:

-   progressed Document Matrix content;
-   relevant unresolved readings;
-   material calibration findings;
-   localization and addressing;
-   traceability of materially changed readings.

Validation SHALL NOT require persistence of temporary aids that can be
regenerated without scientific loss.

### 9.7 Comparative Refinement Validation

Where comparative refinement has been used, Validation SHALL confirm
that:

-   initial independent assessment was performed to the extent
    scientifically practicable where required by Section 7.5;
-   material differences or uncertainty were not concealed;
-   comparative calibration remained within the transcription boundary;
-   material changes remain sufficiently traceable.

### 9.8 Execution Handoff Validation

Validation SHALL confirm that the scientific result prepared for handoff:

-   contains the Scientific Observation Artifacts required by the defined
    scope;
-   contains the applicable Relationships required by this Execution and GM
    Core semantics;
-   preserves relevant uncertainty and source-derived distinctions;
-   preserves required provenance and execution traceability;
-   does not imply that persistent register incorporation or scientific
    reconciliation has occurred.

The term `validated` in this Execution means conforming to the
applicable transcription process and representation requirements.

It SHALL NOT mean that the represented historical content has been
proven true.

## 10. Execution Handoff Boundary

### 10.1 Purpose

The Execution Handoff Boundary separates the scientific result produced and
validated by Transcription from subsequent persistent register modification.

### 10.2 Transcription Responsibility

The Transcription Execution SHALL produce and validate registration-ready
Scientific Observation Artifacts and the applicable Relationships connecting
each Observation to the Registered Source from which it was produced.

The Relationship semantics SHALL conform to the applicable GM Core
Relationship model. Creation and validation of the applicable
Source–Observation Relationship are part of the scientific result of this
Execution.

The handoff result SHALL preserve relevant uncertainty, source-derived
distinctions, provenance, validation information, and execution provenance.

### 10.3 Register-Modification Responsibility

Comparison with potentially corresponding persistent scientific information
for the purpose of register modification, persistent incorporation of the
validated result, and establishment of a new Register Revision belong to the
applicable register-modification Execution.

This Execution SHALL NOT perform those operations.

### 10.4 Scientific Boundary

The Transcription Execution SHALL NOT reconcile its resulting Scientific
Observations with potentially corresponding persistent scientific information
or determine historical truth, source reliability, person identity, event
identity, genealogical relationship, or final scientific preference between
competing claims.

Questions requiring such assessment SHALL remain available for applicable
subsequent scientific processing.

### 10.5 Completion Effect

Successful completion of this Execution establishes a validated,
registration-ready scientific result.

It SHALL NOT by itself establish persistent incorporation, a new Register
Revision, or a reconciled persistent scientific state.

## 11. Execution Conformance

### 11.1 Conformance Principle

An implementation conforms to this Execution only where it preserves the
complete scientific function and boundaries defined by this
specification.

Conformance SHALL be assessed against scientific behavior and
reproducibility rather than against a particular user interface or
illustrative notation.

### 11.2 Required Conformance Properties

A conforming implementation SHALL ensure:

-   traceability from Scientific Observation Artifacts to their
    Registered Source and transcription basis;
-   controlled selection of research-relevant observed information;
-   preservation of relevant remaining uncertainty;
-   no implication that an Observation establishes truth, completeness,
    or final scientific validity;
-   distinguishability of representational resolution from scientific
    interpretation;
-   preservation of persistent transcription working state where
    required by the applicable Processing Profile;
-   documented and reproducible material calibration;
-   no requirement to use formal catalogue refinement merely because
    low-threshold calibration is used;
-   independent initial assessment before comparative refinement to the
    extent scientifically practicable where applicable;
-   distinguishability of temporary review and comparison
    representations from Scientific Artifacts;
-   construction and validation of the applicable Source–Observation
    Relationships as part of the Transcription result;
-   preparation of a validated, registration-ready scientific result;
-   preservation of relevant source-derived distinctions and uncertainty;
-   no persistent register modification or scientific reconciliation within
    Transcription;
-   transfer of Research Processing questions beyond the transcription
    boundary to an applicable subsequent Execution.

### 11.3 Method Implementation Conformance

A conforming implementation MAY use notation, symbols, colors,
segmentation conventions, visual aids, or comparison representations
different from the illustrative examples in Section 6.

Such alternatives conform only where:

-   their meaning is documented;
-   relevant scientific distinctions remain visible;
-   uncertainty remains reproducible;
-   candidate, descriptive, and resolved states remain distinguishable
    where required;
-   source traceability is preserved.

Conformance SHALL NOT require the use of every Scientific Working Method
available in Section 6.

Only methods selected or required by the applicable Processing Profile
need to be implemented for a particular processing task.

### 11.4 Processing Profile Conformance

A project-specific Processing Profile conforms only where it preserves
the Execution task, method boundaries, Observation Construction rules,
Validation requirements, applicable Relationship Construction, and Execution
Handoff requirements.

A Processing Profile SHALL NOT transfer Research Processing
responsibilities into Transcription.

### 11.5 Artifact and Register Conformance

A conforming execution result SHALL contain all Scientific Observation
Artifacts and applicable Relationships required by the defined scope and SHALL
constitute a validated, registration-ready scientific result.

Persistent register modification and establishment of a Register Revision are
outside the completion conditions of this Execution.

Temporary Working Representations SHALL NOT be treated as persistent
Scientific Artifacts unless independently created under an applicable
artifact contract.

### 11.6 Conformance Result

An implementation SHALL be considered conforming only when all
applicable requirements of this Execution and the selected Processing
Profile have been satisfied.

Scientific conformance under this Execution SHALL NOT be represented as
proof of historical truth or final genealogical correctness.

## Appendix A --- Reference Processing Profiles

### A.1 Purpose

This Appendix provides the Reference Processing Profiles defined by
Section 8.2.

The profiles provide specification templates for project-specific
Processing Profiles and demonstrate different practical entries into the
same Transcription Execution architecture.

They SHALL NOT be interpreted as separate Execution architectures or as
universally mandatory method sequences.

### A.2 Tabular Document Transcription

#### A.2.1 Purpose

This Reference Processing Profile applies where the observable source
representation is sufficiently accessible through tabular,
field-oriented, line-oriented, or otherwise structurally localizable
source content.

#### A.2.2 Reference Sequence

The Reference Processing Profile proceeds through the following logical
sequence:

1.  The Registered Source enters Initialization and Source Validation.
2.  The transcription target is defined.
3.  Relevant source content is localized and segmented.
4.  An initial assessment is performed.
5.  A Document Matrix AWD is established as the persistent transcription
    working state.
6.  Transcription Calibration MAY be applied iteratively where required,
    and its results MAY progress the Document Matrix AWD.
7.  Research-relevant observed information is selected from the
    progressed Document Matrix AWD.
8.  A temporary Observation Review Representation MAY be constructed
    where required.
9.  Scientific Observations and required Relationships are constructed.
10. The resulting Scientific Observations and Relationships undergo
    Validation.
11. The validated Scientific Observations and applicable Relationships are
    prepared as a registration-ready scientific result.
12. Successful completion reaches the Execution Handoff Boundary.
13. Persistent register modification, where required, occurs under the
    applicable subsequent register-modification Execution.

#### A.2.3 Persistent Working State

The Document Matrix AWD constitutes the persistent transcription working
state for this Reference Processing Profile.

It SHALL preserve the progressed transcription and scientifically
material calibration state required for continuation, review, and
recovery.

It SHALL NOT constitute a Scientific Artifact merely because it is
persistent.

#### A.2.4 Matrix Construction

The source SHALL be localized and segmented sufficiently for stable
reference to the relevant source content.

The Document Matrix SHOULD preserve:

-   stable source-local addresses;
-   current readings;
-   unresolved or partial readings;
-   omissions or damage where relevant;
-   scientifically material calibration information;
-   sufficient traceability for later Observation Construction.

#### A.2.5 Calibration

Where readings remain uncertain, applicable methods from Section 6 MAY
be used iteratively or in parallel.

Calibration SHALL remain subordinate to observable source form and SHALL
NOT silently replace unresolved source content with contextual
expectation.

#### A.2.6 Observation Construction

Research-relevant observed information SHALL be selected from the
progressed transcription state.

An optional temporary Observation Review Representation MAY be used
before Scientific Observation construction.

The review representation SHALL NOT become a Scientific Artifact merely
through use.

The complete Document Matrix or calibration history need not be
transferred into the resulting Scientific Observations.

#### A.2.7 Validation and Persistence

The resulting Scientific Observations and applicable Relationships SHALL
pass Validation before they are prepared as a registration-ready scientific
result.

Relevant source-derived distinctions and remaining uncertainty SHALL remain
distinguishable.

Successful completion reaches the Execution Handoff Boundary; persistent
register modification belongs to the applicable subsequent Execution.

### A.3 Handwritten Document Transcription

#### A.3.1 Purpose

This Reference Processing Profile applies to handwritten documents for
which plain-text transcription is initially incomplete, difficult, or
dependent on controlled handwriting calibration.

It demonstrates a low-threshold entry into decryption through
constrained hypotheses and observable source comparison, followed by
increasingly source-internal calibration.

It SHALL NOT be interpreted as requiring every handwritten document to
begin with a year, date, formula, number word, or any other particular
anchor.

#### A.3.2 Reference Sequence

The Reference Processing Profile proceeds through the following logical
sequence:

1.  The Registered Source enters Initialization and Source Validation.
2.  The transcription target is defined.
3.  Relevant source content is localized and segmented.
4.  An initial independent assessment SHOULD be performed to the extent
    scientifically practicable.
5.  A Document Matrix AWD is established as the persistent transcription
    working state.
6.  Transcription Calibration MAY be applied iteratively to progress the
    Document Matrix AWD. Applicable calibration methods MAY include:
    -   constrained-value anchors;
    -   formula-assisted candidate generation;
    -   Bracketed Reading;
    -   Descriptive Glyph Calibration;
    -   Number and Formula Anchor Calibration;
    -   Stroke-Pattern Comparison;
    -   Visual Glyph Segmentation;
    -   Same-Writer Comparison;
    -   Small-Window / Overlap Comparison.
7.  Where the progressed Document Matrix is scientifically sufficient
    for the defined scope, processing MAY proceed to research-relevant
    selection. Where it remains insufficient for systematic decryption,
    formal refinement MAY proceed to a Word Catalogue and, where
    word-level refinement remains insufficient, to a Glyph Catalogue.
8.  Research-relevant observed information is selected.
9.  A temporary Observation Review Representation MAY be constructed
    where required.
10. Scientific Observations and required Relationships are constructed
    and validated.
11. The validated result is prepared as registration-ready.
12. Successful completion reaches the Execution Handoff Boundary.
13. Persistent register modification, where required, occurs under the
    applicable subsequent register-modification Execution.

#### A.3.3 Initialization and Known Context

Initialization MAY identify contextual information already known
independently of the reading, including:

-   known or probable year;
-   source-type metadata;
-   expected language;
-   place or repository context;
-   other constrained values relevant to localization or candidate
    generation.

Such information SHALL remain distinguishable from observed source
content.

Known context MAY generate or constrain transcription hypotheses.

It SHALL NOT establish a reading merely because the hypothesized value
would fit the context.

#### A.3.4 Initial Anchor Hypothesis

Where a source contains a visibly corresponding constrained expression,
a known contextual value MAY be used to generate an initial
transcription candidate.

For example, where source metadata independently establishes the year
`1854` and the source appears to contain a written year expression, the
expected written form MAY be treated as a candidate and compared with
the observable glyph sequence.

The candidate SHALL be assessed against the visible source form and MAY
be supported, partially supported, or rejected.

A known year SHALL NOT establish the reading of a written year
expression.

The source MAY express a date numerically or by another form.

The transferable method principle is the use of a constrained anchor
where scientifically applicable, not a requirement to begin with a year.

#### A.3.5 Constrained Word and Formula Comparison

A partially readable word MAY be compared against a scientifically
constrained candidate set.

For example:

-   a suspected month word MAY be compared with the limited vocabulary
    of possible month names;
-   a preceding day-number word MAY be captured descriptively or
    glyphically and compared against plausible number-word candidates;
-   recurring documentary formulas MAY generate candidate readings.

A familiar formula SHALL NOT be used as a textual template to complete
unread source content.

Every formula-assisted candidate remains subject to observable source
form.

Apparent conformity with an expected documentary formula SHALL NOT
establish the document type.

Where the visible source contradicts the expected formula or source
type, the source reading SHALL remain controlling.

#### A.3.6 Number-Word and Glyph Calibration

Once one or more constrained readings have sufficient source support,
the Processing Profile MAY seek further occurrences that strengthen
writer-specific calibration.

Useful occurrences MAY include:

-   date expressions;
-   ages;
-   quantities;
-   recurring number words;
-   recurring formula components;
-   repeated letter or glyph forms.

Resolved local readings MAY increasingly serve as writer-specific
comparison material for unresolved readings elsewhere in the same source
or same-writer corpus.

The calibration process SHOULD therefore shift, where possible, from
externally constrained candidate generation toward source-internal
comparison.

Writer-specific calibration SHALL NOT be generalized into a universal
glyph identity without independent support.

#### A.3.7 Iterative Document Matrix

The Document Matrix AWD constitutes the persistent transcription working
state for this Reference Processing Profile.

Unresolved or partially resolved readings MAY remain represented through
the applicable uncertainty notation or descriptive method.

Examples include:

-   `[unsichere Lesung]`;
-   `[f-artig]`;
-   `[o/u?]`;
-   `[enge n]`.

These examples are illustrative and SHALL NOT establish mandatory
notation.

A field-tested segmented configuration may, for example, use five-line
windows with one repeated boundary line as the continuation and comparison
anchor:

```text
Window 1: Z01-Z05
Window 2: Z05-Z09
Window 3: Z09-Z13
```

This 5+1 configuration is illustrative only. It does not prescribe a
window size, overlap size, or universal segmentation sequence. Other
segment and overlap sizes MAY be used where appropriate to the source and
processing context.

Where a reading becomes sufficiently resolved, the matrix MAY be
progressed by replacing or removing the earlier uncertainty
representation while preserving scientifically material traceability
where required.

Material calibration findings SHALL be documented in the persistent
working state.

A separate solved-word register SHALL NOT be required where the
progressed Document Matrix and its calibration state already preserve
the necessary information.

#### A.3.8 Formal Catalogue Escalation

Where the Document Matrix and ordinary Transcription Calibration remain
insufficient for systematic decryption, the Processing Profile MAY
proceed to a Word Catalogue.

Where word-level refinement remains insufficient, the Processing Profile
MAY proceed further to a Glyph Catalogue.

#### A.3.9 Independent Reading and Comparative Calibration

Relevant repeated or mutually informative source segments SHOULD first
be assessed independently to the extent scientifically practicable.

Subsequent comparison MAY refine the readings through same-writer
evidence, stroke-pattern comparison, visual segmentation, or another
applicable method.

Comparison SHALL NOT silently replace an independently recorded reading
or conceal material uncertainty or disagreement.

Small source windows MAY be used for focused comparison provided that
sufficient overlap or localization is retained to preserve source
context and reproducibility.

#### A.3.10 Observation Construction

Scientific Observation Construction SHALL select research-relevant
observed information from the progressed transcription state.

An optional temporary Observation Review Representation MAY summarize
the selected information before persistence.

Review MAY assess:

-   faithful transfer from the transcription basis;
-   representation;
-   provenance;
-   remaining uncertainty;
-   whether structured representational resolution remains within the
    transcription boundary.

Review SHALL NOT determine:

-   historical truth;
-   source reliability;
-   true document type beyond what the source itself supports;
-   person identity;
-   genealogical relationships;
-   competing genealogical claims.

The complete handwriting calibration history need not be transferred
into the resulting Scientific Observations.

#### A.3.11 Validation and Update

The resulting Scientific Observations and applicable Relationships SHALL
pass Validation according to Section 9.

The validated result SHALL then be prepared as registration-ready according
to Sections 7.12--7.13 and the Execution Handoff Boundary in Section 10.

Scientific reconciliation and persistent register modification remain outside
this Execution.

Successful completion reaches the Execution Handoff Boundary.

### A.4 Reference Profile Interpretation

The two Reference Processing Profiles illustrate different practical
entry conditions into the same Execution architecture:

-   A.2 Tabular Document Transcription uses observable source structure
    as its primary practical entry.
-   A.3 Handwritten Document Transcription MAY use constrained
    hypotheses for initial candidate generation. Candidate acceptance
    remains controlled by observable source comparison, while subsequent
    source-internal calibration MAY progressively strengthen the
    reading.

Both profiles remain governed by the same Scientific Working Methods and
the same Execution architecture.

Neither profile establishes a universal method sequence.
