# Genealogy Model (GM)

## GM Core v1.0

### Artifact Working Document (AWD)

STATUS

Baseline

VERSION

1.0 Core Initialization Baseline

DOCUMENT_IDENTIFIER

GC001-GM-Core

DOCUMENT_TYPE

NormativeSpecificati

DEPENDS_ON

GSL-2.0-RC3

LANGUAGE

DSL

SPECIFICATION_LINEAGE

AUTHOR JonasM49

PUBLISHED_AT 2026-07-15

CANONICAL_REPOSITORY https://github.com/JonasM49/scientific-Framework

LICENSE CC BY-NC-SA 4.0

------------------------------------------------------------------------------

SECTION

GeneralArtifactModelBinding

PURPOSE

DefineHowTheGenealogyModelSpecializesTheGeneralScientificArtifactModelDefinedByTheGeneralScientificLayer.

RULE

The Genealogy Model SHALL adopt the General Scientific Artifact Model defined by the General Scientific Layer.

RULE

The Genealogy Model SHALL specialize Scientific Artifact types only by adding genealogy-specific semantics.

RULE

The Genealogy Model SHALL NOT redefine identity, lifecycle, provenance, metadata, integrity or traceability requirements already defined by the General Scientific Layer.

RULE

Whenever a genealogy-specific concept can be represented by specialization of the General Scientific Artifact Model, specialization SHALL be preferred over independent definition.

SECTION

AuthoritativeWorkingLifecycleBinding

PURPOSE

DefineHowGenealogyModelArtifactsAdoptTheAuthoritativeWorkingElementLifecycleDefinedByTheGeneralScientificLayer.

CONFORMS_TO

GSL.AuthoritativeWorkingElement

RULE

A Genealogy Model artifact that requires controlled iterative development SHALL conform to the Authoritative Working Element model defined by the General Scientific Layer.

RULE

The Genealogy Model SHALL inherit AWE generation, predecessor lineage, validation, authority transfer, recovery and persistence requirements without independent redefinition.

RULE

Genealogy-specific AWE specializations SHALL add only domain-specific validation, content-integrity or persistence constraints.

RULE

A failed transformation SHALL preserve the last verified authoritative GM artifact state.

RULE

Authority SHALL transfer to a successor GM artifact only after the successor has been completely persisted and successfully verified.

RULE

Artifact lifecycle state, artifact version and AWE generation SHALL remain distinguishable.

SUBSECTION

AWEApplicabilityForGMArtifacts

PURPOSE

IdentifyWhichGenealogyModelArtifactsRequireAuthoritativeWorkingElementConformance.

AWE_REQUIRED_FOR

ProjectScientificSpecificationWorkingDraft
AuthoritativeGenealogicalResearchArtifactRegister
IterativelyDevelopedGenealogicalResearchArtifact

AWE_CONDITIONAL_FOR

DerivedExportWorkingArtifact
ReferenceImplementationWorkingArtifact
ValidationArtifactUnderIterativeRevision

AWE_NOT_REQUIRED_BY_DEFAULT_FOR

FrozenReleasedSpecification
ImmutableSourceArtifact
LossyPresentationExport
ReadOnlyReferenceArtifact

RULE

A GM artifact SHALL conform to the Authoritative Working Element model when it is developed through controlled iterative transformation and one current authoritative state must be preserved.

RULE

The Authoritative Genealogical Research Artifact Register SHALL conform to AWE because it represents the authoritative persistent research state.

RULE

The Authoritative Genealogical Research Artifact Register SHALL be a Core-defined scientific model.

RULE

Its operational realization SHALL be defined by the applicable Processing architecture.

RULE

A Project Scientific Specification under active revision SHALL conform to AWE.

RULE

Immutable source artifacts SHALL preserve provenance and integrity but SHALL NOT be converted into AWE working states merely because they are referenced by a project.

RULE

Derived exports SHOULD conform to AWE only when the export itself is iteratively developed as an authoritative working artifact.

SUBSECTION

GenealogySpecificAWEValidationRequirements

PURPOSE

DefineGenealogySpecificValidationRequirementsAppliedInAdditionToTheGeneralScientificLayerAWEModel.

VALIDATION_REQUIREMENTS

GenealogicalTraceability
SourceEvidenceCompleteness
RelationshipConsistency
IdentityResolutionConsistency
GenealogicalUncertaintyIntegrity
ProcessingProfileConformance

RULE

Every authoritative Authoritative Genealogical Research Artifact Register SHALL preserve complete traceability from every asserted research statement to its supporting Scientific Artifacts.

RULE

Authority SHALL NOT be transferred when unresolved identity conflicts would materially alter the scientific interpretation.

RULE

Every authoritative genealogy artifact SHALL preserve explicit uncertainty representations across all AWE generations.

RULE

Genealogy-specific validation SHALL extend, but SHALL NOT replace or weaken, the validation requirements inherited from the General Scientific Layer.

SECTION

ScientificEvolutionArchitectureBinding

PURPOSE

DefineHowTheGenealogyModelAdoptsTheScientificEvolutionArchitectureDefinedByTheGeneralScientificLayer.

CONFORMS_TO

GSL.ScientificEvolutionArchitecture

RULE

The Genealogy Model SHALL adopt the Scientific Evolution Architecture defined by the General Scientific Layer.

RULE

The Genealogy Model SHALL use the General Scientific Layer candidate lifecycle for all normative specification development.

RULE

The Genealogy Model SHALL NOT redefine candidate management, review, integration, consolidation, publication or archival processes already defined by the General Scientific Layer.

RULE

Genealogy-specific evolution requirements SHALL extend only the scientific content under review and SHALL NOT modify the inherited evolution process.

RULE

Every normative Genealogy Model change SHALL remain traceable through the inherited Scientific Evolution Architecture.

INHERITED_EVOLUTION_PROCESSES

SpecificationCandidateManagement
CandidateLifecycle
ReviewAndResolution
ArchitectureIntegrationReview
ControlledConsolidation
EditorialCleanup
EvidenceBasedValidation
ReleaseBoundArchival
ControlledArtifactTransfer

RULE

The Genealogy Model SHALL reference the inherited evolution processes and SHALL NOT define competing GM-specific equivalents.

RULE

Genealogy-specific reviews MAY define domain-specific review criteria, but their lifecycle, authority and archival handling SHALL remain governed by the General Scientific Layer.

SUBSECTION

GenealogySpecificEvolutionReviewCriteria

PURPOSE

DefineGenealogySpecificReviewCriteriaAppliedWithinTheInheritedScientificEvolutionArchitecture.

REVIEW_CRITERIA

GenealogicalMethodConsistency
SourceModelConsistency
ArtifactSpecializationConsistency
ProjectProfileConsistency
ResearchRecordSetIntegrity
ExportModelConsistency

RULE

Genealogy-specific reviews SHALL evaluate only genealogy-specific scientific content.

RULE

General Scientific Layer process conformance SHALL be assumed through inheritance and SHALL NOT be revalidated by Genealogy Model reviews.

RULE

Every genealogy-specific review finding SHOULD identify the affected Genealogy Model artifact, inherited General Scientific Layer concept and proposed genealogy-specific resolution.

RULE

A Genealogy Model review SHALL distinguish between General Scientific Layer conformance findings and genealogy-specific modeling findings.

SECTION

ScientificWorkingContextBinding

PURPOSE

DefineHowTheGenealogyModelAdoptsTheScientificWorkingContextDefinedByTheGeneralScientificLayer.

CONFORMS_TO

GSL.ScientificWorkingContext

RULE

The Genealogy Model SHALL adopt the Scientific Working Context defined by the General Scientific Layer.

RULE

The Genealogy Model SHALL inherit the Human Role Profile, AI Role Profile and Collaboration Model without independent redefinition.

RULE

The Genealogy Model SHALL define only genealogy-specific working guidance that extends the inherited Scientific Working Context.

RULE

Genealogy-specific working guidance SHALL NOT redefine authority, responsibilities or interaction principles already defined by the General Scientific Layer.

RULE

Every genealogy-specific working recommendation SHALL remain traceable to the inherited Scientific Working Context.

INHERITED_WORKING_CONTEXT

HumanRoleProfile
AIRoleProfile
CollaborationModel
InteractionPrinciples
ScientificResponsibilities

RULE

The Genealogy Model SHALL reference inherited working context concepts and SHALL NOT define GM-specific equivalents for roles, collaboration or authority.

RULE

The Genealogy Model MAY define genealogy-specific working recommendations only where they extend genealogical research practice.

SUBSECTION

GenealogySpecificWorkingGuidance

PURPOSE

DefineGenealogySpecificWorkingRecommendationsExtendingTheInheritedScientificWorkingContext.

WORKING_GUIDANCE

EvidenceFirstResearch
SourceBeforeInterpretation
ProgressiveHypothesisValidation
ControlledIdentityResolution
ExplicitUncertaintyDocumentation
AuthoritativeResearchPersistence

RULE

