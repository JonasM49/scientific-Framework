# Genealogy Model (GM)

STATUS: Baseline

VERSION: 1.3

DOCUMENT_IDENTIFIER: GM-Core

DOCUMENT_TYPE: NormativeSpecification

DEPENDS_ON: GSL-2.0

LANGUAGE: DSL SPECIFICATION_LINEAGE

AUTHOR: JonasM49

PUBLISHED_AT: 2026-09-19

CANONICAL_REPOSITORY: https://github.com/JonasM49/scientific-Framework

LICENSE: CC-BY-NC-SA-4.0

------------------------------------------------------------------------

## 1 GM Core Foundations and Project Binding

### 1.1 General Artifact Model Binding

PURPOSE

DefineHowTheGenealogyModelSpecializesTheGeneralScientificArtifactModelDefinedByTheGeneralScientificLayer.

RULE

The Genealogy Model SHALL adopt the General Scientific Artifact Model
defined by the General Scientific Layer.

RULE

The Genealogy Model SHALL specialize Scientific Artifact types only by
adding genealogy-specific semantics.

RULE

The Genealogy Model SHALL NOT redefine identity, lifecycle, provenance,
metadata, integrity or traceability requirements already defined by the
General Scientific Layer.

RULE

Whenever a genealogy-specific concept can be represented by
specialization of the General Scientific Artifact Model, specialization
SHALL be preferred over independent definition.

PRINCIPLE

EstablishedConceptReuse

RULE

Where an established scientific or technical concept adequately
satisfies a Genealogy Model requirement, the Genealogy Model SHALL
prefer specification of the genealogy-specific conditions governing
its scientific use over independent redefinition of that concept.

### 1.2 Authoritative Working Lifecycle Binding

PURPOSE

DefineHowGenealogyModelArtifactsAdoptTheAuthoritativeWorkingElementLifecycleDefinedByTheGeneralScientificLayer.

CONFORMS_TO

GSL.AuthoritativeWorkingElement

RULE

A Genealogy Model artifact that requires controlled iterative
development SHALL conform to the Authoritative Working Element model
defined by the General Scientific Layer.

RULE

The Genealogy Model SHALL inherit AWE generation, predecessor lineage,
validation, authority transfer, recovery and persistence requirements
without independent redefinition.

RULE

Genealogy-specific AWE specializations SHALL add only domain-specific
validation, content-integrity or persistence constraints.

RULE

A failed transformation SHALL preserve the last verified authoritative
GM artifact state.

RULE

Authority SHALL transfer to a successor GM artifact only after the
successor has been completely persisted and successfully verified.

RULE

Artifact lifecycle state, artifact version and AWE generation SHALL
remain distinguishable.

#### 1.2.1 AWE Applicability For GM Artifacts

PURPOSE

IdentifyWhichGenealogyModelArtifactsRequireAuthoritativeWorkingElementConformance.

AWE_REQUIRED_FOR

ProjectScientificSpecificationWorkingDraft
AuthoritativeGenealogicalResearchArtifactRegister
IterativelyDevelopedGenealogicalResearchArtifact

AWE_CONDITIONAL_FOR

DerivedExportWorkingArtifact ReferenceImplementationWorkingArtifact
ValidationArtifactUnderIterativeRevision

AWE_NOT_REQUIRED_BY_DEFAULT_FOR

FrozenReleasedSpecification ImmutableSourceArtifact
LossyPresentationExport ReadOnlyReferenceArtifact

RULE

A GM artifact SHALL conform to the Authoritative Working Element model
when it is developed through controlled iterative transformation and one
current authoritative state must be preserved.

RULE

The Authoritative Genealogical Research Artifact Register SHALL conform
to AWE because it represents the authoritative persistent research
state.

RULE

The Authoritative Genealogical Research Artifact Register SHALL be a
Core-defined scientific model.

RULE

Its operational realization SHALL be defined by the applicable
Processing architecture.

RULE

A Project Scientific Specification under active revision SHALL conform
to AWE.

RULE

Immutable source artifacts SHALL preserve provenance and integrity but
SHALL NOT be converted into AWE working states merely because they are
referenced by a project.

RULE

Derived exports SHOULD conform to AWE only when the export itself is
iteratively developed as an authoritative working artifact.

#### 1.2.2 Genealogy Specific AWE Validation Requirements

PURPOSE

DefineGenealogySpecificValidationRequirementsAppliedInAdditionToTheGeneralScientificLayerAWEModel.

VALIDATION_REQUIREMENTS

GenealogicalTraceability SourceEvidenceCompleteness
RelationshipConsistency IdentityResolutionConsistency
GenealogicalUncertaintyIntegrity ProcessingProfileConformance

RULE

Every authoritative Authoritative Genealogical Research Artifact
Register SHALL preserve complete traceability from every asserted
research statement to its supporting Scientific Artifacts.

RULE

Authority SHALL NOT be transferred when unresolved identity conflicts
would materially alter the scientific interpretation.

RULE

Every authoritative genealogy artifact SHALL preserve explicit
uncertainty representations across all AWE generations.

RULE

Genealogy-specific validation SHALL extend, but SHALL NOT replace or
weaken, the validation requirements inherited from the General
Scientific Layer.

### 1.3 Scientific Evolution Architecture Binding

PURPOSE

DefineHowTheGenealogyModelAdoptsTheScientificEvolutionArchitectureDefinedByTheGeneralScientificLayer.

CONFORMS_TO

GSL.ScientificEvolutionArchitecture

RULE

The Genealogy Model SHALL adopt the Scientific Evolution Architecture
defined by the General Scientific Layer.

RULE

The Genealogy Model SHALL use the General Scientific Layer candidate
lifecycle for all normative specification development.

RULE

The Genealogy Model SHALL NOT redefine candidate management, review,
integration, consolidation, publication or archival processes already
defined by the General Scientific Layer.

RULE

Genealogy-specific evolution requirements SHALL extend only the
scientific content under review and SHALL NOT modify the inherited
evolution process.

RULE

Every normative Genealogy Model change SHALL remain traceable through
the inherited Scientific Evolution Architecture.

INHERITED_EVOLUTION_PROCESSES

SpecificationCandidateManagement CandidateLifecycle ReviewAndResolution
ArchitectureIntegrationReview ControlledConsolidation EditorialCleanup
EvidenceBasedValidation ReleaseBoundArchival ControlledArtifactTransfer

RULE

The Genealogy Model SHALL reference the inherited evolution processes
and SHALL NOT define competing GM-specific equivalents.

RULE

Genealogy-specific reviews MAY define domain-specific review criteria,
but their lifecycle, authority and archival handling SHALL remain
governed by the General Scientific Layer.

#### 1.3.1 Genealogy Specific Evolution Review Criteria

PURPOSE

DefineGenealogySpecificReviewCriteriaAppliedWithinTheInheritedScientificEvolutionArchitecture.

REVIEW_CRITERIA

GenealogicalMethodConsistency SourceModelConsistency
ArtifactSpecializationConsistency ProjectProfileConsistency
ResearchRecordSetIntegrity ExportModelConsistency

RULE

Genealogy-specific reviews SHALL evaluate only genealogy-specific
scientific content.

RULE

General Scientific Layer process conformance SHALL be assumed through
inheritance and SHALL NOT be revalidated by Genealogy Model reviews.

RULE

Every genealogy-specific review finding SHOULD identify the affected
Genealogy Model artifact, inherited General Scientific Layer concept and
proposed genealogy-specific resolution.

RULE

A Genealogy Model review SHALL distinguish between General Scientific
Layer conformance findings and genealogy-specific modeling findings.

### 1.4 Scientific Working Context Binding

PURPOSE

DefineHowTheGenealogyModelAdoptsTheScientificWorkingContextDefinedByTheGeneralScientificLayer.

CONFORMS_TO

GSL.ScientificWorkingContext

RULE

The Genealogy Model SHALL adopt the Scientific Working Context defined
by the General Scientific Layer.

RULE

The Genealogy Model SHALL inherit the Human Role Profile, AI Role
Profile and Collaboration Model without independent redefinition.

RULE

The Genealogy Model SHALL define only genealogy-specific working
guidance that extends the inherited Scientific Working Context.

RULE

Genealogy-specific working guidance SHALL NOT redefine authority,
responsibilities or interaction principles already defined by the
General Scientific Layer.

RULE

Every genealogy-specific working recommendation SHALL remain traceable
to the inherited Scientific Working Context.

INHERITED_WORKING_CONTEXT

HumanRoleProfile AIRoleProfile CollaborationModel InteractionPrinciples
ScientificResponsibilities

RULE

The Genealogy Model SHALL reference inherited working context concepts
and SHALL NOT define GM-specific equivalents for roles, collaboration or
authority.

RULE

The Genealogy Model MAY define genealogy-specific working
recommendations only where they extend genealogical research practice.

#### 1.4.0 Genealogy Specific Professional Operating Context

PURPOSE

SpecializeTheInheritedScientificAIRoleForGenealogicalScientificWorkWithoutCreatingIndependentAuthority.

RULE

Unless explicitly specialized or overridden by the applicable project
profile, the AI SHOULD operate with the professional perspective, methods,
source awareness and research heuristics expected of an experienced
genealogical researcher.

RULE

The genealogy-specific AI professional role SHALL specialize, but SHALL NOT
replace, the scientific AI role and Human--AI collaboration requirements
inherited from the General Scientific Layer.

RULE

A project profile MAY further specialize or explicitly override the
genealogy-specific professional role. Any such specialization or override
SHALL preserve all applicable inherited scientific requirements.

RULE

The genealogy-specific professional operating context SHALL apply during
project initialization as well as during subsequent genealogical scientific
processing.

RULE

Where GSL and GM Core are jointly applicable, initialization SHALL be
interpreted through the genealogy-specific professional operating context
rather than through an unspecialized general analytical role.

RULE

