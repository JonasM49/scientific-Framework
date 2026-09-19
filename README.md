# scientific-Framework

Scientific Framework for structured, traceable and collaborative
scientific work with AI.

The repository contains the **General Scientific Layer (GSL)** and the
depending **Genealogy Model (GM)**. The Genealogy Model specializes the
general scientific architecture for genealogical research and provides
concrete **GM Executions** for defined scientific tasks.

The GSL is intended to provide a **domain-independent scientific
foundation**; GM is its first domain-specific specialization. The
framework is currently validated primarily through genealogical
research. Future specialization of the GSL into other domain models
would provide an important test of whether its architecture is
sufficiently general and domain-independent.

The framework is designed around explicit scientific responsibilities,
traceable artifacts and relationships, controlled human--AI
collaboration, and graph-based research structures.

## Architecture

``` text
General Scientific Layer (GSL)
        ↓
Genealogy Model Core (GM Core)
        ↓
GM Executions
```

### 1 --- General Scientific Layer

[`1-GSL/`](1-GSL/)

The GSL defines the general scientific principles and architecture used
by the framework. It provides the normative foundation for scientific
working context, evidence and knowledge handling, traceability,
uncertainty, human--AI collaboration, and controlled scientific
evolution.

The GSL is intended to support future domain models that do not inherit
from GM Core. Such non-genealogical specialization is a future
validation path, not a currently demonstrated field-test result.

Current baseline:

-   [`GSL-v2.0.md`](1-GSL/GSL-v2.0.md)

### 2 --- Genealogy Model Core

[`2-GM-Core/`](2-GM-Core/)

GM Core specializes the GSL for genealogical research. It defines the
common genealogical scientific architecture, including artifacts,
relationships, project context, processing boundaries, and the interface
between GM Core and GM Executions.

Current baseline:

-   [`GM-Core-v1.3_Baseline.md`](2-GM-Core/GM-Core-v1.3_Baseline.md)

### 3 --- GM Executions

[`3-GM-Exec/`](3-GM-Exec/)

GM Executions define controlled processing for specific genealogical
scientific tasks. They inherit from GSL and GM Core and specialize only
the execution-specific scientific responsibilities required for their
task.

Published Executions currently include:

-   [`GM-Exec_Person_Identity_Research_v2.3_Baseline.md`](3-GM-Exec/GM-Exec_Person_Identity_Research_v2.3_Baseline.md)
    --- Baseline
-   [`GM-Exec_Source_Registration-v1.2_Candidate.md`](3-GM-Exec/GM-Exec_Source_Registration-v1.2_Candidate.md)
    --- Candidate
-   [`GM-Exec_Transcription-v1.2_Baseline.md`](3-GM-Exec/GM-Exec_Transcription-v1.2_Baseline.md)
    --- Baseline

## GM Execution Development

The **GM-Exec Specification Development Template** supports the
controlled development of additional GM Executions.

It is a development aid and **is not an additional normative layer**. A
GM Execution developed with the template inherits normatively from GSL
and GM Core.

Recommended repository location:

-   `3-GM-Exec/Template/GM-Exec_Specification_Development_Template_v1.1_Baseline.md`

## Intended use

The framework is intended to be usable directly with a capable Large
Language Model (LLM), such as ChatGPT:

1.  Load the applicable framework files into the LLM --- GSL, GM Core,
    and the GM Execution required for the research task.
2.  Provide the research material and define the research objective and
    applicable project context.
3.  Begin the research collaboratively within the scientific and
    execution boundaries defined by the loaded specifications.
4.  Preserve validated results in the project's persistent research
    structure so that later work can continue from an explicit
    scientific state.

The specifications are designed to provide the LLM with a structured
scientific working context rather than relying only on conversational
instructions.

## Key characteristics

### Scientific working

The framework is designed for scientific work with explicit provenance,
traceability, uncertainty, validation, and controlled human--AI
collaboration. Scientific responsibilities are assigned to defined
architectural owners instead of being left implicit in the conversation.

