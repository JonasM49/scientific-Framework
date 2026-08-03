# General Scientific Layer (GSL) v2.0 RC3 Authoritative Working Draft

DOCUMENT_IDENTIFIER

GSL-2.0-RC3

STATUS

BaselineValidated

VERSION

2.0 RC3 Baseline Validated

SUPERSEDES

GSL v2.0 RC2

------------------------------------------------------------------------------

WORKING_STATE

AWE_OBJECT_CODE

GSL

AWE_GENERATION
002

SOURCE_AWE

GSL_v2.0_RC2_Verified

EXPECTED_PARENT

GSL_v2.0_RC2_Verified

CURRENT_PHASE
BaselineCertified

LAST_COMPLETED
AWE_AuthoritativeWorkingPractice_Integration

NEXT_STEP
Maintenance

------------------------------------------------------------------------------
## 1. METADATA

VERSION
2.0 RC3 Authoritative Working Draft

STATUS
ReleaseCandidate

CURRENT_BASELINE
RC2 Verified

SUPERSEDES
GSL v2.0 RC2

DOCUMENT_TYPE
NormativeSpecification

DOCUMENT_IDENTIFIER
GSL-2.0-RC3

AUTHOR
JonasM49

PUBLISHED_AT
2026-07-15

CANONICAL_REPOSITORY
[<URL>](https://github.com/JonasM49/scientific-Framework)

LICENSE
CC BY-NC-SA 4.0

VALIDATION_STATUS
InheritedFromRC2Verified

NEXT_STAGE
WorkingDraftDevelopment

PURPOSE

ProfessionalizeScientificResearch
DeterministicHumanAICollaboration
EvidenceBased
Reproducible
Traceable

## 2. SCOPE

The General Scientific Layer (GSL) defines universal principles for
human–AI supported scientific work.

The GSL specifies scientific behavior, governance, validation,
traceability and specification evolution.

The GSL does not define domain-specific methods,
project-specific workflows or implementation-specific technologies.

These aspects MUST be defined by domain models,
project profiles or reference implementations.

## 3. FOUNDATION

RULE

RULE_NAME
EvidenceFirst

MUST
ObservationBeforeInterpretation
FactBeforeHypothesis
PrimarySourcesFirst
PreserveOriginal
NeverInvent
NeverGuess
MaintainTraceability
VersionEverything

## 4. SCIENTIFIC WORKFLOW

FLOW

Acquire
>
Prepare
>
Observe
>
Interpret
>
Correlate
>
Evaluate
>
Preserve
>
Report

## 5. HUMAN–AI COLLABORATION

PURPOSE

DeterministicScientificCollaboration

PRINCIPLE

AISuggests
HumanDecides
ProjectPersists
SystemExecutes

SCIENTIFIC_WORKING_CONTEXT

PURPOSE

DefineTheSharedScientificTaskContextFromWhichHumanAndAIRoleProfilesDeriveTheirCommonWorkingOrientation.

REQUIRED_ELEMENTS

PrimaryScientificObjective
ApplicableModels
ApplicableMethods
PrimaryTerminology
AuthoritativeWorkingRequirements
ProjectSpecificAdaptations

RULE

Every active scientific project SHOULD define one Scientific Working Context.

RULE

The Scientific Working Context MUST define the shared objective, terminology, applicable models and working methods for both human and AI participation.

RULE

Human Role Profiles and AI Role Profiles MUST inherit or reference the applicable Scientific Working Context.

RULE

Common scientific requirements MUST be defined once in the Scientific Working Context and MUST_NOT be duplicated independently in human and AI role profiles.

RULE

When domain or project specialization is required, the Scientific Working Context MUST be specialized by the applicable domain model and further adapted by the Project Scientific Specification.

RULE

Project adaptations MUST remain traceable to the inherited domain and General Scientific Layer context.

HUMAN_ROLE_PROFILE

PURPOSE

DefineHumanSpecificResponsibilitiesAndWorkingPreferencesWithinTheScientificWorkingContext.

TYPICAL_RESPONSIBILITIES

ScientificDecisionAuthority
EvidenceAcceptance
ProjectGovernance
ValidationApproval
InteractionPreferences

RULE

A Human Role Profile MUST describe task-oriented responsibilities and MUST_NOT be interpreted as an authorization or access-control profile.

AI_ROLE_PROFILE

PURPOSE

DefineThePrimaryTaskOrientedBehaviorOfTheAIWithinTheScientificWorkingContext.

REQUIRED_ELEMENTS

PrimaryAIBehavior
PrimaryExpertise
ScientificPriorities
InteractionBehavior
UncertaintyHandling

RULE

The active AI Role Profile MUST guide the primary expertise, terminology, priorities and interaction behavior of the AI.

RULE

An AI Role Profile MUST describe a preferred working orientation and MUST_NOT be interpreted as an exhaustive limitation of available knowledge or capabilities.

RULE

The AI MUST apply additional methodological, architectural, technical or implementation expertise when required for tasks within the active model or its controlled development.

RULE

A domain-oriented AI Role Profile MUST_NOT prevent controlled development of the applicable domain model or General Scientific Layer.

RULE

Domain application and model development MUST remain distinguishable working contexts.

RULE

When the scientific task changes materially, the active role profile SHOULD be reviewed and updated.

## 6. PARAMETER RESOLUTION

FLOW

DetectUndefinedParameter
>
GenerateRecommendation
>
ExplainAlternatives
>
ExplainConsequences
>
RequestHumanDecision
>
PersistDecision
>
ReuseDecision

RULE

RULE_NAME
AskOnlyForUndefinedMaterialParameters

MUST
ReuseConfirmedProjectDecisions
NeverAskAgainWithoutConflict
VersionChangedDecisions

## 7. DECISION CLASSES

AI_AUTONOMOUS

TemporaryFormatting
ReversiblePresentation

AI_SUGGEST_HUMAN_DECIDE

ReferenceSyntax
OutputStructure
RepositoryType
NamingConvention
ValidationThreshold

HUMAN_ONLY

ConfirmFacts
FreezeReferenceArtifacts
PromoteHypothesisToFact
OverrideProjectConvention

## 8. DECISION PERSISTENCE

RULE

RULE_NAME
PersistConfirmedProjectDecisions

MUST
MaintainDecisionHistory
ReusePersistedDecisions
WarnOnConflicts
RequireExplicitOverrideForChanges

## 9. INTERACTION

RULE

RULE_NAME
RequestPersistenceAfterValidatedResults

MUST
ExplainConsequencesOfMissingPersistence
SeparateSuggestionsFromDecisions
DocumentOpenQuestions
MaintainTransparency

PROGRESSIVE_SCIENTIFIC_ADOPTION

PURPOSE

ExposeOnlyTheMethodologicalComplexityRequiredForTheActiveWorkingContextWhilePreservingAPredictablePathToAdvancedUse.

ADOPTION_LEVELS

Application
ModelContribution
GeneralScientificLayerContribution

RULE

A conforming model SHOULD provide a default application-oriented working context for its primary user group.

RULE

Application-oriented users MUST be able to use the scientific workflow and applicable Authoritative Working Elements without understanding the full specification-development architecture.

RULE

Model development and General Scientific Layer development MUST remain optional extensions of ordinary scientific application.

RULE

The active model SHOULD explain relevant working methods at the point of project creation or first use without requiring a separate extensive handbook.

RULE

Adoption levels MUST remain changeable when the task or working context changes.

RULE

Progressive Scientific Adoption MUST_NOT classify persons by capability, age or technical background.

RULE

Progressive Scientific Adoption MUST guide presentation depth and working focus, not restrict access or authority.

## 10. KNOWLEDGE MODEL

MODEL

Source
Observation
Evidence
Fact
Hypothesis
ProjectKnowledge

RULE

RULE_NAME
SeparateWorkingKnowledgeFromPersistentKnowledge

MUST
PreserveEvidenceChain

## 11. QUALITY

RULE

RULE_NAME
CheckConsistency

MUST
DocumentConflicts
RecordUncertainty
EveryFactRequiresEvidence
EveryHypothesisRequiresReason

## 12. SCIENTIFIC ARTIFACT MODEL

PURPOSE

DefineTheUniversalScientificArtifactFoundationForAllModelsAndProjectsBasedOnTheGeneralScientificLayer.

ARCHITECTURAL_PRINCIPLE

Foundation
>
Reuse
>
Specialization

RULE

Every architectural responsibility MUST have exactly one normative owner.

RULE

Models and project specifications MUST reference, conform to or specialize an existing responsibility and MUST_NOT independently redefine it.

### 12.1 SCIENTIFIC ARTIFACT

BASE_TYPE

ScientificArtifact

PURPOSE

DefineTheCommonBaseTypeForPersistentScientificContentAndScientificProcessArtifacts.

RULE

Every Scientific Artifact MUST possess one stable artifact identity.

RULE

Every Scientific Artifact MUST identify its artifact type independently of its lifecycle state.

RULE

Artifact type, architectural layer and lifecycle state MUST remain distinguishable.

RULE

A domain model that adds domain-specific properties MUST specialize ScientificArtifact.

RULE

When no suitable domain artifact type exists, a Project Scientific Specification MUST specialize ScientificArtifact directly.

RULE

Specialization MUST_NOT weaken inherited mandatory requirements.

### 12.2 SCIENTIFIC ARTIFACT IDENTITY AND VERSION

REQUIRED_PROPERTIES

ArtifactIdentifier
ArtifactVersion
ArtifactType
OwningSpecification
LifecycleState

RULE

Artifact identity MUST remain stable throughout revisions of the same artifact lineage.

RULE

Artifact version MUST change whenever released or frozen content is modified.

RULE

Artifact version and Authoritative Working Element generation MUST remain distinguishable.

### 12.3 SCIENTIFIC ARTIFACT METADATA

REQUIRED_PROPERTIES

Title
Status
Version
Provenance
Traceability

OPTIONAL_PROPERTIES

Author
PublishedAt
CanonicalRepository
CanonicalDocument
License

RULE

Metadata MUST be sufficient to identify, interpret and verify the artifact within its scientific context.

### 12.4 SCIENTIFIC ARTIFACT PROVENANCE AND HISTORY

RULE

Every Scientific Artifact MUST preserve materially relevant origin, predecessor and derivation information.

RULE

Artifact history MUST remain traceable across revisions, specialization, promotion, supersession and archival.

RULE

Released historical states MUST_NOT be modified in place.

### 12.5 SCIENTIFIC ARTIFACT RELATIONSHIPS

RELATIONSHIP_CLASSES

Input
Predecessor
Derivation
Specialization
Validation
Promotion
Supersession
Archival

RULE

Scientific Artifact relationships MUST identify the related artifact and the relationship class.

RULE

Relationship semantics MUST remain distinguishable from lifecycle transitions and Authoritative Working Element lineage.

RULE

A domain model that defines domain-specific relationship semantics MUST specialize the applicable General Scientific Layer relationship class.

### 12.6 SCIENTIFIC ARTIFACT TAXONOMY

PURPOSE

ClassifyScientificArtifactsIndependentlyOfLifecycleStateAndDomainSpecificImplementation.

TAXONOMY_AXES

ScientificFunction
ArchitecturalLayer
SpecializationLineage

SCIENTIFIC_FUNCTION_CLASSES

SpecificationArtifact
ModelArtifact
ProjectSpecificationArtifact
WorkingArtifact
CandidateArtifact
ReviewArtifact
ValidationArtifact
ResultArtifact
ReferenceImplementationArtifact

RULE

The taxonomy MUST classify an artifact by scientific function and MUST_NOT use lifecycle states as artifact classes.

RULE

When an artifact performs more than one scientific function, every function MUST be explicitly declared and non-conflicting.

RULE

Domain-specific artifact classes MUST specialize an applicable General Scientific Layer function class whenever one exists.

RULE

The taxonomy MUST remain extensible and MUST_NOT require all domain-specific artifact classes to be enumerated in the General Scientific Layer.

### 12.7 SCIENTIFIC ARTIFACT CONFORMANCE

CONFORMANCE_FORMS

ConformsTo
InheritsFrom
Specializes

RULE

ConformsTo MUST be used when an artifact adopts a model without asserting a direct type-specialization relationship.

RULE

InheritsFrom or Specializes MUST be used only for genuine type specialization.

RULE

Lifecycle transitions MUST_NOT be represented as type inheritance.

RULE

Every specialization MUST preserve traceability to its direct base type.

### 12.8 SCIENTIFIC ARTIFACT INTEGRITY

RULE

RULE_NAME
MaintainArtifactHistory

MUST
MaintainArtifactTraceability
PreserveArtifactIntegrity
PreserveArtifactProvenance
PreserveRelationshipIntegrity

SHOULD

ReuseExistingArtifacts
MinimizeArtifactDuplication

MUST_NOT

ModifyReleasedArtifactsWithoutVersionIncrement
LoseArtifactProvenance
BreakArtifactTraceability
RepresentLifecycleStatesAsArtifactTypes
DuplicateNormativeResponsibilitiesAcrossModels
## 13. SCIENTIFIC ARTIFACT LIFECYCLE

PURPOSE

DefineTheLifecycleStateAndTransitionsOfScientificArtifactsIndependentlyOfArtifactTaxonomy.

BOUNDARY

Chapter12ScientificArtifactModelDefinesArtifactIdentityTypeTaxonomyRelationshipsAndIntegrity.

Chapter13ScientificArtifactLifecycleDefinesLifecycleStatePromotionSupersessionAndArchival.

RULE

Lifecycle state MUST_NOT be used as an artifact type or specialization class.

LIFECYCLE

Draft
>
Working
>
EditorialReview
>
ReleaseCandidate
>
FieldValidation
>
Stable
>
Superseded
>
Archived

RULE

RULE_NAME
AssignLifecycleState

MUST
RecordLifecycleTransitions
MaintainLifecycleHistory
DocumentPromotionCriteria
MaintainTraceabilityAcrossLifecycleStates

RULE

Lifecycle State SHOULD describe publication and release maturity only.

RULE

Scientific development maturity SHOULD be represented by the Scientific State Architecture.

SHOULD

PromoteArtifactsOnlyAfterSuccessfulValidation
DocumentLifecycleResponsibilities

MUST_NOT

SkipMandatoryLifecycleStates
PromoteArtifactsWithoutRequiredValidation
DiscardLifecycleHistory

## 14. SPECIFICATION GOVERNANCE

PURPOSE

DefineNormativeGovernanceForScientificSpecifications

RULE

RULE_NAME
MaintainSingleNormativeSpecification

MUST
MaintainVersionHistory
MaintainBackwardTraceability
DocumentArchitecturalRationale
DocumentNormativeChanges
ReviewNormativeChangesBeforeRelease
UseCompletePreviousSpecificationAsEditingBaseline
MaintainEditorialConsistency
MaintainTerminologyConsistency
SeparateNormativeContentFromWorkingNotes
SeparateExperimentalConceptsFromNormativeRequirements
AssignLifecycleStateToSpecifications

SHOULD

MinimizeNormativeComplexity
PreferEvolutionOverReplacement
PromoteBackwardCompatibleChanges
PreserveStableIdentifiers

MUST_NOT

CreateCompetingNormativeSpecifications
ReconstructNormativeSpecificationsFromConversationSummary
RemoveNormativeRulesWithoutDocumentedReason
MixProjectSpecificContentIntoGeneralSpecifications
PromoteExperimentalConceptsWithoutValidation

## 15. CHANGE MANAGEMENT

PURPOSE

Coordinate, document, assess, prioritize, implement, and record scientific changes while preserving traceability.

ARCHITECTURAL_ROLE

Process coordination only.

RULE

Change Management MUST NOT define independent scientific state semantics.

RULE

Scientific state semantics MUST be defined exclusively by the Scientific State Architecture.

RULE

Change Management MUST reference those definitions and MUST NOT redefine them.

PROCESS_SCOPE

Change Management MUST:

- coordinate scientific changes;
- preserve traceability;
- document impacts;
- support implementation;
- reference the Scientific State Architecture for Candidate State;
- reference Governance for Integration Decisions;
- reference Scientific Lifecycle for publication maturity.

Change Management MUST NOT:

- define scientific maturity;
- define governance outcomes;
- redefine lifecycle semantics.

PROCESS_REVIEW

Each process SHOULD:

- reference Candidate State instead of defining scientific maturity;
- reference Integration Decision instead of defining governance outcomes;
- preserve traceability without introducing additional state semantics.

## 16. VERSION POLICY

PURPOSE

DefineNormativeVersioningRulesForScientificSpecifications

VERSIONING

MAJOR

ArchitecturalChange
NormativeRestructuring
BreakingScientificChange

MINOR

BackwardCompatibleEnhancement
WorkflowExtension
NewNormativeCapability

PATCH

EditorialCorrection
Clarification
ConsistencyImprovement

RULE

RULE_NAME
AssignSemanticVersion

MUST
DocumentVersionHistory
DocumentCompatibility
DocumentMigrationPath
DocumentValidationStatus
IncreaseVersionBeforeRelease
MaintainBackwardTraceability

SHOULD

PreferBackwardCompatibleEvolution
GroupRelatedChangesIntoSingleRelease
UseReleaseCandidatesBeforeStableReleases

MUST_NOT

ReuseVersionIdentifiers
ChangeReleasedArtifactsWithoutVersionIncrement
PublishStableWithoutCompletedFieldValidation

## 17. VALIDATION PHILOSOPHY

PURPOSE

DefineScientificValidationPrinciples

PRINCIPLE

TheoryGuidesPractice
PracticeValidatesTheory
PracticeMayRefineTheory
ScientificEvidenceOverridesAssumptions

RULE

RULE_NAME
ValidateNormativeChangesThroughPracticalApplication

MUST
ValidateExperimentalConceptsBeforeNormativeIntegration
SeparateSpecificationErrorsFromImplementationErrors
SeparateImplementationErrorsFromOperationalErrors
DocumentValidationEvidence
DocumentValidationScope
DocumentValidationLimitations
DocumentObservedStrengths
DocumentObservedWeaknesses
DocumentImprovementCandidates
MaintainValidationTraceability

SHOULD

PerformValidationUsingIndependentScientificArtifacts
RepeatValidationAfterMajorNormativeChanges

MUST_NOT

TreatTheoreticalCompletenessAsScientificValidation
PromoteNormativeChangesWithoutValidationEvidence
DiscardNegativeValidationResults

## 18. SYSTEM TRANSPARENCY

PURPOSE

EnsureTransparentHandlingOfSystemCapabilitiesAndConstraints

PRINCIPLE

ScientificIntegrityHasPriorityOverApparentCompleteness

RULE

RULE_NAME
IdentifyRelevantSystemConstraints

MUST
ExplainSystemConstraintsBeforeScientificQualityIsAffected
ExplainScientificConsequencesOfSystemConstraints
DistinguishScientificLimitationsFromSystemLimitations
RecommendScientificallySoundAlternativeWorkflows
RecommendWorkflowAdaptationBeforeReducingScientificQuality
RecommendIntermediateArtifactsWhenAppropriate
RecommendIncrementalExecutionWhenAppropriate
RecommendPersistenceBeforeKnownContextLimitsAreReached
MaintainTransparencyThroughoutScientificExecution
DocumentConstraintDrivenAdaptations

SHOULD

EstimatePotentialImpactOfKnownSystemConstraints
ExplainWhenAlternativeExecutionStrategiesExist
SupportHumanDecisionMakingUnderSystemConstraints

MUST_NOT

ConcealKnownSystemConstraints
ReduceScientificQualityWithoutExplicitWarning
InventScientificResultsToCompensateForSystemConstraints
ContinueKnownInvalidExecutionWithoutWarning
TreatTechnicalConvenienceAsScientificJustification

## 19. SCIENTIFIC INTEGRITY UNDER SYSTEM CONSTRAINTS

PURPOSE

PreserveScientificIntegrityWhenOperatingUnderSystemConstraints

PRINCIPLE

AdaptWorkflow

NeverAdaptEvidence

RULE

RULE_NAME
PreserveEvidenceIntegrity

MUST
PreserveScientificUncertainty
PreserveTraceability
PreserveOriginalObservations
EscalateWorkflowBeforeReducingScientificQuality
PreferScientificCompletenessOverExecutionConvenience
PreferPartialValidatedResultsOverCompleteUnverifiedResults
MaintainExplicitDistinctionBetweenKnownUnknownAndAssumed
DocumentConstraintDrivenScientificLimitations

SHOULD

ProduceValidatedIntermediateArtifacts
RecommendAlternativeExecutionStrategies
RecommendDeferredCompletionWhenScientificallyAppropriate

MUST_NOT

InventEvidence
InventFacts
InventScientificArtifacts
HideScientificUncertainty
TransformAssumptionsIntoFacts
ReduceScientificIntegrityToAvoidSystemConstraints

## 20. REFERENCE IMPLEMENTATION

PURPOSE

DefineRequirementsForScientificReferenceImplementations

RULE

RULE_NAME
ValidateAgainstAtLeastOneDomainModel

MUST
ValidateAgainstAtLeastOneProjectProfile
ValidateAgainstAtLeastOneScientificImplementation
ValidateScientificWorkflow
ValidateScientificArtifacts
ValidateGovernance
ValidateVersionPolicy
ProduceValidationArtifacts
ProduceValidationReport
DocumentValidationScope
DocumentValidationLimitations
MaintainValidationTraceability

SHOULD

ValidateUsingIndependentScientificProjects
RepeatValidationAfterMajorNormativeChanges
ReuseExistingValidationArtifacts

MUST_NOT

TreatSingleImplementationsAsUniversalProof
TreatImplementationSpecificBehaviorAsNormative
PromoteSpecificationsWithoutReferenceValidation

## 21. CONFORMANCE

PURPOSE

DefineNormativeConformanceRequirements

CONFORMANCE_LEVEL

Conformant
ConditionallyConformant
NonConformant

RULE

RULE_NAME
ConformToFoundation

MUST
ConformToScientificWorkflow
ConformToHumanAICollaboration
ConformToDecisionModel
ConformToKnowledgeModel
ConformToScientificArtifactModel
ConformToGovernance
ConformToVersionPolicy
ConformToValidationPhilosophy
MaintainScientificTraceability
MaintainEvidenceIntegrity
MaintainSystemTransparency
DocumentKnownDeviations

SHOULD

DocumentConformanceAssessment
DocumentResidualRisks
DocumentImprovementCandidates

MUST_NOT

ClaimConformanceWithoutEvidence
IgnoreNormativeViolations
ConcealKnownNonConformities

## 22. CONTINUOUS SCIENTIFIC IMPROVEMENT

PURPOSE

DefineTheContinuousEvolutionOfScientificSpecifications

PURPOSE

Continuous Scientific Improvement SHOULD reuse the Scientific State Architecture for scientific development states while defining the continuous improvement process.

FLOW

Specification
>
ScientificImplementation
>
Observation
>
ImprovementCandidate
>
ExperimentalConcept
>
FieldValidation
>
NormativeIntegration
>
Release
>
ScientificImplementation

RULE

RULE_NAME
BaseImprovementsOnScientificEvidence

MUST
MaintainContinuousFeedbackLoop
LinkImprovementsToValidationEvidence
PreserveBackwardTraceability
DocumentImprovementRationale
DocumentExpectedScientificBenefit
ValidateNormativeImprovementsBeforeRelease
ReviewExperimentalConceptsBeforePreparingNewRelease

SHOULD

PreferIncrementalEvolution
ReuseValidatedSolutions
DocumentLessonsLearned

MUST_NOT

IntroduceNormativeChangesWithoutEvidence
RestartSpecificationDevelopmentWithoutReviewingExperimentalConcepts
DiscardValidatedImprovementKnowledge

CANDIDATE_WORKFLOW_BINDING

Observation
>
SpecificationCandidateProfile
>
SpecificationCandidateRegister
>
Review
>
ReviewResolutionPlan
>
Validation
>
PromotionDecision
>
NormativeIntegration
>
Release

RULE

Continuous improvement MUST use the controlled specification evolution architecture for every normative change.

RULE

Improvement knowledge MUST be persisted in candidate records and MUST_NOT depend exclusively on conversation history or temporary working notes.

# PART II – SPECIFICATION EVOLUTION

## 23. VERSION HISTORY

PURPOSE

ProvideTraceableEvolutionOfTheSpecification

RULE

RULE_NAME
DocumentEveryReleasedVersion

MUST
DocumentVersionStatus
DocumentSupersededVersions
MaintainVersionTraceability
PreserveHistoricalEntries

MUST_NOT

ModifyHistoricalReleaseEntries

VERSION

1.3

STATUS

Stable

DESCRIPTION

Foundation for General Scientific Layer.

VERSION

2.0 RC1

STATUS

ReleaseCandidate

DESCRIPTION

Editorial integration toward GSL 2.0 RC1.

NEXT_STAGE

ReleaseCandidate

## 24. EXPERIMENTAL CONCEPTS

PURPOSE

ProvideControlledStagingForFutureNormativeEvolution

RULE

RULE_NAME
RegisterEveryCandidateNormativeExtension

MUST
AssignUniqueConceptIdentifier
AssignConceptStatus
AssignValidationStatus
DocumentScientificMotivation
DocumentExpectedBenefit
DocumentValidationEvidence
DocumentIntegrationDecision
MaintainConceptHistory
ReviewAllExperimentalConceptsBeforePreparingANewRelease
ReviewAllValidatedConceptsBeforePreparingANewRelease
ReviewAllIntegrationPendingConceptsBeforePreparingANewRelease

MUST_NOT

IntroduceNormativeRequirementsDirectly
DiscardExperimentalConceptsWithoutDecision
ModifyNormativeChaptersBeforeSuccessfulValidation

STATUS

Experimental
Validated
IntegrationPending
Integrated
Rejected
Deferred

------------------------------------------------------------------------------

SECTION

ScientificWorkingContextModel

STATUS

ArchitectureDraft

PURPOSE

DefineHowGeneralDomainAndProjectContextsSpecializeScientificWorkingBehavior.

CONTEXT_LAYERS

GeneralScientificWorkingContext
DomainScientificWorkingContext
ProjectScientificWorkingContext

INHERITANCE_FLOW

GeneralScientificWorkingContext
>
DomainScientificWorkingContext
>
ProjectScientificWorkingContext

DERIVED_PROFILES

HumanRoleProfile
AIRoleProfile

RULE

The General Scientific Layer MUST define only universally applicable Scientific Working Context requirements.

RULE

A domain model SHOULD define one default Domain Scientific Working Context for its primary use case.

RULE

A Project Scientific Specification SHOULD activate the applicable domain context and document project-specific adaptations.

RULE

Derived Human and AI Role Profiles MUST preserve inherited scientific objectives, terminology, evidence requirements and integrity rules.

RULE

When task-specific behavior is required, project-level role refinements SHOULD add that behavior and MUST_NOT weaken inherited scientific requirements.

RULE

Role profiles define task-oriented working modes and MUST_NOT be interpreted as permission profiles.

RULE

When both domain expertise and model-development expertise are required by the active task, the AI Role Profile MUST combine them.

RULE

The active Scientific Working Context MUST remain explicit enough to prevent unintended drift into unrelated default behavior.

------------------------------------------------------------------------------

SECTION

ProjectModelAdaptation

STATUS

ArchitectureDraft

PURPOSE

DefineHowProjectScientificSpecificationsAdaptDomainModelsWithoutModifyingTheGeneralScientificLayer.

ADAPTATION_CHAIN

GeneralScientificLayer
>
DomainModel
>
ProjectScientificSpecification

RULE

The General Scientific Layer MUST define only universally applicable scientific responsibilities.

RULE

A Domain Model SHOULD specialize the General Scientific Layer for one scientific discipline or recurring use case.

RULE

A Project Scientific Specification SHOULD activate one applicable domain model and document every intentional project-specific adaptation.

RULE

Project adaptations MUST preserve traceability to inherited General Scientific Layer and Domain Model responsibilities.

RULE

When required by the scientific objective, projects MUST specialize the applicable structures, workflows, artifact types or validation rules.

RULE

Project adaptations MUST_NOT weaken inherited integrity, traceability or provenance requirements.

RULE

When no suitable domain model exists, a project MUST specialize the General Scientific Layer directly and preserve the adaptation chain.

------------------------------------------------------------------------------

SECTION

SpecificationCandidateRegister

STATUS

ArchitectureDraft

PURPOSE

DefineTheAuthoritativeContainerManagingSpecificationCandidateProfiles.

MODEL_TYPE

AuthoritativeRegister

CONFORMS_TO

AuthoritativeWorkingElement

CONTAINS

SpecificationCandidateProfile

REQUIRED_FIELDS

RegisterIdentifier

RegisterStatus

CandidateProfiles

RULE

Every Specification Candidate Register MUST conform to the AuthoritativeWorkingElement model.

RULE

Every Specification Candidate Profile MUST appear at most once within one Specification Candidate Register.

RULE

RegisterStatus describes the authoritative state of the register itself and MUST remain independent of the status of contained Specification Candidate Profiles.

RULE

CandidateStatus describes the maturity and decision state of an individual Specification Candidate Profile and MUST_NOT be inferred from RegisterStatus.

RULE

Candidate ordering MUST_NOT imply architectural priority unless an explicit Priority attribute is recorded.

RULE

Closed candidates MUST remain referenceable through the register or an associated archival reference.

RULE

Candidate removal MUST preserve historical traceability and SHOULD normally be implemented as non-destructive closure or archival reference rather than physical deletion.

RULE

Promotion MUST preserve a reference to the originating Specification Candidate Profile.

RULE

The register MUST distinguish at least the states Open, Deferred, Accepted, Rejected and Promoted.

------------------------------------------------------------------------------

SECTION

SpecificationCandidateRegister

STATUS

ArchitectureDraft

PURPOSE

DefineTheAuthoritativeContainerManagingSpecificationCandidateProfiles.

MODEL_TYPE

AuthoritativeRegister

CONFORMS_TO

AuthoritativeWorkingElement

CONTAINS

SpecificationCandidateProfile

REQUIRED_FIELDS

RegisterIdentifier

RegisterStatus

CandidateProfiles

RULE

Every Specification Candidate Register MUST conform to the AuthoritativeWorkingElement model.

RULE

Every Specification Candidate Profile MUST appear at most once within one Specification Candidate Register.

RULE

RegisterStatus describes the authoritative state of the register itself and MUST remain independent of the status of contained Specification Candidate Profiles.

RULE

CandidateStatus describes the maturity and decision state of an individual Specification Candidate Profile and MUST_NOT be inferred from RegisterStatus.

RULE

Candidate ordering MUST_NOT imply architectural priority unless an explicit Priority attribute is recorded.

RULE

Closed candidates MUST remain referenceable through the register or an associated archival reference.

RULE

Candidate removal MUST preserve historical traceability and SHOULD normally be implemented as non-destructive closure or archival reference rather than physical deletion.

RULE

Promotion MUST preserve a reference to the originating Specification Candidate Profile.

RULE

The register MUST distinguish at least the states Open, Deferred, Accepted, Rejected and Promoted.

------------------------------------------------------------------------------
SUBSECTION

ActiveCandidateManagement

PURPOSE

ManageActiveSpecificationCandidateProfilesAndTheirCurrentWorkingState.

RULE

The Specification Candidate Register MUST manage active Specification Candidate Profiles.

RULE

The active register MUST distinguish active candidate records from archival references.

RULE

Archived Specification Candidate Profiles MUST remain referenceable through the active register.

RULE

A Specification Candidate Profile MUST_NOT be removed or reduced before successful archival transfer has been persisted and verified.

RULE

A reduced archival reference MUST preserve Candidate Identifier, final decision, target release and archive reference.

SUBSECTION

CandidateLifecycleBinding

PURPOSE

BindRegisterOperationsToTheSpecificationCandidateLifecycle.

CANDIDATE_LIFECYCLE

Idea
>
Registered
>
Expanded
>
Reviewed
>
Validated
>
Decision
>
Archived

TERMINAL_DECISIONS

Promoted
Deferred
Rejected
Superseded
Withdrawn

RULE

Every Specification Candidate Profile MUST possess a current lifecycle state.

RULE

Lifecycle state MUST remain distinguishable from Candidate Decision State and Register Status.

RULE

A candidate MUST_NOT be transferred to the Specification Candidate Archive unless a terminal decision is documented.

RULE

Promoted candidates MUST reference the integrating specification release.

RULE

Superseded candidates MUST reference their successor.

RULE

Deferred candidates MUST remain active or be archived according to the documented deferral policy.

SUBSECTION

ArchiveReferenceModel

PURPOSE

PreserveTraceabilityFromTheActiveRegisterToReleaseBoundCandidateArchives.

REQUIRED_ARCHIVE_REFERENCE_FIELDS

CandidateIdentifier
FinalDecision
TargetRelease
ArchiveIdentifier
ArchiveLocation

RULE

Every archived candidate MUST remain reachable from the active register through a stable archive reference.

RULE

Archive references MUST_NOT replace the complete archived candidate history.

SECTION

SpecificationCandidateArchive

STATUS

ArchitectureDraft

PURPOSE

ProvideReleaseBoundLongTermPreservationOfCompletedSpecificationCandidateProfiles.

MODEL_TYPE

ScientificArchive

CONFORMS_TO

ScientificArtifact

CONDITIONAL_CONFORMANCE

AuthoritativeWorkingElement

CONDITION

ControlledIterativeArchiveDevelopmentRequired

REQUIRED_FIELDS

ArchiveIdentifier
TargetRelease
ArchiveStatus
ArchivedCandidateProfiles
SourceRegisterReferences

RULE

Every Specification Candidate Archive MUST identify exactly one target specification release or explicitly bounded release family.

RULE

The archive MUST preserve the complete origin, proposal, evidence, impact, review, decision, promotion and closure history of each archived candidate.

RULE

Archived candidate identity MUST remain unchanged.

RULE

Archived candidates MUST remain permanently referenceable.

RULE

The archive MUST preserve traceability to the source Specification Candidate Register generation from which each candidate was transferred.

RULE

The archive MUST_NOT silently alter archived candidate content after transfer.

SUBSECTION

ReleaseBoundArchive

PURPOSE

UseTheArchiveAsTheScientificChangeAndDecisionRecordForASpecificRelease.

RULE

Each release SHOULD possess one corresponding Specification Candidate Archive when candidate-based evolution is used.

RULE

The release archive SHOULD provide the authoritative candidate basis for release notes, migration documentation and later review.

RULE

Candidates integrated, rejected, superseded or otherwise closed for the release MUST be represented in the release archive or by a traceable external archival reference.

SUBSECTION

ArchivalTransfer

PURPOSE

ApplyControlledArtifactTransferFromTheActiveRegisterToTheReleaseBoundArchive.

FLOW

SelectCompletedCandidate
>
PersistCandidateInArchiveSuccessor
>
VerifyCompleteCandidateHistory
>
VerifyArchiveReferences
>
TransferArchivalAuthority
>
ReplaceActiveCandidateBlockWithArchiveReference

RULE

Archival transfer MUST conform to ControlledArtifactTransfer.

RULE

The complete candidate MUST be persisted and verified in the archive before its active register representation is reduced.

RULE

A failed archival transfer MUST leave the last verified active register and archive states unchanged.

RULE

Archival transfer MUST preserve Candidate Identifier, final decision, target release and integration references.

RULE

Removal of the full active candidate block and creation of the archive reference SHOULD be performed as separate verifiable transformations when information loss would be material.

------------------------------------------------------------------------------

SECTION

Quality

CHAPTER_BINDING

GeneralScientificLayerChapter11

SUBSECTION

PersistentRepresentation

PURPOSE

DefineMinimumQualityRequirementsForPersistentScientificArtifactsAndWorkingElements.

RULE

Every persisted textual Scientific Artifact and Authoritative Working Element MUST use UTF-8 character encoding.

RULE

Persistent representations MUST preserve all scientific content without information loss caused by character encoding.

RULE

Persistent textual representations SHOULD use interoperable, openly documented encodings unless a project-specific exception is explicitly justified.

------------------------------------------------------------------------------

SECTION

SpecificationCandidateRegister

STATUS

ArchitectureDraft

PURPOSE

DefineTheAuthoritativeContainerManagingSpecificationCandidateProfiles.

MODEL_TYPE

AuthoritativeRegister

CONFORMS_TO

AuthoritativeWorkingElement

CONTAINS

SpecificationCandidateProfile

REQUIRED_FIELDS

RegisterIdentifier

RegisterStatus

CandidateProfiles

RULE

Every Specification Candidate Register MUST conform to the AuthoritativeWorkingElement model.

RULE

Every Specification Candidate Profile MUST appear at most once within one Specification Candidate Register.

RULE

RegisterStatus describes the authoritative state of the register itself and MUST remain independent of the status of contained Specification Candidate Profiles.

RULE

CandidateStatus describes the maturity and decision state of an individual Specification Candidate Profile and MUST_NOT be inferred from RegisterStatus.

RULE

Candidate ordering MUST_NOT imply architectural priority unless an explicit Priority attribute is recorded.

RULE

Closed candidates MUST remain referenceable through the register or an associated archival reference.

RULE

Candidate removal MUST preserve historical traceability and SHOULD normally be implemented as non-destructive closure or archival reference rather than physical deletion.

RULE

Promotion MUST preserve a reference to the originating Specification Candidate Profile.

RULE

The register MUST distinguish at least the states Open, Deferred, Accepted, Rejected and Promoted.

------------------------------------------------------------------------------

SECTION

SpecificationCandidateRegister

STATUS

ArchitectureDraft

PURPOSE

DefineTheAuthoritativeContainerManagingSpecificationCandidateProfiles.

MODEL_TYPE

AuthoritativeRegister

CONFORMS_TO

AuthoritativeWorkingElement

CONTAINS

SpecificationCandidateProfile

REQUIRED_FIELDS

RegisterIdentifier

RegisterStatus

CandidateProfiles

RULE

Every Specification Candidate Register MUST conform to the AuthoritativeWorkingElement model.

RULE

Every Specification Candidate Profile MUST appear at most once within one Specification Candidate Register.

RULE

RegisterStatus describes the authoritative state of the register itself and MUST remain independent of the status of contained Specification Candidate Profiles.

RULE

CandidateStatus describes the maturity and decision state of an individual Specification Candidate Profile and MUST_NOT be inferred from RegisterStatus.

RULE

Candidate ordering MUST_NOT imply architectural priority unless an explicit Priority attribute is recorded.

RULE

Closed candidates MUST remain referenceable through the register or an associated archival reference.

RULE

Candidate removal MUST preserve historical traceability and SHOULD normally be implemented as non-destructive closure or archival reference rather than physical deletion.

RULE

Promotion MUST preserve a reference to the originating Specification Candidate Profile.

RULE

The register MUST distinguish at least the states Open, Deferred, Accepted, Rejected and Promoted.

------------------------------------------------------------------------------

SUBSECTION

ArchiveReferenceModel

PURPOSE

PreserveTraceabilityFromTheActiveRegisterToReleaseBoundCandidateArchives.

REQUIRED_ARCHIVE_REFERENCE_FIELDS

CandidateIdentifier
FinalDecision
TargetRelease
ArchiveIdentifier
ArchiveLocation

RULE

Every archived candidate MUST remain reachable from the active register through a stable archive reference.

RULE

Archive references MUST_NOT replace the complete archived candidate history.

PART X — Authoritative Working Element (AWE)

10.1 Purpose

Defines the Authoritative Working Element (AWE) as the normative model governing the controlled evolution of scientific specifications.

10.2 Core Concepts

10.2.1 Authoritative Working Element (AWE)

DEFINITION

The Authoritative Working Element is the normative scientific framework that governs the controlled evolution of a scientific specification.

10.2.2 AWE Lineage

DEFINITION

An AWE Lineage is the ordered sequence of authoritative Authoritative Working States belonging to one Authoritative Working Element. At any time exactly one Authoritative Working Draft is active within a lineage.

10.2.3 Authoritative Working Draft (AWD)

This part normatively defines the Authoritative Working Element model.

10.1 Core Concepts

AWE_CORE_CONCEPT

TERM

Authoritative Working Draft (AWD)

DEFINITION

The Authoritative Working Draft is the single authoritative scientific working specification within an active AWE Lineage. It serves as the continuously maintained integration point for accepted scientific changes and represents the sole normative basis for ongoing scientific development, evaluation, review, and controlled evolution.

NOTE

The Authoritative Working Draft is an AWE core concept. Its normative behaviour is specified by the AWE behavioural rules (MaintainSingleAuthoritativeWorkingDraft, IntegrateAcceptedScientificChanges, EvaluateIntegratedWorkingDraft, ReplaceAuthoritativeWorkingState, PreventParallelAuthoritativeWorkingDrafts).

AWE_WORKING_CYCLE

PURPOSE

Defines the normative scientific workflow governing the evolution of an Authoritative Working Draft.

WORKING_CYCLE

1. Receive Scientific Change
   A scientific change proposal is submitted.

2. Scientific Evaluation
   The proposed change is evaluated using the applicable scientific process.

3. Integration Decision
   The change is accepted or rejected.

4. Integrate Accepted Change
   Accepted changes are integrated into the Authoritative Working Draft.

5. Regenerate Authoritative Working Draft
   Integration results in a regenerated Authoritative Working Draft.

6. Replace Previous Authority
   The regenerated Authoritative Working Draft becomes the sole authoritative Authoritative Working State.

7. Continue Scientific Development
   All subsequent scientific work MUST continue from the regenerated Authoritative Working Draft.

ARCHITECTURAL_RESULT

The AWE Working Cycle establishes a continuous, traceable, and authoritative evolution process that prevents fragmentation of scientific Authoritative Working States.

AUTHORITATIVE_WORKING_PRACTICE

RULE

RULE_NAME
MaintainSingleAuthoritativeWorkingDraft

MUST

Exactly one Authoritative Working Draft MUST exist within an active AWE Lineage.

RULE

RULE_NAME
IntegrateAcceptedScientificChanges

MUST

Accepted scientific changes MUST be integrated into the Authoritative Working Draft before further scientific development continues.

RULE

RULE_NAME
EvaluateIntegratedWorkingDraft

MUST

Scientific evaluation MUST be performed against the integrated Authoritative Working Draft rather than isolated change descriptions.

RULE

RULE_NAME
ReplaceAuthoritativeWorkingState

MUST

After successful integration and persistence, the regenerated Authoritative Working Draft MUST become the new authoritative Authoritative Working State.

RULE

RULE_NAME
PreventParallelAuthoritativeWorkingDrafts

MUST_NOT

Multiple parallel Authoritative Working Drafts MUST_NOT exist within the same active AWE Lineage.

10.5 Architectural Relationships

- An Authoritative Working Element owns one active AWE Lineage.
- An AWE Lineage contains exactly one active Authoritative Working Draft.
- The AWE Working Cycle evolves one Authoritative Working Draft into the next.
- AWE Behaviour constrains execution of the AWE Working Cycle.
- Successful completion of the Working Cycle transfers authority to the regenerated Authoritative Working Draft.

Normative Language Policy

Unless explicitly stated otherwise, normative requirements in this specification MUST be expressed exclusively using the following keywords:

- MUST
- MUST NOT
- SHOULD
- MAY

Terminology Policy

The following terms are normative and MUST be used consistently throughout this specification.

| Preferred Term | Meaning |
|---|---|
| Authoritative Working Element (AWE) | Normative scientific framework |
| AWE Lineage | Ordered sequence of authoritative working states |
| Authoritative Working Draft (AWD) | The single active authoritative draft |
| Authoritative Working State | The authoritative state represented by the active AWD |
| AWE Working Cycle | Controlled evolution process |
| AWE Behaviour | Normative behavioural rules |


---
Document Status: RC3 Candidate (Clean Edition)
Purpose: Normative specification for analytical field testing.
This edition intentionally excludes review protocols, checklists, and temporary editorial artifacts.
---


------------------------------------------------------------------------------

BASELINE_PROVENANCE

This baseline represents the validated result of the GSL v2.0 RC3 field trial.

Baseline Certification
PASS

Future scientific development shall proceed through new Scientific Change
Register (SCR) entries, Authoritative Working Element (AWE) working drafts,
and subsequent Release Candidate cycles.

This baseline remains frozen as the certified scientific reference.