This specialization SHALL guide recognition of genealogically relevant
context and materially undefined parameters but SHALL NOT independently
establish a ResearchObjective, SourceDomainSelection, scientific conclusion
or operational authorization.

RULE

Where GSL and GM are applicable as the governing scientific framework for a
genealogical project, their availability SHALL by itself establish neither a
framework-development objective nor a specification-review task.

RULE

The genealogy-specific professional operating context SHALL apply the
governing framework to the genealogical research context rather than treat
the framework itself as the object of scientific or technical development.

RULE

Framework development, specification review or normative revision SHALL
require an explicitly established applicable development or review context.

#### 1.4.1 Genealogy Specific Working Guidance

PURPOSE

DefineGenealogySpecificWorkingRecommendationsExtendingTheInheritedScientificWorkingContext.

WORKING_GUIDANCE

EvidenceFirstResearch SourceBeforeInterpretation
ProgressiveHypothesisValidation ControlledIdentityResolution
ExplicitUncertaintyDocumentation AuthoritativeResearchPersistence
StructuredInteractionBoundary

RULE

Genealogical research SHOULD prioritize evidence collection before
interpretation.

RULE

Every interpretation SHOULD remain explicitly linked to supporting
scientific artifacts.

RULE

Identity resolution SHOULD be performed progressively and revised only
through evidence-based validation.

RULE

Genealogical uncertainty SHOULD remain explicitly documented until
resolved by sufficient evidence.

RULE

The authoritative Authoritative Genealogical Research Artifact Register
SHOULD remain the primary persistent representation of ongoing research.

RULE

Where scientific work extends across multiple interaction cycles, each
completed working block SHOULD provide a clear interaction boundary
before the next human prompt.

RULE

Where appropriate, the interaction boundary SHOULD be formed by a
concise and concrete question that closes the current working block and
exposes a meaningful point from which the human participant may
continue, correct, interrupt or reprioritize the scientific work.

RULE

An interaction-boundary question SHALL NOT by itself constitute a new
scientific decision and SHALL NOT replace clarification or human
decision where a material scientific parameter, conflict or decision
remains unresolved.

RULE

Where an established Scientific Working Context contains a sufficiently
defined current work scope and no material parameter requires clarification,
a semantically sufficient continuation acknowledgement MAY continue that
existing work scope.

RULE

An interaction boundary intended to permit such continuation SHALL be
presented in a form that makes the applicable decision, completed work state
or continuation option recognizable to the human participant.

RULE

A continuation acknowledgement SHALL be interpreted in relation to that
recognizable interaction boundary and SHALL NOT by itself constitute a new
scientific decision, changed work scope or new authorization.

RULE

A change of Research Focus within an established ResearchObjective SHALL NOT
by itself constitute a change of ResearchObjective.

### 1.5 Project Model Adaptation Binding

PURPOSE

DefineHowTheGenealogyModelAdoptsTheProjectModelAdaptationDefinedByTheGeneralScientificLayer.

CONFORMS_TO

GSL.ProjectModelAdaptation

RULE

The Genealogy Model SHALL adopt the Project Model Adaptation defined by
the General Scientific Layer.

RULE

The Genealogy Model SHALL inherit the General Scientific Layer project
adaptation architecture without independent redefinition.

RULE

The Genealogy Model SHALL define only genealogy-specific project
adaptation guidance.

RULE

Genealogy-specific project adaptations SHALL specialize the inherited
General Scientific Layer project adaptation model and SHALL NOT replace
or weaken it.

RULE

Every Genealogy Model project profile SHALL remain traceable to the
inherited Project Model Adaptation.

### 1.6 Controlled Artifact Transfer Binding

PURPOSE

DefineHowTheGenealogyModelAdoptsTheControlledArtifactTransferDefinedByTheGeneralScientificLayer.

CONFORMS_TO

GSL.ControlledArtifactTransfer

RULE

The Genealogy Model SHALL adopt the Controlled Artifact Transfer
architecture defined by the General Scientific Layer.

RULE

The Genealogy Model SHALL inherit the General Scientific Layer transfer
process, transfer authority and transfer traceability requirements
without independent redefinition.

RULE

The Genealogy Model SHALL define only genealogy-specific transfer
guidance.

RULE

Genealogy-specific transfer definitions SHALL specialize the inherited
Controlled Artifact Transfer model and SHALL NOT replace or weaken it.

RULE

Every genealogy-specific artifact transfer SHALL preserve traceability
to the originating authoritative Scientific Artifact.

INHERITED_TRANSFER_MODEL

GSL.ControlledArtifactTransfer GSL.TransferAuthority
GSL.TransferTraceability GSL.TransferIntegrity GSL.TransferValidation
GSL.TransferClassification GSL.TransferProvenance

RULE

The Genealogy Model SHALL reference the inherited Controlled Artifact
Transfer model and SHALL NOT define GM-specific equivalents for general
transfer processes, authority, provenance, integrity or validation.

### 1.7 Genealogy Specific Artifact Transfer Guidance

PURPOSE

DefineGenealogySpecificRequirementsForControlledTransferOfGenealogicalResearchArtifacts.

TRANSFER_GUIDANCE

AuthoritativeGenealogicalResearchArtifactRegisterTransfer
GenealogicalSourceArtifactTransfer
GenealogicalRelationshipArtifactTransfer
GenealogicalEventArtifactTransfer GenealogicalExportProfiles
GenealogicalTransferConstraints

RULE

An Authoritative Genealogical Research Artifact Register SHALL remain
the authoritative research representation after every controlled
transfer.

RULE

Every transferred genealogical artifact SHALL preserve complete
traceability to the originating Scientific Artifacts and supporting
evidence.

RULE

Transfers between genealogy-specific artifact types SHALL preserve
identity resolution, relationship consistency and explicit uncertainty
representation.

RULE

Genealogy-specific export profiles SHALL explicitly declare whether the
resulting representation is lossless, lossy or non-authoritative.

RULE

Lossy genealogy-specific transfers SHALL explicitly identify which
scientific information cannot be represented in the target format.

RULE

A genealogy-specific transfer SHOULD preserve every reusable scientific
relationship whenever the target representation supports it.

RULE

Transfer-specific transformations SHALL remain reproducible through
documented Processing Profiles.

RULE

A genealogy-specific transfer SHALL NOT silently modify genealogical
evidence, relationships, identity assignments or uncertainty states.

### 1.8 Scientific Artifact Lifecycle Binding

PURPOSE

DefineHowTheGenealogyModelAdoptsTheScientificArtifactLifecycleDefinedByTheGeneralScientificLayer.

CONFORMS_TO

GSL.ScientificArtifactLifecycle

INHERITS

GSL.ArtifactLifecycleState GSL.ArtifactLifecycleTransition

RULE

The Genealogy Model SHALL use the Scientific Artifact Lifecycle defined
by the General Scientific Layer.

RULE

The Genealogy Model SHALL NOT redefine general artifact lifecycle states
or transitions.

RULE

Genealogy-specific artifact types MAY define additional lifecycle
constraints only where required by genealogical scientific content.

RULE

Genealogy-specific lifecycle constraints SHALL remain compatible with
the inherited Scientific Artifact Lifecycle.

RULE

Artifact type, lifecycle state, artifact version and AWE generation
SHALL remain distinguishable.

INHERITED_LIFECYCLE_MODEL

GSL.ScientificArtifactLifecycle GSL.ArtifactLifecycleState
GSL.ArtifactLifecycleTransition GSL.AuthoritativeWorkingElementLifecycle

RULE

The Genealogy Model SHALL reference the inherited lifecycle model and
SHALL NOT define GM-specific equivalents for general artifact states,
transitions, promotion, supersession or archival.

RULE

Genealogy-specific artifact status terms SHALL describe domain content
or validation state and SHALL NOT act as replacements for inherited
lifecycle states.

#### 1.8.1 Genealogy Specific Lifecycle Constraints

PURPOSE

DefineGenealogySpecificConstraintsAppliedInAdditionToTheInheritedScientificArtifactLifecycle.

LIFECYCLE_CONSTRAINTS

SourceTraceabilityPreservation EvidenceStatePreservation
IdentityResolutionPreservation RelationshipConsistencyPreservation
UncertaintyStatePreservation RegisterMembershipConsistency

RULE

A Genealogical Research Artifact SHALL preserve source traceability
across every inherited lifecycle transition.

RULE

A lifecycle transition SHALL NOT silently remove or weaken documented
evidence states.

RULE

A lifecycle transition affecting a PersonIdentity SHALL preserve prior
identity-resolution decisions and their supporting evidence.

RULE

A lifecycle transition affecting genealogical Relationships or Events
SHALL preserve genealogical relationship consistency.

RULE

Explicit uncertainty states SHALL remain preserved until they are
resolved through documented scientific validation.

RULE

An artifact entering or leaving the authoritative Genealogical Research
Artifact Register SHALL do so through a controlled lifecycle transition.

RULE

A genealogy-specific lifecycle constraint SHALL extend, but SHALL NOT
replace or weaken, the inherited Scientific Artifact Lifecycle.

### 1.9 Semantic Specialization Binding

PURPOSE

DefineHowTheGenealogyModelAddsGenealogicalSemanticOrientationWithoutIntroducingAlternativeCoreArtifactArchitectures.

DESCRIPTION

The General Scientific Layer defines the applicable General Scientific
Artifact requirements.

The Genealogy Model preserves those requirements and adds only the
minimum genealogy-specific semantic reference sets and Processing
extension boundaries required for genealogical research.

Genealogy-specific Artifact Types SHALL be semantic specializations of
the uniform Scientific Artifact architecture and SHALL NOT establish
separate structural inheritance hierarchies within the Core.

RULE

Every Genealogy Model Scientific Artifact SHALL conform to all
applicable General Scientific Layer requirements.

RULE

Genealogy-specific semantic reference types SHALL define only domain
meaning and SHALL NOT redefine the uniform Scientific Artifact
architecture.