Genealogical research SHOULD prioritize evidence collection before interpretation.

RULE

Every interpretation SHOULD remain explicitly linked to supporting scientific artifacts.

RULE

Identity resolution SHOULD be performed progressively and revised only through evidence-based validation.

RULE

Genealogical uncertainty SHOULD remain explicitly documented until resolved by sufficient evidence.

RULE

The authoritative Authoritative Genealogical Research Artifact Register SHOULD remain the primary persistent representation of ongoing research.

SECTION

ProjectModelAdaptationBinding

PURPOSE

DefineHowTheGenealogyModelAdoptsTheProjectModelAdaptationDefinedByTheGeneralScientificLayer.

CONFORMS_TO

GSL.ProjectModelAdaptation

RULE

The Genealogy Model SHALL adopt the Project Model Adaptation defined by the General Scientific Layer.

RULE

The Genealogy Model SHALL inherit the General Scientific Layer project adaptation architecture without independent redefinition.

RULE

The Genealogy Model SHALL define only genealogy-specific project adaptation guidance.

RULE

Genealogy-specific project adaptations SHALL specialize the inherited General Scientific Layer project adaptation model and SHALL NOT replace or weaken it.

RULE

Every Genealogy Model project profile SHALL remain traceable to the inherited Project Model Adaptation.

SECTION

ControlledArtifactTransferBinding

PURPOSE

DefineHowTheGenealogyModelAdoptsTheControlledArtifactTransferDefinedByTheGeneralScientificLayer.

CONFORMS_TO

GSL.ControlledArtifactTransfer

RULE

The Genealogy Model SHALL adopt the Controlled Artifact Transfer architecture defined by the General Scientific Layer.

RULE

The Genealogy Model SHALL inherit the General Scientific Layer transfer process, transfer authority and transfer traceability requirements without independent redefinition.

RULE

The Genealogy Model SHALL define only genealogy-specific transfer guidance.

RULE

Genealogy-specific transfer definitions SHALL specialize the inherited Controlled Artifact Transfer model and SHALL NOT replace or weaken it.

RULE

Every genealogy-specific artifact transfer SHALL preserve traceability to the originating authoritative Scientific Artifact.

INHERITED_TRANSFER_MODEL

GSL.ControlledArtifactTransfer
GSL.TransferAuthority
GSL.TransferTraceability
GSL.TransferIntegrity
GSL.TransferValidation
GSL.TransferClassification
GSL.TransferProvenance

RULE

The Genealogy Model SHALL reference the inherited Controlled Artifact Transfer model and SHALL NOT define GM-specific equivalents for general transfer processes, authority, provenance, integrity or validation.

SECTION

GenealogySpecificArtifactTransferGuidance

PURPOSE

DefineGenealogySpecificRequirementsForControlledTransferOfGenealogicalResearchArtifacts.

TRANSFER_GUIDANCE

AuthoritativeGenealogicalResearchArtifactRegisterTransfer
GenealogicalSourceArtifactTransfer
GenealogicalRelationshipArtifactTransfer
GenealogicalEventArtifactTransfer
GenealogicalExportProfiles
GenealogicalTransferConstraints

RULE

A Authoritative Genealogical Research Artifact Register SHALL remain the authoritative research representation after every controlled transfer.

RULE

Every transferred genealogical artifact SHALL preserve complete traceability to the originating Scientific Artifacts and supporting evidence.

RULE

Transfers between genealogy-specific artifact types SHALL preserve identity resolution, relationship consistency and explicit uncertainty representation.

RULE

Genealogy-specific export profiles SHALL explicitly declare whether the resulting representation is lossless, lossy or non-authoritative.

RULE

Lossy genealogy-specific transfers SHALL explicitly identify which scientific information cannot be represented in the target format.

RULE

A genealogy-specific transfer SHOULD preserve every reusable scientific relationship whenever the target representation supports it.

RULE

Transfer-specific transformations SHALL remain reproducible through documented Processing Profiles.

RULE

A genealogy-specific transfer SHALL NOT silently modify genealogical evidence, relationships, identity assignments or uncertainty states.

SECTION

ScientificArtifactLifecycleBinding

PURPOSE

DefineHowTheGenealogyModelAdoptsTheScientificArtifactLifecycleDefinedByTheGeneralScientificLayer.

CONFORMS_TO

GSL.ScientificArtifactLifecycle

INHERITS

GSL.ArtifactLifecycleState
GSL.ArtifactLifecycleTransition

RULE

The Genealogy Model SHALL use the Scientific Artifact Lifecycle defined by the General Scientific Layer.

RULE

The Genealogy Model SHALL NOT redefine general artifact lifecycle states or transitions.

RULE

Genealogy-specific artifact types MAY define additional lifecycle constraints only where required by genealogical scientific content.

RULE

Genealogy-specific lifecycle constraints SHALL remain compatible with the inherited Scientific Artifact Lifecycle.

RULE

Artifact type, lifecycle state, artifact version and AWE generation SHALL remain distinguishable.

INHERITED_LIFECYCLE_MODEL

GSL.ScientificArtifactLifecycle
GSL.ArtifactLifecycleState
GSL.ArtifactLifecycleTransition
GSL.AuthoritativeWorkingElementLifecycle

RULE

The Genealogy Model SHALL reference the inherited lifecycle model and SHALL NOT define GM-specific equivalents for general artifact states, transitions, promotion, supersession or archival.

RULE

Genealogy-specific artifact status terms SHALL describe domain content or validation state and SHALL NOT act as replacements for inherited lifecycle states.

SUBSECTION

GenealogySpecificLifecycleConstraints

PURPOSE

DefineGenealogySpecificConstraintsAppliedInAdditionToTheInheritedScientificArtifactLifecycle.

LIFECYCLE_CONSTRAINTS

SourceTraceabilityPreservation
EvidenceStatePreservation
IdentityResolutionPreservation
RelationshipConsistencyPreservation
UncertaintyStatePreservation
RegisterMembershipConsistency

RULE

A Genealogical Research Artifact SHALL preserve source traceability across every inherited lifecycle transition.

RULE

A lifecycle transition SHALL NOT silently remove or weaken documented evidence states.

RULE

A lifecycle transition affecting a Person Artifact SHALL preserve prior identity-resolution decisions and their supporting evidence.

RULE

A lifecycle transition affecting Relationship or Event Artifacts SHALL preserve genealogical relationship consistency.

RULE

Explicit uncertainty states SHALL remain preserved until they are resolved through documented scientific validation.

RULE

An artifact entering or leaving the authoritative Genealogical Research Artifact Register SHALL do so through a controlled lifecycle transition.

RULE

A genealogy-specific lifecycle constraint SHALL extend, but SHALL NOT replace or weaken, the inherited Scientific Artifact Lifecycle.

SECTION

SemanticSpecializationBinding

PURPOSE

DefineHowTheGenealogyModelAddsGenealogicalSemanticOrientationWithoutIntroducingAlternativeCoreArtifactArchitectures.

DESCRIPTION

The General Scientific Layer defines the applicable General Scientific Artifact requirements.

The Genealogy Model preserves those requirements and adds only the minimum genealogy-specific semantic reference sets and Processing extension boundaries required for genealogical research.

Genealogy-specific Artifact Types SHALL be semantic specializations of the uniform Scientific Artifact architecture and SHALL NOT establish separate structural inheritance hierarchies within the Core.

RULE

Every Genealogy Model Scientific Artifact SHALL conform to all applicable General Scientific Layer requirements.

RULE

Genealogy-specific semantic reference types SHALL define only domain meaning and SHALL NOT redefine the uniform Scientific Artifact architecture.

RULE

Type-specific formation, constraints, interpretation and operational behavior SHALL be defined by the applicable Processing architecture.

RULE

Processing and project-specific specializations SHALL preserve semantic compatibility with their referenced Core meaning.

RULE

No semantic specialization MAY remove, replace or weaken inherited scientific requirements.

RULE

Every Processing or project-specific specialization SHALL preserve traceability to its referenced semantic type and applicable Processing definition.

SECTION

ArchitectureAxes

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

SECTION

FoundationalPrinciples

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

------------------------------------------------------------------------------

SECTION

ArchitectureOverview

PURPOSE

ProvideAHighLevelOverviewOfTheTargetRearchitectureWithoutChangingNormativeSemantics.

ARCHITECTURE_FLOW

Source
ScientificObservationArtifact
DerivedScientificArtifact
ScientificRelationship
ScientificCluster
AuthoritativeGenealogicalResearchArtifactRegister
PresentationView

RULE

The Architecture Overview SHALL describe the target migration architecture only.

RULE

Detailed normative semantics SHALL be defined in their respective chapters during later migration steps.

------------------------------------------------------------------------------

SECTION

ProjectInitialization

PURPOSE

DefineTheMinimumProjectInitializationRequiredToBeginGenealogicalScientificWork.

CONFORMS_TO

GSL.ScientificWorkingContext
GSL.ProjectModelAdaptation

DESCRIPTION