### Separation of observation and research

Source-near observation is kept distinct from subsequent interpretation,
correlation, hypothesis formation, identity research, and other research
activities. This helps preserve what was actually observed in a source
while allowing later conclusions to remain reviewable and revisable.

### Graph-based data structure

Research knowledge is represented through scientific artifacts and
explicit relationships between them. This graph-oriented structure
allows persons, events, information, sources, observations, and other
research elements to remain individually addressable while their
scientific context is preserved through relationships.

### Persistent results

Validated scientific results can be preserved as persistent project
state rather than existing only in the LLM conversation. Persistent
artifacts, relationships, provenance, and authoritative register states
provide a basis for continuing research across sessions, tools, and
processing steps.

## Scientific design principles

The framework separates general scientific responsibilities from
genealogy-specific semantics and execution-specific procedures.

A central architectural rule is **Single Owner**: each normative
scientific responsibility has exactly one normative owner. Other
architectural elements reference or inherit that responsibility instead
of redefining it.

The framework also follows the development principle **"Normiere --
entwickle nicht neu."** Established scientific or technical concepts are
reused where they adequately satisfy the scientific requirement; the
framework specifies the conditions for their scientific use instead of
independently redefining them.

## Public field test and feedback

This publication is intended as a **public field test** of the
framework.

The current architecture has been developed and repeatedly tested
through practical genealogical research. Publication is intended to
extend that evaluation to other researchers, source types, research
questions, workflows, and tool environments.

Feedback is especially valuable when it identifies a concrete scientific
or architectural problem rather than only proposing a textual change.

Where possible, feedback should therefore be submitted as a **qualified
issue** describing:

-   the concrete research use case or source context;
-   the observed problem or limitation;
-   the affected framework layer or specification, if identifiable;
-   the current behavior or applicable rule;
-   the expected scientific requirement;
-   evidence or a reproducible example;
-   whether the issue appears to require clarification, specialization,
    correction, or a specification change.

For proposed normative changes, contributors are encouraged to formulate
the issue in terms compatible with the **Scientific Change Proposal
(SCP)** concepts defined by the GSL. This makes the scientific
motivation, affected responsibility, evidence, and proposed change
assessable before implementation.

A Pull Request may then implement an already understood and assessable
change. A Pull Request alone is not a substitute for describing the
scientific problem that motivates a normative change.

This distinction is intentional:

``` text
Research experience
        ↓
Qualified issue / evidence
        ↓
Scientific assessment
        ↓
SCP where a normative change is required
        ↓
Controlled specification evolution
        ↓
Implementation / Pull Request where appropriate
```

Reports showing that the framework works without modification in a new
use case are also valuable field-test evidence.

## Contribution and independent development

The framework supports both a central contribution path and independent
experimentation.

``` text
Central contribution path

Field test
    ↓
Qualified issue / evidence
    ↓
Scientific assessment
    ↓
SCP where required
    ↓
Controlled integration
```

Contributors can report findings to the central repository for
assessment against the current GSL, GM Core, and applicable GM
Execution. This provides a common place for evaluating whether an
observed problem requires clarification, specialization, correction, or
normative evolution.

``` text
Independent development path

Repository
    ↓
Fork
    ↓
Adaptation / independent field test
    ↓
Findings
    ↓
optional contribution back to the central project
```

A fork may explore another application, adaptation, or development path
independently. Findings from such work can later be contributed back as
qualified issues, evidence, SCP input, or implementation proposals where
appropriate.

The central repository therefore provides a controlled reference lineage
without preventing independent scientific experimentation.

## Status

This repository is under active development. Documents explicitly marked
**Baseline** represent released reference states. Documents marked
**Candidate** are publication candidates still subject to their
controlled validation and promotion process.

## License

This project is licensed under the Creative Commons
Attribution-NonCommercial-ShareAlike 4.0 International
(CC BY-NC-SA 4.0) license.

See `LICENSE` for the full license terms.