RULE

Type-specific formation, constraints, interpretation and operational
behavior SHALL be defined by the applicable Processing architecture.

RULE

Processing and project-specific specializations SHALL preserve semantic
compatibility with their referenced Core meaning.

RULE

No semantic specialization MAY remove, replace or weaken inherited
scientific requirements.

RULE

Every Processing or project-specific specialization SHALL preserve
traceability to its referenced semantic type and applicable Processing
definition.

### 1.10 Architecture Axes

PURPOSE

SeparateLayerTypeAndLifecycleAsIndependentArchitecturalDimensions.

ARCHITECTURE_AXIS

Layer

VALUES

GeneralScientificLayer

GenealogyModel

Project

ARCHITECTURE_AXIS

Type

VALUES

BaseType

DomainType

ProjectType

ARCHITECTURE_AXIS

Lifecycle

VALUES

DefinedByGeneralScientificLayer

RULE

Layer, type and lifecycle SHALL be modeled as independent dimensions.

RULE

Type inheritance SHALL NOT be used to represent lifecycle transitions.

### 1.11 Foundational Principles

PRINCIPLE

SourceCenteredResearch

PRINCIPLE

ScientificProcessingBeforeInterpretation

PRINCIPLE

EvidenceBeforeReconstruction

PRINCIPLE

SeparationOfEvidenceAndInterpretation

PRINCIPLE

ValidatedScientificArtifacts

PRINCIPLE

IdentityResolutionFromMultipleIndependentSources

PRINCIPLE

ProjectContextAwareness

PRINCIPLE

ProgressiveScientificRefinement

PRINCIPLE

ObservationBeforeArtifactFormation

PRINCIPLE

ArtifactCenteredScientificPersistence

PRINCIPLE

ExplicitScientificRelationships

PRINCIPLE

ScientificClusterComposition

------------------------------------------------------------------------

### 1.12 Architecture Overview

PURPOSE

ProvideAHighLevelOverviewOfTheCurrentGMCoreArchitectureWithoutChangingNormativeSemantics.

ARCHITECTURE_FLOW

Source ScientificObservationArtifact DerivedScientificArtifact
ScientificRelationship ScientificCluster
AuthoritativeGenealogicalResearchArtifactRegister PresentationView

RULE

The Architecture Overview SHALL describe the current GM Core
architecture only.

RULE

Detailed normative semantics SHALL be defined in their respective
sections of this specification.

------------------------------------------------------------------------

### 1.13 Project Initialization

PURPOSE

DefineTheMinimumProjectInitializationRequiredToBeginGenealogicalScientificWork.

CONFORMS_TO

GSL.ScientificWorkingContext GSL.ProjectModelAdaptation

DESCRIPTION

The Project Scientific Specification is progressively refined as
additional project-specific information becomes available during
scientific work.

RULE

The Genealogy Model SHOULD request only the minimum project-specific
information required to begin scientific work.

RULE

A formal Project Scientific Specification SHALL NOT be required before
scientific work can begin.

RULE

The initial project definition SHALL contain:

ResearchDomain ResearchObjective

RULE

The Project Scientific Specification SHALL support progressive
refinement throughout the scientific lifecycle.

RULE

Progressive Project Initialization SHALL preserve scientific
traceability, reproducibility and Authoritative Working Element
management throughout the complete scientific lifecycle.

### 1.14 Transition To Scientific Working Mode

PURPOSE

DefineTheGenealogySpecificTransitionFromProjectInitializationToControlledScientificProcessing.

CONFORMS_TO

GSL.ScientificWorkingContext

GSL.ProjectModelAdaptation

#### 1.14.1 Transition Trigger

PURPOSE

DefineTheNormativeTriggerForEnteringTheScientificObservationModel.

RULE

The transition to the Scientific Observation Model SHALL occur when the
first scientific input enters controlled scientific processing.

RULE

From this point onward all scientific activities SHALL conform to the
applicable Processing Profile.

#### 1.14.2 Transition Result

PURPOSE

DefineTheArchitecturalStateAfterSuccessfulTransition.

RESULT

ScientificObservationModelActive

ProcessingProfileControlled

ProjectInitializationCompleted

RULE

Scientific work SHALL continue under the Scientific Observation Model.

RULE

Project initialization SHALL thereafter support scientific work but
SHALL no longer govern it.

ACTIVE_PART

ProjectScientificSpecification

PURPOSE

SpecializeTheInheritedProjectScientificSpecificationForGenealogicalResearch.

SPECIFICATION_TYPE

ProjectScientificSpecification

SPECIALIZES

GSL.ProjectScientificSpecification

INHERITED_PROJECT_MODEL

ProjectIdentity ResearchDefinition ProjectConfiguration
ProjectExtensions ConfigurationExtensionBoundary
ProjectGovernanceBinding ProjectModelAdaptation ScientificWorkingContext

RULE

The Genealogy Model SHALL NOT redefine the inherited general project
model.

RULE

A genealogical Project Scientific Specification SHALL preserve
conformance with the inherited General Scientific Layer project model.

### 1.15 Genealogy Project Binding

PURPOSE

DefineTheGenealogyModelSpecificBindingOfAProjectScientificSpecification.

REQUIRED_FIELDS

AppliedGenealogyModelVersion

RULE

Every genealogical Project Scientific Specification SHALL identify the
applied Genealogy Model version.

RULE

The applied Genealogy Model version SHALL remain traceable across all
project versions.

### 1.16 Genealogy Project Knowledge Inputs

PURPOSE

DefineGenealogySpecificClassesOfProjectKnowledgeEnteringControlledScientificProcessing.

GENEALOGY_SPECIFIC_KNOWLEDGE_CLASSES

GenealogicalSourceMaterial ImportedGenealogicalData
ReferencedGenealogicalResearch LegacyGenealogicalDatabase

RULE

Imported genealogical knowledge SHALL preserve its original provenance.

RULE

Standardized external genealogical formats SHOULD enter the scientific
workflow through documented Processing Profiles.

RULE

Technical conformance of imported genealogical data SHALL be evaluated
separately from the scientific validity of its content.

### 1.17 Genealogy Project Configuration

PURPOSE

DefineTheSelectionOfGenealogyModelComponentsForAConcreteProject.

GENEALOGY_SPECIFIC_CONFIGURATION_ELEMENTS

ActivatedProcessingProfiles ActivatedGenealogicalArtifactTypes
ActivatedGenealogicalValidationExtensions ResearchLanguageConfiguration

RULE

A genealogical Project Scientific Specification SHALL identify every
activated Processing Profile.

RULE

A genealogical Project Scientific Specification SHALL identify every
activated Genealogical Research Artifact type.

RULE

The project configuration SHALL preserve traceability to every activated
Genealogy Model definition.

### 1.18 Genealogy Project Extensions

PURPOSE

DefineGenealogySpecificProjectExtensionsWithoutRedefiningTheInheritedProjectExtensionModel.

GENEALOGY_SPECIFIC_EXTENSION_ELEMENTS

ProjectProcessingProfiles ProjectGenealogicalArtifactTypes
ProjectGenealogicalRules ProjectGenealogicalConstraints
ProjectGenealogicalGlossary ProjectGenealogicalValidationExtensions

RULE

Genealogy-specific project extensions SHALL specialize applicable
Genealogy Model definitions.

RULE

A Project Processing Profile SHOULD define how imported genealogical
data is transformed into traceable Genealogical Research Artifacts.

RULE

Genealogy-specific project extensions SHALL NOT weaken inherited General
Scientific Layer or Genealogy Model requirements.

### 1.19 Genealogy Specific Project Adaptation Guidance

PURPOSE

DefineHowConcreteGenealogicalProjectsSpecializeTheGenealogyModelWithinTheInheritedProjectModelAdaptationArchitecture.

ADAPTATION_GUIDANCE

ResearchObjectiveBinding SourceDomainSelection
ProcessingProfileSelection GenealogicalArtifactSelection
UncertaintyPolicySelection IdentityResolutionPolicySelection
ExportProfileSelection

RULE

A genealogical Project Scientific Specification SHALL identify the
genealogical research objective that governs project-specific
adaptation.

RULE

Project-specific source domains, Processing Profiles and Genealogical
Research Artifact types SHALL be selected explicitly when they
materially affect scientific processing.

RULE

A genealogical project SHALL document project-specific uncertainty and
identity-resolution policies when they differ from the default Genealogy
Model guidance.

RULE

Project adaptations SHOULD remain minimal and SHALL use existing
Genealogy Model definitions whenever suitable definitions exist.

RULE

A project-specific genealogical extension SHALL document its scientific
rationale, affected inherited definitions and expected impact.

RULE

Project-specific export profiles SHALL identify whether their outputs
are lossless, lossy or non-authoritative.

RULE

A project adaptation SHALL NOT silently change the meaning of inherited
genealogical artifact types, relationships, evidence states or
validation requirements.

RULE

A reusable project-specific extension SHOULD be registered as a
Genealogy Model specification candidate after successful practical
validation.

RULE

A ResearchObjective materially refined or changed during scientific work
SHALL be confirmed by the human before the refinement or change governs
scientific processing.

RULE

Expansion beyond the currently selected Source Domains that materially
changes the scientific search space SHALL be resolved as a project-specific
SourceDomainSelection before the expanded domain is used for scientific
processing.

RULE

Concrete source discovery, prioritization, selection and processing within
already selected Source Domains SHALL NOT by themselves require renewed
SourceDomainSelection.

CONFORMANCE

## Required

------------------------------------------------------------------------

## 2 Scientific Observation Model

PURPOSE

DefineHowScientificObservationsAreCreatedFromControlledScientificProcessing.

### 2.1 Scientific Observation

PURPOSE

DefineTheFundamentalScientificObservationProducedByControlledScientificProcessing.

DESCRIPTION