The Project Scientific Specification is progressively refined as additional project-specific information becomes available during scientific work.

RULE

The Genealogy Model SHOULD request only the minimum project-specific information required to begin scientific work.

RULE

A formal Project Scientific Specification SHALL NOT be required before scientific work can begin.

RULE

The initial project definition SHALL contain:

ResearchDomain
ResearchObjective

RULE

The Project Scientific Specification SHALL support progressive refinement throughout the scientific lifecycle.

RULE

Progressive Project Initialization SHALL preserve scientific traceability, reproducibility and Authoritative Working Element management throughout the complete scientific lifecycle.

SECTION

TransitionToScientificWorkingMode

PURPOSE

DefineTheNormativeTransitionFromProjectInitializationToScientificObservation.

CONFORMS_TO

GSL.ScientificWorkingContext

GSL.ProjectModelAdaptation

DESCRIPTION

Scientific work can begin before a complete Project Scientific Specification has been established.

#SUBSECTION

MinimumOperationalReadiness

PURPOSE

DefineTheMinimumConditionsRequiredToBeginControlledScientificWork.

RULE

The minimum project definition SHALL be sufficient to perform the next scientific activity.

RULE

A complete Project Scientific Specification SHALL NOT be required before scientific work begins.

#SUBSECTION

ProgressiveProjectCompletion

PURPOSE

DefineHowProjectInformationIsCompletedDuringScientificWork.

RULE

Additional project information SHOULD be requested only when required by the current scientific activity.

RULE

Project information MAY be refined throughout the scientific lifecycle.

#SUBSECTION

TransitionTrigger

PURPOSE

DefineTheNormativeTriggerForEnteringTheScientificObservationModel.

RULE

The transition to the Scientific Observation Model SHALL occur when the first source enters controlled scientific processing.

RULE

From this point onward all scientific activities SHALL conform to the applicable Processing Profile.

#SUBSECTION

TransitionResult

PURPOSE

DefineTheArchitecturalStateAfterSuccessfulTransition.

RESULT

ScientificObservationModelActive

ProcessingProfileControlled

ProjectInitializationCompleted

RULE

Scientific work SHALL continue under the Scientific Observation Model.

RULE

Project initialization SHALL thereafter support scientific work but SHALL no longer govern it.

ACTIVE_PART

ProjectScientificSpecification

PURPOSE

SpecializeTheInheritedProjectScientificSpecificationForGenealogicalResearch.

SPECIFICATION_TYPE

ProjectScientificSpecification

SPECIALIZES

GSL.ProjectScientificSpecification

INHERITED_PROJECT_MODEL

ProjectIdentity
ResearchDefinition
ProjectConfiguration
ProjectExtensions
ConfigurationExtensionBoundary
ProjectGovernanceBinding
ProjectModelAdaptation
ScientificWorkingContext

RULE

The Genealogy Model SHALL NOT redefine the inherited general project model.

RULE

A genealogical Project Scientific Specification SHALL preserve conformance with the inherited General Scientific Layer project model.

SECTION

GenealogyProjectBinding

PURPOSE

DefineTheGenealogyModelSpecificBindingOfAProjectScientificSpecification.

REQUIRED_FIELDS

AppliedGenealogyModelVersion

RULE

Every genealogical Project Scientific Specification SHALL identify the applied Genealogy Model version.

RULE

The applied Genealogy Model version SHALL remain traceable across all project versions.

SECTION

GenealogyProjectKnowledgeInputs

PURPOSE

DefineGenealogySpecificClassesOfProjectKnowledgeEnteringControlledScientificProcessing.

GENEALOGY_SPECIFIC_KNOWLEDGE_CLASSES

GenealogicalSourceMaterial
ImportedGenealogicalData
ReferencedGenealogicalResearch
LegacyGenealogicalDatabase

RULE

Imported genealogical knowledge SHALL preserve its original provenance.

RULE

Standardized external genealogical formats SHOULD enter the scientific workflow through documented Processing Profiles.

RULE

Technical conformance of imported genealogical data SHALL be evaluated separately from the scientific validity of its content.

SECTION

GenealogyProjectConfiguration

PURPOSE

DefineTheSelectionOfGenealogyModelComponentsForAConcreteProject.

GENEALOGY_SPECIFIC_CONFIGURATION_ELEMENTS

ActivatedProcessingProfiles
ActivatedGenealogicalArtifactTypes
ActivatedGenealogicalValidationExtensions
ResearchLanguageConfiguration

RULE

A genealogical Project Scientific Specification SHALL identify every activated Processing Profile.

RULE

A genealogical Project Scientific Specification SHALL identify every activated Genealogical Research Artifact type.

RULE

The project configuration SHALL preserve traceability to every activated Genealogy Model definition.

SECTION

GenealogyProjectExtensions

PURPOSE

DefineGenealogySpecificProjectExtensionsWithoutRedefiningTheInheritedProjectExtensionModel.

GENEALOGY_SPECIFIC_EXTENSION_ELEMENTS

ProjectProcessingProfiles
ProjectGenealogicalArtifactTypes
ProjectGenealogicalRules
ProjectGenealogicalConstraints
ProjectGenealogicalGlossary
ProjectGenealogicalValidationExtensions

RULE

Genealogy-specific project extensions SHALL specialize applicable Genealogy Model definitions.

RULE

A Project Processing Profile SHOULD define how imported genealogical data is transformed into traceable Genealogical Research Artifacts.

RULE

Genealogy-specific project extensions SHALL NOT weaken inherited General Scientific Layer or Genealogy Model requirements.

SECTION

GenealogySpecificProjectAdaptationGuidance

PURPOSE

DefineHowConcreteGenealogicalProjectsSpecializeTheGenealogyModelWithinTheInheritedProjectModelAdaptationArchitecture.

ADAPTATION_GUIDANCE

ResearchObjectiveBinding
SourceDomainSelection
ProcessingProfileSelection
GenealogicalArtifactSelection
UncertaintyPolicySelection
IdentityResolutionPolicySelection
ExportProfileSelection

RULE

A genealogical Project Scientific Specification SHALL identify the genealogical research objective that governs project-specific adaptation.

RULE

Project-specific source domains, Processing Profiles and Genealogical Research Artifact types SHALL be selected explicitly when they materially affect scientific processing.

RULE

A genealogical project SHALL document project-specific uncertainty and identity-resolution policies when they differ from the default Genealogy Model guidance.

RULE

Project adaptations SHOULD remain minimal and SHALL use existing Genealogy Model definitions whenever suitable definitions exist.

RULE

A project-specific genealogical extension SHALL document its scientific rationale, affected inherited definitions and expected impact.

RULE

Project-specific export profiles SHALL identify whether their outputs are lossless, lossy or non-authoritative.

RULE

A project adaptation SHALL NOT silently change the meaning of inherited genealogical artifact types, relationships, evidence states or validation requirements.

RULE

A reusable project-specific extension SHOULD be registered as a Genealogy Model specification candidate after successful practical validation.

CONFORMANCE

Required
---

------------------------------------------------------------------------------

2 ScientificObservationModel

PART

ScientificObservationModel

PURPOSE

DefineHowScientificObservationsAreCreatedFromControlledScientificProcessing.

SECTION

ScientificObservation

PURPOSE

DefineTheFundamentalScientificObservationProducedByControlledScientificProcessing.

DESCRIPTION

A Scientific Observation represents the first controlled persistent Scientific Artifact produced from a source.

A Scientific Observation preserves the observed scientific content together with its documented observational uncertainty.

A Scientific Observation SHALL remain independent from interpretation, normalization, hypothesis formation, identity resolution and scientific conclusions.

Scientific Observations constitute persistent scientific evidence.

RULE

Every Scientific Observation SHALL be a Scientific Artifact governed by the uniform Core Scientific Artifact requirements.

RULE

Its status as a Scientific Artifact SHALL NOT permit interpretive or normalizing modification of the observed content.

SUBSECTION

ScientificObservationIdentity

PURPOSE

DefineTheIdentityRequirementsForScientificObservations.

DESCRIPTION

A Scientific Observation is an independently identifiable scientific result produced through controlled scientific processing.

Its identity represents the observed scientific content and remains independent from the processed input, the applied processing activity and every derived Scientific Artifact.

REQUIRED_INFORMATION

ObservationIdentifier

RULE

Every Scientific Observation SHALL possess exactly one stable Observation Identifier.

RULE

The Observation Identifier SHALL remain stable while the scientific identity of the Scientific Observation remains unchanged.

RULE

A change to the Processing Record, Processing Profile or Processing Profile version SHALL NOT by itself require a new Observation Identifier.

RULE

Scientific Observations representing different scientific observations SHALL possess different Observation Identifiers.

RULE

The identity of a Scientific Observation SHALL remain distinguishable from:

InputIdentifier

ProcessingRecordIdentifier

ScientificArtifactIdentifier

DerivationIdentifier

RULE

Supersession or reprocessing SHALL preserve traceability to predecessor Scientific Observations.

RULE