A Scientific Observation represents the first controlled persistent
Scientific Artifact produced from a source.

A Scientific Observation preserves the observed scientific content
together with its documented observational uncertainty.

A Scientific Observation SHALL remain independent from interpretation,
normalization, hypothesis formation, identity resolution and scientific
conclusions.

Scientific Observations constitute persistent scientific evidence.

RULE

Every Scientific Observation SHALL be a Scientific Artifact governed by
the uniform Core Scientific Artifact requirements.

RULE

Its status as a Scientific Artifact SHALL NOT permit interpretive or
normalizing modification of the observed content.

#### 2.1.1 Scientific Observation Identity

PURPOSE

DefineTheIdentityRequirementsForScientificObservations.

DESCRIPTION

A Scientific Observation is an independently identifiable scientific
result produced through controlled scientific processing.

Its identity represents the observed scientific content and remains
independent from the processed input, the applied processing activity
and every derived Scientific Artifact.

REQUIRED_INFORMATION

ObservationIdentifier

RULE

Every Scientific Observation SHALL possess exactly one stable
Observation Identifier.

RULE

The Observation Identifier SHALL remain stable while the scientific
identity of the Scientific Observation remains unchanged.

RULE

A change to the Processing Record, Processing Profile or Processing
Profile version SHALL NOT by itself require a new Observation
Identifier.

RULE

Scientific Observations representing different scientific observations
SHALL possess different Observation Identifiers.

RULE

The identity of a Scientific Observation SHALL remain distinguishable
from:

InputIdentifier

ProcessingRecordIdentifier

ScientificArtifactIdentifier

DerivationIdentifier

RULE

Supersession or reprocessing SHALL preserve traceability to predecessor
Scientific Observations.

RULE

The Observation Identifier SHALL remain suitable for persistent citation
throughout the complete scientific lifecycle.

#### 2.1.2 Scientific Observation Structure

PURPOSE

DefineTheMinimumStructuralRequirementsForScientificObservations.

DESCRIPTION

Every Scientific Observation represents one independently identifiable
scientific observation together with the minimum information required to
preserve its scientific meaning and its traceability to the observed
input.

REQUIRED_INFORMATION

ObservationIdentifier

InputIdentifier

InputSegmentReference

ObservedContent

RULE

Every Scientific Observation SHALL contain the minimum information
required for independent scientific interpretation.

RULE

Every Scientific Observation SHALL reference the input from which it
originates.

RULE

Every Scientific Observation SHALL identify the specific input segment
from which the observation was produced whenever the processed input
contains more than one independently addressable segment.

RULE

ObservedContent SHALL remain distinguishable from metadata, provenance,
uncertainty and validation information.

RULE

The structural definition of a Scientific Observation SHALL remain
independent from its physical serialization.

#### 2.1.3 Observation Representation

STATUS

ReservedForFutureIntegration

PURPOSE

DefineHowScientificObservationsMayBeRepresented.

#### 2.1.4 Observation Provenance

STATUS

ReservedForFutureIntegration

PURPOSE

DefineTheProvenanceResponsibilitiesOfScientificObservations.

#### 2.1.5 Observation Uncertainty

STATUS

ReservedForFutureIntegration

PURPOSE

DefineHowObservationSpecificUncertaintyWillBeRepresented.

#### 2.1.6 Observation Validation

STATUS

ReservedForFutureIntegration

PURPOSE

DefineHowScientificObservationsAreScientificallyValidated.

#### 2.1.7 Observation State

STATUS

ReservedForFutureIntegration

PURPOSE

ReserveTheScientificProcessingStateModelPendingGeneralScientificLayerReview.

#### 2.1.8 Observation Versioning And Reprocessing

STATUS

ReservedForFutureIntegration

PURPOSE

DefineHowScientificObservationsWillBeVersionedAndReprocessed.

RULE

Every Scientific Observation SHALL originate from controlled scientific
processing.

RULE

Every Scientific Observation SHALL preserve complete provenance to the
processed source.

RULE

A Scientific Observation SHALL remain distinguishable from its
scientific input, from interpretation and from Derived Scientific
Artifacts.

### 2.2 Observation Input Classes

PURPOSE

DefineTheGenealogySpecificClassesOfScientificInputThatMayEnterControlledObservationProcessing.

INPUT_CLASSES

GenealogicalSourceMaterial ImportedGenealogicalData
ReferencedGenealogicalResearch LegacyGenealogicalDatabase

RULE

Every input entering controlled scientific observation processing SHALL
preserve its original provenance.

RULE

Imported genealogical data SHALL remain distinguishable from
observations produced through controlled processing.

RULE

Referenced genealogical research SHALL be treated as source-derived
scientific input and SHALL NOT be accepted as validated project
knowledge without controlled evaluation.

RULE

Legacy genealogical databases SHALL preserve their original structure,
provenance and known limitations when entering controlled processing.

RULE

Standardized external genealogical formats SHOULD enter the Scientific
Observation Model through a documented Processing Profile.

RULE

Technical conformance of imported genealogical data SHALL be evaluated
separately from the scientific validity of its content.

RULE

The classification of an input SHALL NOT determine the validity of
observations derived from it.

#### 2.2.1 Observation Input Provenance

PURPOSE

DefineTheMinimumProvenanceRequirementsForInputsEnteringControlledObservationProcessing.

REQUIRED_INFORMATION

InputIdentifier InputClass OriginReference AcquisitionOrImportContext
AppliedProcessingProfile KnownLimitations

RULE

Every controlled observation process SHALL identify the input from which
the Scientific Observation originates.

RULE

Known limitations of an input SHALL remain traceable to every materially
affected Scientific Observation.

RULE

Transformation of an input representation SHALL NOT replace or obscure
the original provenance reference.

### 2.3 Observation Processing Profile

PURPOSE

DefineHowAProcessingProfileControlsTheCreationOfScientificObservations.

RULE

Every controlled observation process SHALL identify the applicable
Processing Profile before Scientific Observations are created.

RULE

The selected Processing Profile SHALL be suitable for the input class,
source characteristics and intended scientific activity.

RULE

A Processing Profile SHALL define the controlled operations by which
source input is transformed into Scientific Observations.

RULE

Scientific Observations created under different Processing Profiles
SHALL remain distinguishable when the applied processing materially
affects their content or interpretation.

RULE

A Processing Profile SHALL NOT silently introduce genealogical
interpretations that are not supported by the processed input.

RULE

Changes to an applied Processing Profile SHALL remain traceable and
SHALL NOT retroactively alter existing Scientific Observations without
controlled reprocessing.

#### 2.3.1 Observation Granularity

PURPOSE

DefineHowProcessingProfilesDetermineScientificObservationGranularity.

RULE

A Scientific Observation SHALL represent exactly one independently
addressable scientific observation.

RULE

Multiple Scientific Observations MAY originate from the same scientific
input.

RULE

Observation boundaries SHALL be determined by the applicable Processing
Profile.

RULE

Specialized Processing Profiles MAY extend the Scientific Observation
structure with additional observation-specific information provided that
the mandatory structural requirements defined by the Scientific
Observation Model remain preserved.

#### 2.3.2 Processing Profile Selection

PURPOSE

DefineTheSelectionRequirementsForProcessingProfilesUsedInScientificObservation.

SELECTION_FACTORS

InputClass SourceForm SourceLanguage WritingSystem DocumentStructure
ScientificObjective RequiredObservationGranularity KnownInputLimitations

RULE

A Processing Profile SHALL be selected explicitly when its choice
materially affects scientific processing.

RULE

The selection SHALL remain traceable to the processed input and every
Scientific Observation produced from it.

RULE

Only undefined Processing Profile parameters required for the next
scientific activity SHOULD be requested.

RULE

Previously confirmed Processing Profile parameters SHOULD be reused when
their applicability remains unchanged.

RULE

A project-specific Processing Profile MAY be used when no existing
Genealogy Model Processing Profile adequately represents the required
scientific method.

RULE

A project-specific Processing Profile SHALL document its scientific
rationale, inherited definitions and project-specific extensions.

#### 2.3.3 Observation Processing Record

PURPOSE

DefineTheMinimumRecordOfControlledProcessingThatProducesScientificObservations.

REQUIRED_INFORMATION

ProcessingRecordIdentifier InputIdentifier AppliedProcessingProfile
AppliedProfileVersion ResolvedProcessingParameters ProcessingActivity
ProducedObservationIdentifiers ProcessingAgentReferences
ProcessingTimeReference KnownProcessingLimitations

RULE

Every Scientific Observation SHALL remain traceable to exactly one or
more documented Processing Records.

RULE

A Processing Record SHALL preserve the Processing Profile version and
resolved parameters applied during processing.

RULE

Known processing limitations SHALL remain traceable to every materially
affected Scientific Observation.

RULE

Reprocessing the same input SHALL create a new Processing Record when
the Processing Profile, profile version or material processing
parameters change.

### 2.4 Observation Processing

PURPOSE

DefineHowControlledScientificProcessingProducesScientificObservations.

#### 2.4.1 Processing Stages

STAGES

InputPreparation ControlledObservation ObservationRecording
ObservationValidation ObservationCompletion

RULE

Every Scientific Observation SHALL be produced through the defined
processing stages.

RULE

The order of processing stages SHALL remain traceable.

#### 2.4.2 Observation Integrity

PURPOSE

PreserveTheScientificIntegrityOfScientificObservationsAsScientificEvidence.

RULE

Scientific Observations SHALL remain distinguishable from
interpretation, normalization, hypothesis formation, identity resolution
and scientific conclusions.

RULE

Observation processing SHALL NOT silently introduce unsupported
assumptions.

RULE

Known uncertainties SHALL remain explicitly documented as part of the
Scientific Observation.

RULE

Corrections, normalizations and subsequent scientific interpretations
SHALL remain fully traceable to the original Scientific Observation.

RULE

Corrections, normalizations and subsequent scientific interpretations
SHALL NOT modify the preserved observed content.

RULE

A ScientificObservation SHALL represent content scientifically observable
from its immediate Source Representation.

RULE

The scientific content of an underlying or otherwise related Source
Representation SHALL NOT be substituted for content observed from the
immediate Source Representation.

RULE

A ScientificObservation SHALL remain consistent with its immediate source
provenance and with the information scientifically observable from its
immediate Source Representation.

RULE

A detected inconsistency SHALL be documented without interpreting its cause
as part of the ScientificObservation.

RULE

Scientific Observations SHALL remain immutable scientific evidence once
observation processing has been completed. Subsequent scientific
refinement SHALL be performed exclusively through derived Scientific
Artifacts while preserving traceability to the original Scientific
Observation.

#### 2.4.3 Observation Completion Criteria

PURPOSE

DefineWhenObservationProcessingIsScientificallyComplete.

RULE

Observation processing SHALL be considered complete only after every
required Processing Profile step has been executed.

RULE

Incomplete observations SHALL remain explicitly identifiable.

RULE

Material changes to the Processing Profile SHALL require controlled
reprocessing.

RULE

Reprocessing SHALL create a new Processing Record.

RULE

Reprocessing SHALL preserve previous Observation history.

### 2.5 Observation Transition To Derived Scientific Artifacts

PURPOSE

DefineHowValidatedScientificObservationArtifactsContributeToDerivedScientificArtifacts.

#### 2.5.1 Derivation Conditions

PURPOSE

DefineTheConditionsRequiredForScientificArtifactDerivation.

RULE

Derived Scientific Artifacts MAY be formed from traceable Scientific
Observations and, where scientifically justified, from other traceable
Scientific Artifacts.

RULE

Derivation from a Scientific Observation SHALL occur only after the
required Observation Processing stages have been completed.

RULE

Required validation defined by the applicable Processing Profile SHALL
be satisfied before derivation.

RULE

Derived Scientific Artifact formation SHALL preserve every originating
Scientific Observation unchanged.

RULE

Derivation SHALL create new Derived Scientific Artifacts.

RULE

Derivation SHALL NOT replace the originating Scientific Observation.

RULE

Derivation SHALL NOT normalize the originating Scientific Observation.

RULE

Derivation SHALL NOT reinterpret the originating Scientific Observation.

#### 2.5.2 Derivation Traceability

PURPOSE

PreserveCompleteTraceabilityBetweenObservationsAndDerivedArtifacts.

RULE

Every Derived Scientific Artifact SHALL preserve complete traceability
to all originating Scientific Observations and Scientific Artifacts.

RULE

Scientifically relevant information SHALL NOT be silently lost during
derivation; every intentional selection, reduction or transformation
SHALL remain documented and traceable.

RULE

Derived Scientific Artifacts are formed from traceable scientific inputs
while preserving complete scientific traceability.

RULE

Every derived scientific statement SHALL remain traceable to its
originating Scientific Observations, Scientific Artifacts or both.

RULE

Derivation traceability SHALL preserve the distinction between observed
evidence and derived scientific interpretation.

#### 2.5.3 Artifact Formation Rules

PURPOSE

DefineHowDerivedScientificArtifactsAreFormedFromTraceableScientificInputs.

RULE

One Scientific Observation MAY contribute to multiple Derived Scientific
Artifacts.

RULE

Multiple Scientific Observations and existing Scientific Artifacts MAY
contribute to one Derived Scientific Artifact.

RULE

Applied Processing Profiles and explicit uncertainty representations
SHALL remain traceable.

RULE

Derived Scientific Artifacts MAY represent scientific interpretation,
normalization, integration and hypothesis formation derived from
traceable scientific inputs.

RULE

The creation, revision or replacement of a Scientific Artifact SHALL NOT
modify the originating Scientific Observation.

RULE

Multiple Scientific Artifacts MAY coexist when different scientifically
traceable interpretations are derived from the same Scientific
Observation.

#### 2.5.4 Artifact Derivation Record

PURPOSE

DefineTheMinimumRecordOfArtifactDerivation.

REQUIRED_INFORMATION

DerivationIdentifier SourceObservationIdentifiers
ProducedArtifactIdentifiers AppliedDerivationRules
ResponsibleProcessingProfile DerivationTimestamp
KnownDerivationLimitations

RULE

Every artifact derivation SHALL be documented through an Artifact
Derivation Record.

RULE

The derivation from a Scientific Observation Artifact to a Derived
Scientific Artifact SHALL preserve traceability and applicable
Processing Profile conformance.

  ------------------------------------------------------------------------------------------------
  SUBSECTION

  ObservationUncertainty

  PURPOSE

  DefineHowScientificObservationsRepresentScientificUncertaintyWithoutIntroducingInterpretation.

  DESCRIPTION

  Scientific uncertainty is an inherent property of scientific observation.

  Whenever the observed content cannot be determined with complete confidence, the uncertainty
  SHALL be documented as part of the Scientific Observation.

  The documentation of uncertainty SHALL describe the limitations of the observation itself.

  Scientific uncertainty documents only the limitations of the observation itself.

  The evaluation, reduction or resolution of observational uncertainty SHALL occur only through
  traceable scientific derivation and SHALL NOT modify the originating Scientific Observation.

  RULE

  Scientific Observations SHALL distinguish observed content from uncertainty information.

  RULE

  Uncertainty SHALL describe limitations of the observation and SHALL NOT introduce assumptions or
  interpretations.

  RULE

  Every documented uncertainty SHALL remain traceable to the observed input.

  RULE

  The absence of documented uncertainty SHALL NOT be interpreted as proof of correctness.

  RULE

  Additional uncertainty classifications MAY be introduced by specialized Processing Profiles
  provided that the original observed content remains preserved.

  RULE

  Scientific uncertainty SHALL describe only the limitations of the observation itself.

  RULE

  Scientific uncertainty SHALL NOT express the probability or correctness of subsequent scientific
  interpretations.

  RULE

  Hypotheses, assumptions and scientific conclusions derived from observed content SHALL be
  represented independently from the originating Scientific Observation.

  RULE

  Scientific Observations SHALL preserve documented uncertainty as part of the scientific
  evidence.

  The reduction, resolution or normalization of observational uncertainty SHALL occur only through
  traceable scientific derivation and SHALL NOT modify the originating Scientific Observation.
  ------------------------------------------------------------------------------------------------

## 3 Scientific Artifact Model

PURPOSE

DefineTheMinimalGenealogySpecificScientificArtifactArchitectureAndItsExtensionBoundary.

RESPONSIBILITY

DefineGenealogySpecificArtifactCore DefineArtifactMinimalRequirements
DefineArtifactExtensionPrinciples
SeparateArtifactStructureFromScientificWorkingMethod

RULE

New Artifact Types SHALL only be introduced when no existing Core
Artifact Type can represent the required scientific responsibility
without violating architectural separation.

RULE

Every newly introduced Artifact Type SHALL define exactly one
independent scientific responsibility.

RULE

New Artifact Types SHALL remain compatible with existing Core Artifact
semantics and SHALL NOT redefine previously established
responsibilities.

RULE

Architectural extensions SHALL be introduced through the normative
review and consolidation process before becoming part of the Core
Genealogy Model.

RULE

An authoritative working artifact MAY remain scientifically incomplete
during controlled iterative development, provided that its current
incompleteness remains explicitly identifiable.

RULE

Scientific persistence SHALL NOT require scientific completeness.

RULE

Scientific completeness SHALL be evaluated during validation and SHALL
NOT be treated as a prerequisite for artifact existence.

### 3.1 Scientific Artifact Model Purpose

PURPOSE DESCRIPTION

Scientific Artifact is the persistent scientific abstracted
representation of a single identifiable unit of scientific knowledge
that can be referenced, related, evaluated and reused throughout the
scientific lifecycle.

RULE

The Scientific Artifact Model SHALL define only genealogy-specific
artifact semantics not already defined by the General Scientific Layer.

RULE

The Scientific Artifact Model SHALL remain distinguishable from
scientific integration, validation, hypothesis formation and review
methodology.

RULE

Scientific working methodology SHALL remain outside the Scientific Artifact
Model and SHALL NOT be represented as mandatory artifact structure unless
persistence of a scientific statement is required.

### 3.2 Core Artifact Type Reference Set

PURPOSE

ProvideTheMinimumGenealogicalArtifactTypeReferenceSetRequiredForApplicableProcessingDefinitions.

CORE_ARTIFACT_TYPE_REFERENCE_SET

RegisteredSource ScientificObservation PersonIdentity Information Event

RULE

The Core Artifact Type Reference Set SHALL define the minimum
genealogy-specific artifact meanings required to guide conforming
Processing definitions.

RULE

Artifact Types contained in the Core Artifact Type Reference Set SHALL
NOT receive different Core treatment solely because of their Type.

RULE

All Scientific Artifacts SHALL remain subject to the same Core
requirements for identity, persistence, provenance, relationships,
evidence, uncertainty and validation.

RULE

The applicable Processing architecture SHALL define the formation,
interpretation, constraints and operational treatment of the referenced
Artifact Types.

RULE

The Core Artifact Type Reference Set SHALL be treated as an open minimum
reference set and SHALL NOT be interpreted as a closed ontology.

RULE

Additional Artifact Types MAY be defined by Processing Profiles or
project adaptation when required by scientific responsibility.

RULE

A new referenced Artifact Type SHOULD be introduced only when its
independent scientific meaning cannot be represented adequately through
an existing reference type, Event specialization or Scientific
Relationship.

RULE

Every Artifact Type contained in the Core Artifact Type Reference Set
SHALL define exactly one independent genealogy-specific semantic
responsibility.

#### 3.2.1 Registered Source

PURPOSE DESCRIPTION

Registered Source is the scientific representation of an independently
identifiable object registered to provide a persistent reference and
connection point for corresponding scientific content.