The Observation Identifier SHALL remain suitable for persistent citation throughout the complete scientific lifecycle.

SUBSECTION

ScientificObservationStructure

PURPOSE

DefineTheMinimumStructuralRequirementsForScientificObservations.

DESCRIPTION

Every Scientific Observation represents one independently identifiable scientific observation together with the minimum information required to preserve its scientific meaning and its traceability to the observed input.

REQUIRED_INFORMATION

ObservationIdentifier

InputIdentifier

InputSegmentReference

ObservedContent

RULE

Every Scientific Observation SHALL contain the minimum information required for independent scientific interpretation.

RULE

Every Scientific Observation SHALL reference the input from which it originates.

RULE

Every Scientific Observation SHALL identify the specific input segment from which the observation was produced whenever the processed input contains more than one independently addressable segment.

RULE

ObservedContent SHALL remain distinguishable from metadata, provenance, uncertainty and validation information.

RULE

The structural definition of a Scientific Observation SHALL remain independent from its physical serialization.

SUBSECTION

ObservationRepresentation

STATUS

ReservedForFutureIntegration

PURPOSE

DefineHowScientificObservationsMayBeRepresented.

SUBSECTION

ObservationProvenance

STATUS

ReservedForFutureIntegration

PURPOSE

DefineTheProvenanceResponsibilitiesOfScientificObservations.

SUBSECTION

ObservationUncertainty

STATUS

ReservedForFutureIntegration

PURPOSE

DefineHowObservationSpecificUncertaintyWillBeRepresented.

SUBSECTION

ObservationValidation

STATUS

ReservedForFutureIntegration

PURPOSE

DefineHowScientificObservationsAreScientificallyValidated.

SUBSECTION

ObservationState

STATUS

ReservedForFutureIntegration

PURPOSE

ReserveTheScientificProcessingStateModelPendingGeneralScientificLayerReview.

SUBSECTION

ObservationVersioningAndReprocessing

STATUS

ReservedForFutureIntegration

PURPOSE

DefineHowScientificObservationsWillBeVersionedAndReprocessed.

RULE

Every Scientific Observation SHALL originate from controlled scientific processing.

RULE

Every Scientific Observation SHALL preserve complete provenance to the processed source.

RULE

A Scientific Observation SHALL remain distinguishable from interpretation and from Scientific Artifacts.

SECTION

ObservationInputClasses

PURPOSE

DefineTheGenealogySpecificClassesOfScientificInputThatMayEnterControlledObservationProcessing.

INPUT_CLASSES

GenealogicalSourceMaterial
ImportedGenealogicalData
ReferencedGenealogicalResearch
LegacyGenealogicalDatabase

RULE

Every input entering controlled scientific observation processing SHALL preserve its original provenance.

RULE

Imported genealogical data SHALL remain distinguishable from observations produced through controlled processing.

RULE

Referenced genealogical research SHALL be treated as source-derived scientific input and SHALL NOT be accepted as validated project knowledge without controlled evaluation.

RULE

Legacy genealogical databases SHALL preserve their original structure, provenance and known limitations when entering controlled processing.

RULE

Standardized external genealogical formats SHOULD enter the Scientific Observation Model through a documented Processing Profile.

RULE

Technical conformance of imported genealogical data SHALL be evaluated separately from the scientific validity of its content.

RULE

The classification of an input SHALL NOT determine the validity of observations derived from it.

SUBSECTION

ObservationInputProvenance

PURPOSE

DefineTheMinimumProvenanceRequirementsForInputsEnteringControlledObservationProcessing.

REQUIRED_INFORMATION

InputIdentifier
InputClass
OriginReference
AcquisitionOrImportContext
AppliedProcessingProfile
KnownLimitations

RULE

Every controlled observation process SHALL identify the input from which the Scientific Observation originates.

RULE

Known limitations of an input SHALL remain traceable to every materially affected Scientific Observation.

RULE

Transformation of an input representation SHALL NOT replace or obscure the original provenance reference.

SECTION

ObservationProcessingProfile

PURPOSE

DefineHowAProcessingProfileControlsTheCreationOfScientificObservations.

RULE

Every controlled observation process SHALL identify the applicable Processing Profile before Scientific Observations are created.

RULE

The selected Processing Profile SHALL be suitable for the input class, source characteristics and intended scientific activity.

RULE

A Processing Profile SHALL define the controlled operations by which source input is transformed into Scientific Observations.

RULE

Scientific Observations created under different Processing Profiles SHALL remain distinguishable when the applied processing materially affects their content or interpretation.

RULE

A Processing Profile SHALL NOT silently introduce genealogical interpretations that are not supported by the processed input.

RULE

Changes to an applied Processing Profile SHALL remain traceable and SHALL NOT retroactively alter existing Scientific Observations without controlled reprocessing.

SUBSECTION

ObservationGranularity

PURPOSE

DefineHowProcessingProfilesDetermineScientificObservationGranularity.

RULE

A Scientific Observation SHALL represent exactly one independently addressable scientific observation.

RULE

Multiple Scientific Observations MAY originate from the same scientific input.

RULE

Observation boundaries SHALL be determined by the applicable Processing Profile.

RULE

Specialized Processing Profiles MAY extend the Scientific Observation structure with additional observation-specific information provided that the mandatory structural requirements defined by the Scientific Observation Model remain preserved.

SUBSECTION

ProcessingProfileSelection

PURPOSE

DefineTheSelectionRequirementsForProcessingProfilesUsedInScientificObservation.

SELECTION_FACTORS

InputClass
SourceForm
SourceLanguage
WritingSystem
DocumentStructure
ScientificObjective
RequiredObservationGranularity
KnownInputLimitations

RULE

A Processing Profile SHALL be selected explicitly when its choice materially affects scientific processing.

RULE

The selection SHALL remain traceable to the processed input and every Scientific Observation produced from it.

RULE

Only undefined Processing Profile parameters required for the next scientific activity SHOULD be requested.

RULE

Previously confirmed Processing Profile parameters SHOULD be reused when their applicability remains unchanged.

RULE

A project-specific Processing Profile MAY be used when no existing Genealogy Model Processing Profile adequately represents the required scientific method.

RULE

A project-specific Processing Profile SHALL document its scientific rationale, inherited definitions and project-specific extensions.

SUBSECTION

ObservationProcessingRecord

PURPOSE

DefineTheMinimumRecordOfControlledProcessingThatProducesScientificObservations.

REQUIRED_INFORMATION

ProcessingRecordIdentifier
InputIdentifier
AppliedProcessingProfile
AppliedProfileVersion
ResolvedProcessingParameters
ProcessingActivity
ProducedObservationIdentifiers
ProcessingAgentReferences
ProcessingTimeReference
KnownProcessingLimitations

RULE

Every Scientific Observation SHALL remain traceable to exactly one or more documented Processing Records.

RULE

A Processing Record SHALL preserve the Processing Profile version and resolved parameters applied during processing.

RULE

Known processing limitations SHALL remain traceable to every materially affected Scientific Observation.

RULE

Reprocessing the same input SHALL create a new Processing Record when the Processing Profile, profile version or material processing parameters change.

SECTION

ObservationProcessing

PURPOSE

DefineHowControlledScientificProcessingProducesScientificObservations.

SUBSECTION

ProcessingStages

STAGES

InputPreparation
ControlledObservation
ObservationRecording
ObservationValidation
ObservationCompletion

RULE

Every Scientific Observation SHALL be produced through the defined processing stages.

RULE

The order of processing stages SHALL remain traceable.

SUBSECTION

ObservationIntegrity

PURPOSE

PreserveTheScientificIntegrityOfScientificObservationsAsScientificEvidence.

RULE

Scientific Observations SHALL remain distinguishable from interpretation, normalization, hypothesis formation, identity resolution and scientific conclusions.

RULE

Observation processing SHALL NOT silently introduce unsupported assumptions.

RULE

Known uncertainties SHALL remain explicitly documented as part of the Scientific Observation.

RULE

Corrections, normalizations and subsequent scientific interpretations SHALL remain fully traceable to the original Scientific Observation.

RULE

Corrections, normalizations and subsequent scientific interpretations SHALL NOT modify the preserved observed content.

RULE

Scientific Observations SHALL remain immutable scientific evidence once observation processing has been completed. Subsequent scientific refinement SHALL be performed exclusively through derived Scientific Artifacts while preserving traceability to the original Scientific Observation.

SUBSECTION

ObservationCompletionCriteria

PURPOSE

DefineWhenObservationProcessingIsScientificallyComplete.

RULE

Observation processing SHALL be considered complete only after every required Processing Profile step has been executed.

RULE

Incomplete observations SHALL remain explicitly identifiable.

RULE

Material changes to the Processing Profile SHALL require controlled reprocessing.

RULE

Reprocessing SHALL create a new Processing Record.

RULE

Reprocessing SHALL preserve previous Observation history.

SECTION

ObservationTransitionToDerivedScientificArtifacts

PURPOSE