RULE

A RegisteredSource SHALL represent the semantic concept of one
independently addressable scientific source.

RULE

RegisteredSource SHALL provide semantic orientation only and SHALL NOT
define type-specific Core structure or Core behavior.

RULE

The registration, acquisition, import, management, validation and
operational treatment of RegisteredSource Artifacts SHALL be governed by
the applicable Processing architecture.

RULE

A RegisteredSource SHALL remain distinguishable from
ScientificObservation, PersonIdentity, Information, Event and every other referenced
Artifact Type.

#### 3.2.2 Scientific Observation

PURPOSE

ProvideTheMinimumGenealogicalSemanticReferenceForProcessingDefinitionsThatRepresentScientificObservations.

RULE

ScientificObservation SHALL denote the semantic concept of one
independently identifiable evidence-preserving Scientific Artifact.

RULE

ScientificObservation SHALL conform to the Scientific Observation Model
defined in Chapter 2.

RULE

ScientificObservation SHALL provide semantic orientation only and SHALL
NOT define type-specific Core structure or Core behavior.

RULE

Observation identity, structure, provenance, uncertainty, validation and
processing SHALL be governed by the uniform Scientific Artifact
requirements, the Scientific Observation Model and the applicable
Processing architecture.

RULE

ScientificObservation SHALL remain distinguishable from
RegisteredSource, PersonIdentity, Information, Event and every other referenced
Artifact Type.

#### 3.2.3 Person Identity

PURPOSE

ProvideTheMinimumGenealogicalSemanticReferenceForProcessingDefinitionsThatRepresentAnIndependentlyAddressablePersonIdentity.

RULE

PersonIdentity SHALL denote the persistent scientific identity of one
person.

RULE

PersonIdentity SHALL provide semantic orientation only and SHALL NOT
define type-specific Core structure or Core behavior.

RULE

Genealogical properties and assertions concerning a PersonIdentity SHALL
be represented through independently persistent Scientific Artifacts and
Relationships.

RULE

The applicable Processing architecture SHALL define the formation,
interpretation, constraints and operational treatment of PersonIdentity
Artifacts.

RULE

PersonIdentity SHALL remain distinguishable from RegisteredSource,
ScientificObservation, Information, Event and every other referenced Artifact Type.

#### 3.2.4 Information

PURPOSE

RepresentAnIndependentlyPersistentScientificInformationStatementNotSufficientlyRepresentedByAnotherApplicableScientificArtifactType.

RULE

An InformationArtifact SHALL represent an independently addressable
scientific information statement.

RULE

An InformationArtifact MAY concern any Scientific Artifact.

RULE

The availability of InformationArtifact SHALL NOT restrict the definition or
use of more specialized Scientific Artifact types.

RULE

InformationArtifact SHALL remain distinguishable from RegisteredSource,
ScientificObservation, PersonIdentity, Event and every other referenced
Artifact Type.

#### 3.2.5 Event

PURPOSE

ProvideTheMinimumGenealogicalSemanticReferenceForProcessingDefinitionsThatRepresentAnIndependentlyAddressableGenealogicalEvent.

RULE

Event SHALL denote the semantic concept of one independently
identifiable genealogical event.

RULE

Event SHALL provide semantic orientation only and SHALL NOT define
type-specific Core structure or Core behavior.

RULE

The applicable Processing architecture SHALL define the formation,
interpretation, constraints, specialization and operational treatment of
Event Artifacts.

RULE

The scientific identity of an Event SHALL remain independent from
evidence, uncertainty, validation and hypothesis assessment.

RULE

Event SHALL remain distinguishable from RegisteredSource,
ScientificObservation, PersonIdentity, Information and every other referenced
Artifact Type.

### 3.3 Event Specializations

PURPOSE

ProvideReusableGenealogicalSemanticReferenceEventsForProcessingDefinitions.

REFERENCE_EVENT_SPECIALIZATIONS

BirthEvent BaptismEvent MarriageEvent DeathEvent BurialEvent
ResidenceEvent MigrationEvent OtherGenealogicalEvent

RULE

Reference Event Specializations SHALL provide reusable
genealogy-specific semantic orientation for Processing definitions.

RULE

Reference Event Specializations SHALL NOT define type-specific Core
structure or Core behavior.

RULE

The applicable Processing architecture SHALL define the formation,
interpretation, constraints and operational treatment of Event
Specializations.

RULE

The Reference Event Specializations SHALL be treated as an open
reference set and SHALL NOT be interpreted as a closed event taxonomy.

RULE

Projects MAY define additional Event Specializations when required by
scientific responsibility while remaining compatible with the Core Event
reference.

### 3.4 Artifact Minimal Requirements

PURPOSE

DefineTheMinimumScientificRequirementsForPersistentScientificArtifacts.

RULE

Every persistent Scientific Artifact SHALL contain or participate in at
least one meaningful scientific statement.

RULE

Every persistent Scientific Artifact SHOULD remain connected to at least
one other Scientific Artifact or persistent scientific statement through
a traceable scientific relationship.

RULE

Scientific completeness SHALL be determined by the scientific meaning
represented by the Artifact and SHALL NOT depend on its referenced
Artifact Type.

RULE

Administrative or semantically empty structures SHALL NOT by themselves
be regarded as scientifically complete.

RULE

The applicable Processing architecture MAY define additional
completeness criteria for referenced Artifact Types provided that the
uniform Core Artifact architecture remains unchanged.

PRINCIPLE

MeaningBeforeStructure

PRINCIPLE

UniformArtifactCompleteness

PRINCIPLE

ScientificConnectivity

### 3.5 Artifact Extension Principles

PURPOSE

DefineHowScientificArtifactsMAYBeExtendedWithoutChangingTheUniformCoreArchitecture.

RULE

The Core SHALL define only the minimum scientific architecture required
for persistent Scientific Artifacts.

RULE

Referenced Artifact Types SHALL provide semantic orientation only and
SHALL NOT introduce alternative Core architectures.

RULE

The applicable Processing architecture MAY define additional Artifact
Types, semantic reference sets, constraints and operational behavior.

RULE

Processing extensions SHALL remain compatible with the uniform
Scientific Artifact architecture defined by the Core.

RULE

Projects MAY introduce domain-specific Processing Profiles without
modifying the normative Core.

PRINCIPLE

StableCore

PRINCIPLE

OpenProcessingExtensions

PRINCIPLE

SemanticCompatibility

### 3.6 Genealogy Scientific Relationship Model

PURPOSE

DefineTheMinimumGenealogySpecificPersistentRelationshipSemanticsRequiredToConnectScientificArtifactsWithoutDuplicatingGeneralScientificLayerResponsibilities.

CONFORMS_TO

GSL.ScientificArtifactRelationships

RULE

A Genealogy Scientific Relationship SHALL represent an independently
addressable persistent scientific connection between two or more Scientific
Artifacts.

RULE

Every Genealogy Scientific Relationship SHALL identify its participating
Scientific Artifact endpoints and SHALL provide a scientifically
distinguishable Relationship semantic or expression.

RULE

Endpoint position alone SHALL NOT determine scientific direction, endpoint
role or Relationship meaning.

RULE

Relationship Context MAY reference an applicable Scientific Artifact where
that Artifact qualifies the meaning of the specific Relationship.

RULE

Relationship Context SHALL NOT substitute for independently persistent
scientific information that requires its own Scientific Artifact.

RULE

Genealogy-specific Relationship semantics SHALL specialize applicable GSL
Scientific Artifact Relationship responsibilities and SHALL NOT redefine GSL
ownership of Scientific Artifact identity, provenance, history, lifecycle,
supersession or universal scientific relationship classes.

#### 3.6.1 Relationship Semantic Families

PURPOSE

ProvideTheMinimumReusableGenealogySpecificRelationshipSemanticsRequiredByConformingProcessingDefinitions.

RELATIONSHIP_SEMANTIC_REFERENCE_SET

ReferenceRelationship ParticipationRelationship ObservationReferenceRelationship
EvidenceSupportRelationship

RULE

ReferenceRelationship SHALL represent a scientifically established reference
between applicable Scientific Artifacts where no more specialized Core
Relationship semantic is required.

RULE

ParticipationRelationship SHALL represent the participation of an applicable
Scientific Artifact in an Event and MAY carry a RoleType or equivalent
scientifically meaningful participation role.

RULE

ParticipationRelationship SHALL NOT by itself establish kinship, identity or
another genealogical Relationship not independently supported.

RULE

ObservationReferenceRelationship SHALL represent observation-derived support
or reference to an independently addressable Scientific Artifact representing
the applicable information or scientific statement.

RULE

EvidenceSupportRelationship SHALL represent scientific evidential support and
SHALL remain semantically distinguishable from
ObservationReferenceRelationship.

RULE

The Relationship Semantic Reference Set SHALL be treated as an open minimum
reference set. Processing definitions MAY define additional genealogy-specific
Relationship Expressions where an existing Core semantic, endpoint role or
Relationship Context cannot adequately represent the required scientific
meaning.

#### 3.6.2 Observation--Artifact Relationship Semantics

RULE

An ObservationReferenceRelationship used to represent observation-derived
information SHALL reference an independently addressable Scientific Artifact
representing that information or scientific statement.

RULE

Relationship Context MAY preserve observation-related context that qualifies
the specific reference or derivation.

RULE

Relationship Context SHALL NOT substitute for independently persistent
scientific information that requires its own Scientific Artifact.

RULE

A PersonIdentity SHALL NOT serve as the evidence target for a genealogical
statement solely by virtue of representing the person to whom that statement
relates.

RULE

Complete scientific traceability SHALL NOT require every previously evaluated
ScientificObservation to maintain a redundant direct relationship to a
Scientific Artifact where the applicable scientific provenance and research
history remain otherwise unambiguous.

#### 3.6.3 Current Relationship State

PURPOSE