DefineHowValidatedScientificObservationArtifactsContributeToDerivedScientificArtifacts.

SUBSECTION

DerivationConditions

PURPOSE

DefineTheConditionsRequiredForScientificArtifactDerivation.

RULE

Derived Scientific Artifacts MAY be formed from traceable Scientific Observations and, where scientifically justified, from other traceable Scientific Artifacts.

RULE

Derivation from a Scientific Observation SHALL occur only after the required Observation Processing stages have been completed.

RULE

Required validation defined by the applicable Processing Profile SHALL be satisfied before derivation.

RULE

Derived Scientific Artifact formation SHALL preserve every originating Scientific Observation unchanged.

RULE

Derivation SHALL create new Derived Scientific Artifacts.

RULE

Derivation SHALL NOT replace the originating Scientific Observation.

RULE

Derivation SHALL NOT normalize the originating Scientific Observation.

RULE

Derivation SHALL NOT reinterpret the originating Scientific Observation.

SUBSECTION

DerivationTraceability

PURPOSE

PreserveCompleteTraceabilityBetweenObservationsAndDerivedArtifacts.

RULE

Every Derived Scientific Artifact SHALL preserve complete traceability to all originating Scientific Observations and Scientific Artifacts.

RULE

Scientifically relevant information SHALL NOT be silently lost during derivation; every intentional selection, reduction or transformation SHALL remain documented and traceable.

RULE

Derived Scientific Artifacts are formed from traceable scientific inputs while preserving complete scientific traceability.

RULE

Every derived scientific statement SHALL remain traceable to its originating Scientific Observations, Scientific Artifacts or both.

RULE

Derivation traceability SHALL preserve the distinction between observed evidence and derived scientific interpretation.

SUBSECTION

ArtifactFormationRules

PURPOSE

DefineHowDerivedScientificArtifactsAreFormedFromTraceableScientificInputs.

RULE

One Scientific Observation MAY contribute to multiple Derived Scientific Artifacts.

RULE

Multiple Scientific Observations and existing Scientific Artifacts MAY contribute to one Derived Scientific Artifact.

RULE

Applied Processing Profiles and explicit uncertainty representations SHALL remain traceable.

RULE

Derived Scientific Artifacts MAY represent scientific interpretation, normalization, integration and hypothesis formation derived from traceable scientific inputs.

RULE

The creation, revision or replacement of a Scientific Artifact SHALL NOT modify the originating Scientific Observation.

RULE

Multiple Scientific Artifacts MAY coexist when different scientifically traceable interpretations are derived from the same Scientific Observation.

SUBSECTION

ArtifactDerivationRecord

PURPOSE

DefineTheMinimumRecordOfArtifactDerivation.

REQUIRED_INFORMATION

DerivationIdentifier
SourceObservationIdentifiers
ProducedArtifactIdentifiers
AppliedDerivationRules
ResponsibleProcessingProfile
DerivationTimestamp
KnownDerivationLimitations

RULE

Every artifact derivation SHALL be documented through an Artifact Derivation Record.

RULE

The derivation from a Scientific Observation Artifact to a Derived Scientific Artifact SHALL preserve traceability and applicable Processing Profile conformance.

------------------------------------------------------------------------------
SUBSECTION

ObservationUncertainty

PURPOSE

DefineHowScientificObservationsRepresentScientificUncertaintyWithoutIntroducingInterpretation.

DESCRIPTION

Scientific uncertainty is an inherent property of scientific observation.

Whenever the observed content cannot be determined with complete confidence, the uncertainty SHALL be documented as part of the Scientific Observation.

The documentation of uncertainty SHALL describe the limitations of the observation itself.

Scientific uncertainty documents only the limitations of the observation itself.

The scientific evaluation, reduction or resolution of uncertainty belongs exclusively to Scientific Artifacts and SHALL remain independent from Scientific Observations.

RULE

Scientific Observations SHALL distinguish observed content from uncertainty information.

RULE

Uncertainty SHALL describe limitations of the observation and SHALL NOT introduce assumptions or interpretations.

RULE

Every documented uncertainty SHALL remain traceable to the observed input.

RULE

The absence of documented uncertainty SHALL NOT be interpreted as proof of correctness.

RULE

Additional uncertainty classifications MAY be introduced by specialized Processing Profiles provided that the original observed content remains preserved.

RULE

Scientific uncertainty SHALL describe only the limitations of the observation itself.

RULE

Scientific uncertainty SHALL NOT express the probability or correctness of subsequent scientific interpretations.

RULE

The evaluation of hypotheses, assumptions and scientific conclusions belongs exclusively to Scientific Artifacts and SHALL remain independent from Scientific Observations.

RULE

Scientific Observations SHALL preserve documented uncertainty as part of the scientific evidence.

The reduction, resolution or normalization of uncertainty SHALL occur exclusively within Scientific Artifacts and SHALL NOT modify the original Scientific Observation.

------------------------------------------------------------------------------

3 ScientificArtifactModel

PART

ScientificArtifactModel

PURPOSE

DefineTheMinimalGenealogySpecificScientificArtifactArchitectureAndItsExtensionBoundary.

RESPONSIBILITY

DefineGenealogySpecificArtifactCore
DefineArtifactMinimalRequirements
DefineArtifactExtensionPrinciples
SeparateArtifactStructureFromScientificWorkingMethod

RULE

New Artifact Types SHALL only be introduced when no existing Core Artifact Type can represent the required scientific responsibility without violating architectural separation.

RULE

Every newly introduced Artifact Type SHALL define exactly one independent scientific responsibility.

RULE

New Artifact Types SHALL remain compatible with existing Core Artifact semantics and SHALL NOT redefine previously established responsibilities.

RULE

Architectural extensions SHALL be introduced through the normative review and consolidation process before becoming part of the Core Genealogy Model.

RULE

An authoritative working artifact MAY remain scientifically incomplete during controlled iterative development, provided that its current incompleteness remains explicitly identifiable.

RULE

Scientific persistence SHALL NOT require scientific completeness.

RULE

Scientific completeness SHALL be evaluated during validation and SHALL NOT be treated as a prerequisite for artifact existence.

SECTION

ScientificArtifactModelPurpose

PURPOSE
DESCRIPTION

Scientific Artifact is the persistent scientific abstracted representation of a single identifiable unit of scientific knowledge that can be referenced, related, evaluated and reused throughout the scientific lifecycle.

RULE

The Scientific Artifact Model SHALL define only genealogy-specific artifact semantics not already defined by the General Scientific Layer.

RULE

The Scientific Artifact Model SHALL remain distinguishable from scientific integration, validation, hypothesis formation and review methodology.

RULE

Scientific working methodology SHALL be defined in Appendix D and SHALL NOT be represented as mandatory artifact structure unless persistence of a scientific statement is required.

SECTION

CoreArtifactTypeReferenceSet

PURPOSE

ProvideTheMinimumGenealogicalArtifactTypeReferenceSetRequiredForApplicableProcessingDefinitions.

CORE_ARTIFACT_TYPE_REFERENCE_SET

RegisteredSource
ScientificObservation
PersonIdentity
Event

RULE

The Core Artifact Type Reference Set SHALL define the minimum genealogy-specific artifact meanings required to guide conforming Processing definitions.

RULE

Artifact Types contained in the Core Artifact Type Reference Set SHALL NOT receive different Core treatment solely because of their Type.

RULE

All Scientific Artifacts SHALL remain subject to the same Core requirements for identity, persistence, provenance, relationships, evidence, uncertainty and validation.

RULE

The applicable Processing architecture SHALL define the formation, interpretation, constraints and operational treatment of the referenced Artifact Types.

RULE

The Core Artifact Type Reference Set SHALL be treated as an open minimum reference set and SHALL NOT be interpreted as a closed ontology.

RULE

Additional Artifact Types MAY be defined by Processing Profiles or project adaptation when required by scientific responsibility.

RULE

A new referenced Artifact Type SHOULD be introduced only when its independent scientific meaning cannot be represented adequately through an existing reference type, Event specialization or Scientific Relationship.

RULE

Every Artifact Type contained in the Core Artifact Type Reference Set SHALL define exactly one independent genealogy-specific semantic responsibility.

SUBSECTION

RegisteredSource

PURPOSE
DESCRIPTION

Registered Source is the scientific representation of an independently identifiable object registered to provide a persistent reference and connection point for corresponding scientific content.

RULE

A RegisteredSource SHALL represent the semantic concept of one independently addressable scientific source.

RULE

RegisteredSource SHALL provide semantic orientation only and SHALL NOT define type-specific Core structure or Core behavior.

RULE

The registration, acquisition, import, management, validation and operational treatment of RegisteredSource Artifacts SHALL be governed by the applicable Processing architecture.

RULE

A RegisteredSource SHALL remain distinguishable from ScientificObservation, PersonIdentity, Event and every other referenced Artifact Type.

SUBSECTION

ScientificObservation

PURPOSE

ProvideTheMinimumGenealogicalSemanticReferenceForProcessingDefinitionsThatRepresentScientificObservations.

RULE

ScientificObservation SHALL denote the semantic concept of one independently identifiable evidence-preserving Scientific Artifact.

RULE

ScientificObservation SHALL conform to the Scientific Observation Model defined in Chapter 2.

RULE

ScientificObservation SHALL provide semantic orientation only and SHALL NOT define type-specific Core structure or Core behavior.

RULE

Observation identity, structure, provenance, uncertainty, validation and processing SHALL be governed by the uniform Scientific Artifact requirements, the Scientific Observation Model and the applicable Processing architecture.

RULE

ScientificObservation SHALL remain distinguishable from RegisteredSource, PersonIdentity, Event and every other referenced Artifact Type.

SUBSECTION

PersonIdentity

PURPOSE

ProvideTheMinimumGenealogicalSemanticReferenceForProcessingDefinitionsThatRepresentAnIndependentlyAddressablePersonIdentity.

RULE

PersonIdentity SHALL denote the persistent scientific identity of one person.

RULE

PersonIdentity SHALL provide semantic orientation only and SHALL NOT define type-specific Core structure or Core behavior.

RULE

Genealogical properties and assertions concerning a PersonIdentity SHALL be represented through independently persistent Scientific Artifacts and Relationships.

RULE

The applicable Processing architecture SHALL define the formation, interpretation, constraints and operational treatment of PersonIdentity Artifacts.

RULE

PersonIdentity SHALL remain distinguishable from RegisteredSource, ScientificObservation, Event and every other referenced Artifact Type.

SUBSECTION

Event

PURPOSE

ProvideTheMinimumGenealogicalSemanticReferenceForProcessingDefinitionsThatRepresentAnIndependentlyAddressableGenealogicalEvent.

RULE

Event SHALL denote the semantic concept of one independently identifiable genealogical event.

RULE

Event SHALL provide semantic orientation only and SHALL NOT define type-specific Core structure or Core behavior.

RULE

The applicable Processing architecture SHALL define the formation, interpretation, constraints, specialization and operational treatment of Event Artifacts.

RULE

The scientific identity of an Event SHALL remain independent from evidence, uncertainty, validation and hypothesis assessment.

RULE

Event SHALL remain distinguishable from RegisteredSource, ScientificObservation, PersonIdentity and every other referenced Artifact Type.

SECTION

EventSpecializations

PURPOSE

ProvideReusableGenealogicalSemanticReferenceEventsForProcessingDefinitions.

REFERENCE_EVENT_SPECIALIZATIONS

BirthEvent
BaptismEvent
MarriageEvent
DeathEvent
BurialEvent
ResidenceEvent
MigrationEvent
OtherGenealogicalEvent

RULE

Reference Event Specializations SHALL provide reusable genealogy-specific semantic orientation for Processing definitions.

RULE

Reference Event Specializations SHALL NOT define type-specific Core structure or Core behavior.

RULE

The applicable Processing architecture SHALL define the formation, interpretation, constraints and operational treatment of Event Specializations.

RULE

The Reference Event Specializations SHALL be treated as an open reference set and SHALL NOT be interpreted as a closed event taxonomy.

RULE

Projects MAY define additional Event Specializations when required by scientific responsibility while remaining compatible with the Core Event reference.

SECTION

ArtifactMinimalRequirements

PURPOSE

DefineTheMinimumScientificRequirementsForPersistentScientificArtifacts.

RULE

Every persistent Scientific Artifact SHALL contain or participate in at least one meaningful scientific statement.

RULE

Every persistent Scientific Artifact SHOULD remain connected to at least one other Scientific Artifact or persistent scientific statement through a traceable scientific relationship.

RULE

Scientific completeness SHALL be determined by the scientific meaning represented by the Artifact and SHALL NOT depend on its referenced Artifact Type.

RULE

Administrative or semantically empty structures SHALL NOT by themselves be regarded as scientifically complete.

RULE

The applicable Processing architecture MAY define additional completeness criteria for referenced Artifact Types provided that the uniform Core Artifact architecture remains unchanged.

PRINCIPLE

MeaningBeforeStructure

PRINCIPLE

UniformArtifactCompleteness

PRINCIPLE

ScientificConnectivity

SECTION

ArtifactExtensionPrinciples

PURPOSE

DefineHowScientificArtifactsMAYBeExtendedWithoutChangingTheUniformCoreArchitecture.

RULE

The Core SHALL define only the minimum scientific architecture required for persistent Scientific Artifacts.

RULE

Referenced Artifact Types SHALL provide semantic orientation only and SHALL NOT introduce alternative Core architectures.

RULE

The applicable Processing architecture MAY define additional Artifact Types, semantic reference sets, constraints and operational behavior.

RULE

Processing extensions SHALL remain compatible with the uniform Scientific Artifact architecture defined by the Core.

RULE

Projects MAY introduce domain-specific Processing Profiles without modifying the normative Core.

PRINCIPLE

StableCore

PRINCIPLE

OpenProcessingExtensions

PRINCIPLE

SemanticCompatibility

PURPOSE

Define the normative execution boundary and informative supporting material of the Genealogy Model.

# 6.1 Purpose and Scientific Responsibility

## Scientific Responsibility

The **Authoritative Genealogical Research Artifact Register (AGRAR)** defines the authoritative management framework for all addressable scientific elements belonging to a genealogy research project.

Its scientific responsibility is limited to establishing, maintaining, and preserving authoritative register membership throughout the complete lifecycle of the register.

The register shall not define, interpret, or modify the scientific semantics of the referenced elements.

## Normative Requirements

The register shall:

- provide a single authoritative representation of register membership;
- maintain stable identification of register entries;
- support authoritative register revisions;
- preserve traceability throughout all register revisions;
- remain independent of the semantic content of referenced scientific elements.

## Scope Boundaries

This chapter shall not define:

- scientific observations;
- scientific artifacts;
- scientific relationships;
- scientific clusters;
- processing procedures;
- persistence technologies;
- serialization formats;
- implementation-specific execution mechanisms.

These responsibilities are defined by their respective GM Core chapters or by the GM Execution specification.

## Conformance Criteria

A conformant implementation shall demonstrate that:

- register membership is managed exclusively through AGRAR;
- every managed element is represented through a RegisterEntry;
- no semantic interpretation is performed by the register itself;
- register authority is preserved across all register revisions.

## 6.2 Architectural Position

### Scientific Responsibility

This section defines the architectural position of the **Authoritative Genealogical Research Artifact Register (AGRAR)** within the Genealogy Model Core.

AGRAR constitutes the management layer of the GM Core. It provides the authoritative framework for managing scientific elements without defining their scientific semantics or execution.

### Normative Requirements

AGRAR shall:

- operate as the authoritative management component of the GM Core;
- manage membership of addressable scientific elements;
- remain independent of semantic definitions provided by other GM Core chapters;
- remain independent of execution-specific implementations;
- provide the authoritative bridge between the semantic model and the execution layer.

### Architectural Relationships

AGRAR shall:

- inherit the scientific principles defined by the Foundation;
- manage the scientific elements defined by the Semantic Components;
- expose an execution-independent authoritative register model to the GM Execution.

### Scope Boundaries

AGRAR shall not:

- define scientific observations;
- define scientific artifacts;
- define scientific relationships;
- define scientific clusters;
- prescribe persistence technologies;
- prescribe serialization formats;
- prescribe implementation-specific execution behaviour.

### Conformance Criteria

A conformant implementation shall demonstrate that:

- AGRAR occupies the management layer of the GM Core;
- semantic responsibilities remain within the Semantic Components;
- execution responsibilities remain within the GM Execution;
- no architectural responsibility is assigned to more than one layer.

## 6.3 Project Binding and Register Singularity

### Scientific Responsibility

This section defines the normative relationship between a genealogy research project and its Authoritative Genealogical Research Artifact Register (AGRAR).

AGRAR is established by the research project and represents the single authoritative register for all addressable scientific elements belonging to that project.

### Normative Requirements

A genealogy research project shall:

- define exactly one authoritative AGRAR;
- manage all addressable scientific elements through that AGRAR;
- maintain the logical unity of AGRAR regardless of its physical implementation.

AGRAR shall not be partitioned into multiple authoritative registers based on artifact type or scientific category.

### Scope Boundaries

This section shall not define:

- register entries;
- register revisions;
- technical storage structures;
- database schemas;
- serialization formats;
- implementation-specific metadata.

Physical implementations may partition data internally, provided they preserve the normative concept of a single authoritative AGRAR.

### Conformance Criteria

A conformant implementation shall demonstrate that:

- exactly one AGRAR exists for each genealogy research project;
- all addressable scientific elements belong to that AGRAR;
- technical implementations do not create multiple authoritative registers;
- the logical integrity of AGRAR is preserved independently of execution mechanisms.

## 6.4 Register Entry

### Scientific Responsibility

This section defines the normative concept of a **RegisterEntry** within the Authoritative Genealogical Research Artifact Register (AGRAR).