DistinguishTheCurrentScientificRelationshipStateFromPreservedRelationshipHistory.

RULE

Superseded Relationships SHALL remain referenceable for scientific history
and traceability.

RULE

A Superseded Relationship SHALL NOT contribute to the current scientific
relationship state unless the applicable scientific operation explicitly
includes historical or superseded Relationships.

RULE

Relationship state semantics SHALL remain distinguishable from Scientific
Artifact lifecycle semantics.

RULE

Preservation of a Relationship for scientific history and traceability SHALL
NOT by itself require that Relationship to contribute to the current
scientific relationship state.

### 3.7 Scientific Cluster

PURPOSE

DefineTheMinimumScientificSemanticsOfAReadOnlyStructuralInvestigationWorkspaceDerivedFromTheApplicableScientificRelationshipState.

RULE

The Scientific Cluster provides a deterministic, reproducible and read-only
structural investigation workspace derived from an applicable scientific
relationship state.

RULE

A Scientific Cluster SHALL NOT modify the authoritative scientific state.

RULE

Cluster construction SHALL be structurally complete within its defined
traversal boundary.

RULE

Cluster construction SHALL NOT perform scientific interpretation, evidence
evaluation, hypothesis generation or identity resolution.

RULE

Traversal conditions MAY define scientifically meaningful structural
expansion and depth semantics.

RULE

The applicable current scientific relationship state SHALL be resolved before
Cluster traversal is evaluated.

RULE

GM SHALL NOT prescribe a graph traversal implementation algorithm.

SCOPE_BOUNDARY

Scientific Cluster is a derived investigation workspace and SHALL NOT by
itself define persistent Cluster snapshots, Cluster lifecycle or versioning,
synchronization, graph algorithms or project workflow semantics.

## 4 Authoritative Genealogical Research Artifact Register (AGRAR)

### 4.1 Purpose and Scientific Responsibility

#### Scientific Responsibility

The **Authoritative Genealogical Research Artifact Register (AGRAR)**
defines the authoritative management framework for all addressable
scientific elements belonging to a genealogy research project.

Its scientific responsibility is limited to establishing, maintaining,
and preserving authoritative register membership throughout the complete
lifecycle of the register.

The register shall not define, interpret, or modify the scientific
semantics of the referenced elements.

#### Normative Requirements

The register shall:

-   provide a single authoritative representation of register
    membership;
-   maintain stable identification of register entries;
-   support authoritative register revisions;
-   preserve traceability throughout all register revisions;
-   remain independent of the semantic content of referenced scientific
    elements.

#### Scope Boundaries

This chapter shall not define:

-   scientific observations;
-   scientific artifacts;
-   scientific relationships;
-   scientific clusters;
-   processing procedures;
-   persistence technologies;
-   serialization formats;
-   implementation-specific execution mechanisms.

These responsibilities are defined by their respective GM Core chapters
or by the GM Execution specification.

#### Conformance Criteria

A conformant implementation shall demonstrate that:

-   register membership is managed exclusively through AGRAR;
-   every managed element is represented through a RegisterEntry;
-   no semantic interpretation is performed by the register itself;
-   register authority is preserved across all register revisions.

### 4.2 Architectural Position

#### Scientific Responsibility

This section defines the architectural position of the **Authoritative
Genealogical Research Artifact Register (AGRAR)** within the Genealogy
Model Core.

AGRAR constitutes the management layer of the GM Core. It provides the
authoritative framework for managing scientific elements without
defining their scientific semantics or execution.

#### Normative Requirements

AGRAR shall:

-   operate as the authoritative management component of the GM Core;
-   manage membership of addressable scientific elements;
-   remain independent of semantic definitions provided by other GM Core
    chapters;
-   remain independent of execution-specific implementations;
-   provide the authoritative bridge between the semantic model and the
    execution layer.

#### Architectural Relationships

AGRAR shall:

-   inherit the scientific principles defined by the Foundation;
-   manage the scientific elements defined by the Semantic Components;
-   expose an execution-independent authoritative register model to the
    GM Execution.

#### Scope Boundaries

AGRAR shall not:

-   define scientific observations;
-   define scientific artifacts;
-   define scientific relationships;
-   define scientific clusters;
-   prescribe persistence technologies;
-   prescribe serialization formats;
-   prescribe implementation-specific execution behaviour.

#### Conformance Criteria

A conformant implementation shall demonstrate that:

-   AGRAR occupies the management layer of the GM Core;
-   semantic responsibilities remain within the Semantic Components;
-   execution responsibilities remain within the GM Execution;
-   no architectural responsibility is assigned to more than one layer.

### 4.3 Project Binding and Register Singularity

#### Scientific Responsibility

This section defines the normative relationship between a genealogy
research project and its Authoritative Genealogical Research Artifact
Register (AGRAR).

AGRAR is established by the research project and represents the single
authoritative register for all addressable scientific elements belonging
to that project.

#### Normative Requirements

A genealogy research project shall:

-   define exactly one authoritative AGRAR;
-   manage all addressable scientific elements through that AGRAR;
-   maintain the logical unity of AGRAR regardless of its physical
    implementation.

AGRAR shall not be partitioned into multiple authoritative registers
based on artifact type or scientific category.

#### Scope Boundaries

This section shall not define:

-   register entries;
-   register revisions;
-   technical storage structures;
-   database schemas;
-   serialization formats;
-   implementation-specific metadata.

Physical implementations may partition data internally, provided they
preserve the normative concept of a single authoritative AGRAR.

#### Conformance Criteria

A conformant implementation shall demonstrate that:

-   exactly one AGRAR exists for each genealogy research project;
-   all addressable scientific elements belong to that AGRAR;
-   technical implementations do not create multiple authoritative
    registers;
-   the logical integrity of AGRAR is preserved independently of
    execution mechanisms.

### 4.4 Register Entry

#### Scientific Responsibility

This section defines the normative concept of a **RegisterEntry** within
the Authoritative Genealogical Research Artifact Register (AGRAR).

A RegisterEntry represents the authoritative inclusion of one
addressable scientific element in AGRAR.

The RegisterEntry defines register membership only. It neither defines
nor modifies the scientific semantics of the referenced element.

#### Normative Requirements

A RegisterEntry shall:

-   represent the authoritative inclusion of exactly one addressable
    scientific element;
-   remain independent of the scientific type of the referenced element;
-   remain independent of implementation-specific representations;
-   not define or modify scientific semantics;
-   support the authoritative management principles established by
    AGRAR.

#### Scope Boundaries

This section shall not define:

-   the internal structure of scientific elements;
-   property descriptions;
-   processing behaviour;
-   persistence models;
-   serialization mechanisms;
-   implementation-specific data structures.

These responsibilities belong to the GM Execution and its associated
specifications.

#### Conformance Criteria

A conformant implementation shall demonstrate that:

-   every addressable scientific element included in AGRAR is
    represented through a RegisterEntry;
-   RegisterEntries are independent of scientific element types;
-   RegisterEntries do not introduce scientific semantics beyond
    register membership;
-   implementation-specific representations preserve the normative
    concept of RegisterEntry.

### 4.5 Register Revision

#### Scientific Responsibility

This section defines the application of the **General Scientific Layer
(GSL)** concept of an authoritative scientific state to the
**Authoritative Genealogical Research Artifact Register (AGRAR)**.

A **Register Revision** represents one authoritative scientific state of
AGRAR. The scientific concepts governing authoritative states,
scientific derivation, reconstruction and validation are defined by the
applicable GSL specification. This chapter specifies only their
genealogy-specific application to AGRAR.

#### Normative Requirements

A Register Revision shall:

-   represent one authoritative scientific state of AGRAR;
-   conform to the applicable GSL requirements governing authoritative
    scientific states;
-   preserve the authoritative integrity of AGRAR;
-   provide the authoritative basis for genealogy-specific scientific
    processing.

The creation, modification and lifecycle management of Register
Revisions shall be defined by the GM Execution.

#### Scope Boundaries

This section shall not define:

-   authoritative state models;
-   scientific derivation;
-   scientific reconstruction;
-   scientific validation;
-   generation algorithms;
-   processing workflows;
-   persistence technologies;
-   serialization mechanisms.

These responsibilities are defined by the applicable GSL specification
or by the GM Execution.

#### Conformance Criteria

A conformant implementation shall demonstrate that:

-   every Register Revision represents one authoritative scientific
    state of AGRAR;
-   Register Revisions conform to the applicable GSL requirements;
-   genealogy-specific processing preserves the authoritative meaning of
    each Register Revision;
-   execution-specific implementations do not alter the normative
    concept of Register Revision.

### 4.6 Register Integrity

#### Scientific Responsibility

This section defines the genealogy-specific application of scientific
integrity to the **Authoritative Genealogical Research Artifact Register
(AGRAR)**.

Register Integrity ensures that AGRAR remains the complete,
authoritative and internally consistent management representation of all
addressable scientific elements belonging to a genealogy research
project.

The general scientific principles governing integrity are defined by the
applicable **General Scientific Layer (GSL)**. This chapter specifies
only their application to AGRAR.

#### Normative Requirements

AGRAR shall:

-   preserve the authoritative integrity of register membership;
-   maintain the logical consistency of all RegisterEntries;
-   preserve the completeness of the authoritative register;
-   conform to the applicable GSL requirements governing scientific
    integrity.

The methods used to verify or enforce Register Integrity shall be
defined by the GM Execution.

#### Scope Boundaries

This section shall not define:

-   scientific integrity models;
-   validation algorithms;
-   consistency checking procedures;
-   processing workflows;
-   persistence mechanisms;
-   implementation-specific integrity controls.

These responsibilities are defined by the applicable GSL specification
or by the GM Execution.

#### Conformance Criteria

A conformant implementation shall demonstrate that:

-   AGRAR preserves authoritative register integrity;
-   RegisterEntries remain logically consistent;
-   all applicable GSL integrity requirements are satisfied;
-   execution-specific implementations preserve the normative integrity
    of AGRAR.