A RegisterEntry represents the authoritative inclusion of one addressable scientific element in AGRAR.

The RegisterEntry defines register membership only. It neither defines nor modifies the scientific semantics of the referenced element.

### Normative Requirements

A RegisterEntry shall:

- represent the authoritative inclusion of exactly one addressable scientific element;
- remain independent of the scientific type of the referenced element;
- remain independent of implementation-specific representations;
- not define or modify scientific semantics;
- support the authoritative management principles established by AGRAR.

### Scope Boundaries

This section shall not define:

- the internal structure of scientific elements;
- property descriptions;
- processing behaviour;
- persistence models;
- serialization mechanisms;
- implementation-specific data structures.

These responsibilities belong to the GM Execution and its associated specifications.

### Conformance Criteria

A conformant implementation shall demonstrate that:

- every addressable scientific element included in AGRAR is represented through a RegisterEntry;
- RegisterEntries are independent of scientific element types;
- RegisterEntries do not introduce scientific semantics beyond register membership;
- implementation-specific representations preserve the normative concept of RegisterEntry.

## 6.5 Register Revision

### Scientific Responsibility

This section defines the application of the **General Scientific Layer (GSL)** concept of an authoritative scientific state to the **Authoritative Genealogical Research Artifact Register (AGRAR)**.

A **Register Revision** represents one authoritative scientific state of AGRAR. The scientific concepts governing authoritative states, scientific derivation, reconstruction and validation are defined by the applicable GSL specification. This chapter specifies only their genealogy-specific application to AGRAR.

### Normative Requirements

A Register Revision shall:

- represent one authoritative scientific state of AGRAR;
- conform to the applicable GSL requirements governing authoritative scientific states;
- preserve the authoritative integrity of AGRAR;
- provide the authoritative basis for genealogy-specific scientific processing.

The creation, modification and lifecycle management of Register Revisions shall be defined by the GM Execution.

### Scope Boundaries

This section shall not define:

- authoritative state models;
- scientific derivation;
- scientific reconstruction;
- scientific validation;
- generation algorithms;
- processing workflows;
- persistence technologies;
- serialization mechanisms.

These responsibilities are defined by the applicable GSL specification or by the GM Execution.

### Conformance Criteria

A conformant implementation shall demonstrate that:

- every Register Revision represents one authoritative scientific state of AGRAR;
- Register Revisions conform to the applicable GSL requirements;
- genealogy-specific processing preserves the authoritative meaning of each Register Revision;
- execution-specific implementations do not alter the normative concept of Register Revision.

## 6.6 Register Integrity

### Scientific Responsibility

This section defines the genealogy-specific application of scientific integrity to the **Authoritative Genealogical Research Artifact Register (AGRAR)**.

Register Integrity ensures that AGRAR remains the complete, authoritative and internally consistent management representation of all addressable scientific elements belonging to a genealogy research project.

The general scientific principles governing integrity are defined by the applicable **General Scientific Layer (GSL)**. This chapter specifies only their application to AGRAR.

### Normative Requirements

AGRAR shall:

- preserve the authoritative integrity of register membership;
- maintain the logical consistency of all RegisterEntries;
- preserve the completeness of the authoritative register;
- conform to the applicable GSL requirements governing scientific integrity.

The methods used to verify or enforce Register Integrity shall be defined by the GM Execution.

### Scope Boundaries

This section shall not define:

- scientific integrity models;
- validation algorithms;
- consistency checking procedures;
- processing workflows;
- persistence mechanisms;
- implementation-specific integrity controls.

These responsibilities are defined by the applicable GSL specification or by the GM Execution.

### Conformance Criteria

A conformant implementation shall demonstrate that:

- AGRAR preserves authoritative register integrity;
- RegisterEntries remain logically consistent;
- all applicable GSL integrity requirements are satisfied;
- execution-specific implementations preserve the normative integrity of AGRAR.

## 6.7 Execution Boundary

### Scientific Responsibility

This section defines the architectural boundary between the **Genealogy Model Core (GM Core)** and the **Genealogy Model Execution (GM Execution)** for the **Authoritative Genealogical Research Artifact Register (AGRAR)**.

The GM Core defines the normative scientific concepts governing AGRAR.

The GM Execution defines the implementation-specific realization of those concepts.

### Normative Requirements

The GM Core shall define:

- the normative concept of AGRAR;
- the normative concept of RegisterEntry;
- the normative concept of Register Revision;
- the normative concept of Register Integrity.

The GM Execution shall define:

- processing procedures;
- property descriptions;
- persistence models;
- serialization formats;
- execution workflows;
- implementation-specific data structures.

### Scope Boundaries

The GM Core shall not prescribe:

- implementation technologies;
- storage mechanisms;
- programming models;
- database schemas;
- exchange formats;
- execution-specific lifecycle management.

These responsibilities belong exclusively to the GM Execution.

### Conformance Criteria

A conformant implementation shall demonstrate that:

- normative scientific concepts are defined exclusively by the GM Core;
- implementation-specific realization is defined exclusively by the GM Execution;
- no execution-specific behaviour modifies the normative meaning of AGRAR.

## 6.8 Conformance Requirements

### Scientific Responsibility

This section defines the normative conformance requirements for an implementation of the Authoritative Genealogical Research Artifact Register (AGRAR).

It consolidates the normative requirements established throughout this chapter without introducing additional scientific concepts.

### Normative Requirements

A conformant implementation shall demonstrate that:

- exactly one AGRAR exists for each genealogy research project;
- all addressable scientific elements are managed through AGRAR;
- RegisterEntry is used solely as the normative representation of authoritative register membership;
- Register Revisions conform to the applicable General Scientific Layer (GSL) requirements for authoritative scientific states;
- Register Integrity conforms to the applicable GSL requirements for scientific integrity;
- implementation-specific behaviour remains within the responsibilities of the GM Execution.

### Scope Boundaries

This section shall not define:

- additional scientific concepts;
- implementation-specific conformance tests;
- execution-specific validation procedures;
- certification processes.

These responsibilities belong to the applicable GSL, the GM Execution or external conformance procedures.

### Conformance Criteria

A conformant implementation shall satisfy all normative requirements defined in Sections 6.1 through 6.7.

# 7.1 Purpose and Scientific Responsibility

## Scientific Responsibility

This chapter defines the normative architectural interface between the **Genealogy Model Core (GM Core)** and the **Genealogy Model Execution (GM Execution)**.

Its scientific responsibility is limited to establishing the authoritative boundary between normative scientific concepts defined by the GM Core and their operational realization within the GM Execution.

This chapter shall define the responsibilities assigned to each architectural layer without prescribing implementation-specific execution mechanisms.

The scientific semantics defined by the GM Core shall remain authoritative and shall not be altered by the GM Execution.

## Normative Requirements

The architectural interface shall:

- establish the normative boundary between the GM Core and the GM Execution;
- preserve the scientific authority of all concepts defined by the GM Core;
- ensure that operational behavior conforms to the normative semantics of the GM Core;
- permit execution-specific realization without modifying Core semantics;
- provide a stable architectural foundation for future execution specifications.

## Scope Boundaries

This chapter shall not define:

- execution procedures;
- processing profiles;
- validation procedures;
- persistence technologies;
- serialization formats;
- implementation-specific data structures;
- operational workflows.

These responsibilities belong exclusively to the GM Execution and its associated specifications.

## Conformance Criteria

A conformant implementation shall demonstrate that:

- the responsibilities of the GM Core and the GM Execution are clearly separated;
- execution-specific behavior preserves the normative semantics defined by the GM Core;
- no execution-specific implementation redefines, weakens, or replaces normative Core concepts;
- all operational genealogy processing is performed within the architectural responsibilities assigned to the GM Execution.

# 7.2 Architectural Position

## Scientific Responsibility

This section defines the architectural position of the **GM Execution** within the Genealogy Model architecture.

The GM Execution constitutes the operational realization of the normative scientific concepts defined by the **GM Core**.

It provides the execution environment for genealogy-specific scientific processing while preserving the scientific semantics established by the GM Core and the governing principles inherited from the applicable General Scientific Layer (GSL).

## Normative Requirements

The GM Execution shall:

- operate as the exclusive operational layer of the Genealogy Model;
- implement the normative concepts defined by the GM Core;
- preserve the scientific semantics established by the GM Core;
- conform to the applicable requirements of the General Scientific Layer (GSL);
- remain architecturally separated from the normative responsibilities of the GM Core.

## Architectural Relationships

The GM Execution shall:

- inherit the scientific principles defined by the applicable GSL;
- implement the normative concepts defined by the GM Core;
- provide the operational framework for genealogy-specific scientific processing;
- expose implementation-specific functionality without modifying normative Core concepts.

## Scope Boundaries

The GM Execution shall not:

- redefine normative scientific concepts established by the GM Core;
- modify the scientific meaning of Core objects;
- replace or weaken authoritative Core semantics;
- alter the scientific responsibilities assigned to the GM Core.

## Conformance Criteria

A conformant implementation shall demonstrate that:

- the GM Execution occupies the operational layer of the Genealogy Model architecture;
- all execution-specific behavior conforms to the normative concepts defined by the GM Core;
- architectural responsibilities remain clearly separated between the GSL, the GM Core and the GM Execution;
- implementation-specific extensions preserve the authoritative scientific semantics established by the GM Core.

# 7.3 Core Responsibilities

## Scientific Responsibility

This section defines the normative scientific responsibilities assigned exclusively to the **Genealogy Model Core (GM Core)**.

The GM Core establishes the authoritative scientific concepts, architectural principles, and normative semantics that govern the Genealogy Model independently of any operational realization.

These responsibilities constitute the immutable scientific foundation upon which all conforming implementations and execution specifications shall be based.

## Normative Requirements

The GM Core shall define the complete normative framework required to establish the scientific semantics, integrity, and architectural consistency of the Genealogy Model.

The GM Core shall remain implementation-independent and shall provide the authoritative scientific foundation for all conforming operational realizations.

## Scope Boundaries

This section shall not define implementation-specific operational behavior or prescribe how normative Core concepts are realized during execution.

Such responsibilities belong exclusively to the GM Execution and its associated specifications.

## Conformance Criteria

A conformant implementation shall demonstrate that:

- all normative scientific concepts originate from the GM Core;
- operational realizations preserve the authoritative scientific semantics established by the GM Core;
- no implementation-specific behavior modifies, weakens, or replaces the normative responsibilities assigned to the GM Core.

# 7.4 Execution Responsibilities

## Scientific Responsibility

This section defines the normative scientific responsibilities assigned exclusively to the **Genealogy Model Execution (GM Execution)**.

The GM Execution operationalizes the normative scientific concepts established by the **Genealogy Model Core (GM Core)** and provides the execution environment for genealogy-specific scientific processing.

These responsibilities ensure the consistent realization of the Genealogy Model while preserving the authoritative scientific semantics defined by the GM Core.

## Normative Requirements

The GM Execution shall operationalize the normative framework established by the GM Core while preserving its scientific semantics, integrity, and architectural consistency.

The GM Execution shall remain fully conformant with the authoritative concepts defined by the GM Core and shall not modify their normative meaning.

## Scope Boundaries

This section shall not define normative scientific concepts or prescribe the scientific semantics governing the Genealogy Model.

Such responsibilities belong exclusively to the GM Core.

## Conformance Criteria

A conformant implementation shall demonstrate that:

- all operational behavior conforms to the normative framework established by the GM Core;
- the authoritative scientific semantics defined by the GM Core are preserved throughout execution;
- no operational realization redefines, weakens, or replaces the normative concepts established by the GM Core.

# 7.5 Extension Boundary

## Scientific Responsibility

This section defines the normative architectural boundary governing extensions to the **Genealogy Model (GM)**.

Its scientific responsibility is limited to ensuring that extensions preserve the normative integrity, architectural consistency, and scientific semantics established by the **GM Core**.

## Normative Requirements

Extensions shall conform to the normative framework established by the GM Core.

Extensions may introduce additional operational capabilities, provided they remain consistent with the normative scientific concepts and architectural principles defined by the GM Core.

Extensions shall not modify, redefine, or weaken the authoritative scientific semantics established by the GM Core.

## Scope Boundaries

This section shall not define the structure, implementation, or lifecycle of individual extensions.

Such responsibilities belong to the GM Execution and its associated specifications.

## Conformance Criteria

A conformant extension shall demonstrate that:

- the normative scientific semantics established by the GM Core are preserved;
- architectural consistency is maintained;
- no extension introduces normative conflicts with the GM Core;
- implementation-specific functionality remains within the responsibilities of the GM Execution.

# 7.6 Conformance

## Scientific Responsibility

This section defines the normative conformance requirements governing the relationship between the **Genealogy Model Core (GM Core)** and the **Genealogy Model Execution (GM Execution)**.

Its scientific responsibility is limited to establishing the criteria by which an operational realization demonstrates conformity with the normative framework defined by the GM Core.

## Normative Requirements

A conforming operational realization shall preserve the normative scientific semantics, architectural principles, and integrity established by the GM Core.

Conformance shall be demonstrated through the consistent application of the normative framework without modification of its scientific meaning.

## Scope Boundaries

This section shall not define implementation-specific conformance procedures, certification methods, validation algorithms, or assessment processes.

Such responsibilities belong to the GM Execution, the applicable General Scientific Layer (GSL), or external conformance procedures.

## Conformance Criteria

A conformant implementation shall demonstrate that:

- the normative framework established by the GM Core is preserved throughout operational realization;
- architectural responsibilities remain consistent with the separation defined by the GM Core;
- implementation-specific behavior does not alter the authoritative scientific semantics established by the GM Core.

# 7.7 Transition to GM Execution

## Scientific Responsibility

This section defines the normative transition from the **Genealogy Model Core (GM Core)** to the **Genealogy Model Execution (GM Execution)**.

Its scientific responsibility is limited to establishing the architectural continuity between the normative scientific framework defined by the GM Core and its operational realization within the GM Execution.

## Normative Requirements

The GM Execution shall operationalize the normative framework established by the GM Core.

The transition from the GM Core to the GM Execution shall preserve the scientific semantics, architectural principles, and integrity defined by the GM Core.

The GM Execution shall extend the operational capabilities of the Genealogy Model without modifying the normative scientific foundation established by the GM Core.

## Scope Boundaries

This section shall not define the architecture, structure, or operational content of the GM Execution.

Such responsibilities belong exclusively to the GM Execution and its associated specifications.

## Conformance Criteria

A conformant transition shall demonstrate that:

- the GM Execution is based upon the normative framework established by the GM Core;
- the transition preserves the authoritative scientific semantics of the GM Core;
- operational realization remains fully consistent with the architectural principles defined by the GM Core.

# 10 Appendices

## Appendix A — Scientific Specification Consolidation Method (SSCM)

### Purpose

This appendix defines a recommended scientific methodology for consolidating complex scientific specifications while preserving architectural consistency, traceability, maintainability and extensibility.

### Consolidation Phases

#### Phase 1 — Responsibility Identification

Identify the unique scientific responsibility of every architectural component.

#### Phase 2 — Responsibility Migration

Assign every normative statement to exactly one architectural owner.

#### Phase 3 — Responsibility Consolidation

Ensure every architectural component answers one clearly defined scientific question.

#### Phase 4 — Architecture Validation

Validate the consolidated architecture using the following criteria:

- Single Owner Principle
- Completeness
- Redundancy Elimination
- Independent Extensibility

#### Phase 5 — Normative Consistency Review

Review every normative statement (RULE, MUST, SHALL, MUST NOT, SHOULD) for:

- Normative clarity
- Correct architectural ownership
- Redundancy elimination
- Contradiction-free behavior
- Objective testability

#### Phase 6 — Editorial Consolidation

Only after successful architectural validation perform:

- Terminology harmonization
- Structural ordering
- Cross-reference verification
- Editorial consistency
- Final numbering

### Architecture Review Questions

For every architectural component:

1. Does it have exactly one scientific responsibility?
2. Does every normative statement have exactly one owner?
3. Can the component evolve independently?
4. Does it integrate consistently into the complete scientific lifecycle?

# Appendix T — Architectural Core Concepts

## Purpose

Introduce the core architectural concepts of the Genealogy Model. Normative responsibilities, architectural boundaries and behavioral requirements remain defined by the corresponding Purpose and RULE sections of the specification.

## T.1 Scientific Artifact

Definition

A Scientific Artifact is an independently addressable persistent scientific representation forming the fundamental architectural building block from which specialized Scientific Artifacts are derived.

## T.2 Registered Source

Definition

A Registered Source is a Scientific Artifact representing a persistently registered source that may support Scientific Observations and other Scientific Artifacts.

## T.3 Scientific Observation

Definition

A Scientific Observation is a persistently recorded portion of information derived through observation of a Registered Source and made available as a reference for other Scientific Artifacts.

## T.4 Relationship

Definition

A Relationship is the scientific abstracted representation of a scientifically modeled edge connecting two or more Scientific Artifacts within the scientific graph.

## T.5 Evidence

Definition

The scientifically modeled connection between a Scientific Artifact and the supporting Scientific Artifacts or Registered Sources from which its scientific assertions are derived.

## T.6 Scientific Cluster

Definition

A Scientific Cluster is the scientific abstracted representation of a deterministic, reproducible and read-only structural workspace derived from Scientific Artifacts for subsequent scientific processing.

## T.7 Scientific Artifact as a Person

Definition

A Scientific Artifact as a Person is an aggregating Scientific Artifact whose scientific representation is composed of references to independently addressable Scientific Artifacts rather than by embedding scientific properties directly.

## T.8 Obscure Fact

Definition

An Obscure Fact is a scientific fact for which the available evidence is insufficient to support a reliable scientific assertion without introducing hypotheses or unsupported assumptions.