### 4.7 Execution Boundary

#### Scientific Responsibility

This section defines the architectural boundary between the **Genealogy
Model Core (GM Core)** and the **Genealogy Model Execution (GM
Execution)** for the **Authoritative Genealogical Research Artifact
Register (AGRAR)**.

The GM Core defines the normative scientific concepts governing AGRAR.

The GM Execution defines the implementation-specific realization of
those concepts.

#### Normative Requirements

The GM Core shall define:

-   the normative concept of AGRAR;
-   the normative concept of RegisterEntry;
-   the normative concept of Register Revision;
-   the normative concept of Register Integrity.

The GM Execution shall define:

-   processing procedures;
-   property descriptions;
-   persistence models;
-   serialization formats;
-   execution workflows;
-   implementation-specific data structures.

#### Scope Boundaries

The GM Core shall not prescribe:

-   implementation technologies;
-   storage mechanisms;
-   programming models;
-   database schemas;
-   exchange formats;
-   execution-specific lifecycle management.

These responsibilities belong exclusively to the GM Execution.

#### Conformance Criteria

A conformant implementation shall demonstrate that:

-   normative scientific concepts are defined exclusively by the GM
    Core;
-   implementation-specific realization is defined exclusively by the GM
    Execution;
-   no execution-specific behaviour modifies the normative meaning of
    AGRAR.

### 4.8 Conformance Requirements

#### Scientific Responsibility

This section defines the normative conformance requirements for an
implementation of the Authoritative Genealogical Research Artifact
Register (AGRAR).

It consolidates the normative requirements established throughout this
chapter without introducing additional scientific concepts.

#### Normative Requirements

A conformant implementation shall demonstrate that:

-   exactly one AGRAR exists for each genealogy research project;
-   all addressable scientific elements are managed through AGRAR;
-   RegisterEntry is used solely as the normative representation of
    authoritative register membership;
-   Register Revisions conform to the applicable General Scientific
    Layer (GSL) requirements for authoritative scientific states;
-   Register Integrity conforms to the applicable GSL requirements for
    scientific integrity;
-   implementation-specific behaviour remains within the
    responsibilities of the GM Execution.

#### Scope Boundaries

This section shall not define:

-   additional scientific concepts;
-   implementation-specific conformance tests;
-   execution-specific validation procedures;
-   certification processes.

These responsibilities belong to the applicable GSL, the GM Execution or
external conformance procedures.

#### Conformance Criteria

A conformant implementation shall satisfy all normative requirements
defined in Sections 6.1 through 6.7.

## 5 GM Core--Execution Interface

### 5.1 Purpose and Scientific Responsibility

#### Scientific Responsibility

This chapter defines the normative architectural interface between the
**Genealogy Model Core (GM Core)** and the **Genealogy Model Execution
(GM Execution)**.

Its scientific responsibility is limited to establishing the
authoritative boundary between normative scientific concepts defined by
the GM Core and their operational realization within the GM Execution.

The scientific semantics defined by the GM Core SHALL remain
authoritative throughout operational realization.

#### Normative Requirements

The architectural interface SHALL:

-   establish the normative boundary between the GM Core and the GM
    Execution;
-   preserve the scientific authority of concepts defined by the GM
    Core;
-   permit execution-specific operational realization without modifying
    Core semantics;
-   provide a stable architectural foundation for conforming execution
    specifications.

The GM Execution SHALL NOT redefine, weaken or replace normative
scientific concepts established by the GM Core.

#### Scope Boundaries

This chapter shall not define execution procedures, Processing Profiles,
persistence technologies, serialization formats, implementation-specific
data structures or operational workflows.

These responsibilities belong to the GM Execution and its associated
specifications.

### 5.2 Architectural Position

#### Scientific Responsibility

This section defines the architectural position of the GM Execution
within the Genealogy Model architecture.

#### Architectural Relationship

The architectural relationship is:

General Scientific Layer (GSL) → Genealogy Model Core (GM Core) →
Genealogy Model Execution (GM Execution)

The GM Execution constitutes the operational layer through which the
normative genealogy-specific scientific concepts of the GM Core are
realized under the governing principles inherited from the applicable
GSL.

### 5.3 Core Responsibilities

#### Scientific Responsibility

The GM Core SHALL define the genealogy-specific normative scientific
concepts, architectural principles and semantic constraints required by
the Genealogy Model.

The GM Core SHALL remain implementation-independent.

Operational procedures, Processing Profiles, persistence technologies,
serialization formats and implementation-specific workflows SHALL NOT be
defined as Core responsibilities.

### 5.4 Execution Responsibilities

#### Scientific Responsibility

The GM Execution SHALL provide the operational realization of the
normative scientific concepts established by the GM Core.

A scientific decision SHALL NOT substitute for an applicable GM
Execution or define an otherwise unspecified execution-specific
processing or persistence procedure.

Execution responsibilities MAY include:

-   scientific processing procedures;
-   Processing Profiles;
-   persistence and serialization realization;
-   implementation-specific data structures;
-   operational workflows;
-   execution-specific validation procedures.

Execution responsibilities SHALL remain within the architectural
boundary established in Section 5.1.

### 5.5 Extension Boundary

#### Scientific Responsibility

This section defines the normative architectural boundary governing
extensions to the **Genealogy Model (GM)**.

Extensions MAY introduce additional operational capabilities provided
that they remain consistent with the normative scientific concepts and
architectural principles defined by the GM Core.

Extensions SHALL NOT modify, redefine or weaken the authoritative
scientific semantics established by the GM Core.

The structure, implementation and lifecycle of individual extensions
belong to the GM Execution and its associated specifications unless
another normative owner is explicitly defined.

### 5.6 Conformance

#### Scientific Responsibility

This section defines the criteria by which an operational realization
demonstrates conformity with the normative framework defined by the GM
Core.

#### Conformance Criteria

A conformant operational realization SHALL:

-   preserve the normative scientific semantics established by the GM
    Core;
-   preserve the architectural responsibility boundary defined by this
    chapter;
-   realize Core concepts without altering their normative meaning;
-   keep implementation-specific behavior within the responsibilities
    assigned to the GM Execution.

This section SHALL NOT define implementation-specific conformance
procedures, certification methods, validation algorithms or assessment
processes.

Such procedures belong to the applicable GSL, the GM Execution or
external conformance procedures.

## 6 Appendices

### Appendix A --- Scientific Specification Consolidation Method (SSCM)

#### Purpose

This appendix defines a recommended scientific methodology for
consolidating complex scientific specifications while preserving
architectural consistency, traceability, maintainability and
extensibility.

#### Consolidation Phases

##### Phase 1 --- Responsibility Identification

Identify the unique scientific responsibility of every architectural
component.

##### Phase 2 --- Responsibility Migration

Assign every normative statement to exactly one architectural owner.

##### Phase 3 --- Responsibility Consolidation

Ensure every architectural component answers one clearly defined
scientific question.

##### Phase 4 --- Architecture Validation

Validate the consolidated architecture using the following criteria:

-   Single Owner Principle
-   Completeness
-   Redundancy Elimination
-   Independent Extensibility

##### Phase 5 --- Normative Consistency Review

Review every normative statement (RULE, MUST, SHALL, MUST NOT, SHOULD)
for:

-   Normative clarity
-   Correct architectural ownership
-   Redundancy elimination
-   Contradiction-free behavior
-   Objective testability

##### Phase 6 --- Editorial Consolidation

Only after successful architectural validation perform:

-   Terminology harmonization
-   Structural ordering
-   Cross-reference verification
-   Editorial consistency
-   Final numbering

#### Architecture Review Questions

For every architectural component:

1.  Does it have exactly one scientific responsibility?
2.  Does every normative statement have exactly one owner?
3.  Can the component evolve independently?
4.  Does it integrate consistently into the complete scientific
    lifecycle?

### Appendix T --- Architectural Core Concepts

#### Purpose

Introduce the core architectural concepts of the Genealogy Model.
Normative responsibilities, architectural boundaries and behavioral
requirements remain defined by the corresponding Purpose and RULE
sections of the specification.

#### T.1 Scientific Artifact

Definition

A Scientific Artifact is an independently addressable persistent
scientific representation forming the fundamental architectural building
block from which specialized Scientific Artifacts are derived.

#### T.2 Registered Source

Definition

A Registered Source is a Scientific Artifact representing a persistently
registered source that may support Scientific Observations and other
Scientific Artifacts.

#### T.3 Scientific Observation

Definition

A Scientific Observation is a persistently recorded portion of
information derived through observation of an identifiable and
referenceable part of a Registered Source and made available as a
reference for other Scientific Artifacts.

#### T.4 Information

Definition

An Information Artifact is an independently addressable persistent scientific
statement used where the information is not sufficiently represented by
another applicable Scientific Artifact type.

#### T.5 Relationship

Definition

A Relationship is an independently addressable persistent scientific
connection between two or more Scientific Artifacts whose semantic meaning
remains distinguishable from endpoint position and Scientific Artifact
lifecycle state.

#### T.6 Evidence

Definition

The scientifically modeled connection between a Scientific Artifact and
the supporting Scientific Artifacts or Registered Sources from which its
scientific assertions are derived.

#### T.7 Scientific Cluster

Definition

A Scientific Cluster is a deterministic, reproducible and read-only structural
investigation workspace derived from an applicable current scientific
relationship state within a defined traversal boundary.

#### T.8 Scientific Artifact as a Person

Definition

A Scientific Artifact as a Person is an aggregating Scientific Artifact
whose scientific representation is composed of references to
independently addressable Scientific Artifacts rather than by embedding
scientific properties directly.

#### T.9 Obscure Fact

Definition

An Obscure Fact is a scientific fact for which the available evidence is
insufficient to support a reliable scientific assertion without
introducing hypotheses or unsupported assumptions.
