# General Scientific Layer (GSL) v2.0

DOCUMENT_IDENTIFIER: GSL
STATUS: Stable
VERSION: 2.0
SUPERSEDES: GSL v2.0 RC3
DOCUMENT_TYPE: NormativeSpecification

AUTHOR: JonasM49
PUBLISHED_AT: 2026-09-19
CANONICAL_REPOSITORY: https://github.com/JonasM49/scientific-Framework
LICENSE: CC BY-NC-SA 4.0

VALIDATION_STATUS: RC3BaselineValidated; ReleaseConsolidationPassed

PURPOSE:
- ProfessionalizeScientificResearch
- DeterministicHumanAICollaboration
- EvidenceBased
- Reproducible
- Traceable

## 1. SCOPE

The General Scientific Layer (GSL) defines universal principles for
human–AI supported scientific work.

The GSL specifies scientific behavior, governance, validation,
traceability and specification evolution.

The GSL does not define domain-specific methods,
project-specific workflows or implementation-specific technologies.

These aspects MUST be defined by domain models,
project profiles or reference implementations.

## 2. FOUNDATION

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

## 3. SCIENTIFIC WORKFLOW

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

## 4. HUMAN–AI COLLABORATION

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

### 5.1 SCIENTIFIC WORKING CONTEXT SPECIALIZATION

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

## 5. PARAMETER RESOLUTION

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

## 6. DECISION CLASSES

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

## 7. DECISION PERSISTENCE

RULE

RULE_NAME
PersistConfirmedProjectDecisions

MUST
MaintainDecisionHistory
ReusePersistedDecisions
WarnOnConflicts
RequireExplicitOverrideForChanges

## 8. INTERACTION

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

## 9. KNOWLEDGE MODEL

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

## 10. QUALITY

RULE

RULE_NAME
CheckConsistency

MUST
DocumentConflicts
RecordUncertainty
EveryFactRequiresEvidence
EveryHypothesisRequiresReason

### 11.1 PERSISTENT REPRESENTATION

PURPOSE

DefineMinimumQualityRequirementsForPersistentScientificArtifactsAndWorkingElements.

RULE

Every persisted textual Scientific Artifact and Authoritative Working Element MUST use a standardized character encoding capable of lossless representation of the scientific content.

RULE

Persistent representations MUST preserve all scientific content without information loss caused by character encoding.

RULE

Persistent textual representations SHOULD use interoperable, openly documented encoding standards.

NOTE

UTF-8 and UTF-16 are examples of standardized encodings. This specification does not prescribe one specific encoding standard.

## 11. SCIENTIFIC ARTIFACT MODEL

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

### 12.9 PROJECT MODEL ADAPTATION

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

## 12. SCIENTIFIC ARTIFACT LIFECYCLE

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

Scientific development maturity SHOULD be represented by the applicable specialized scientific development state model and MUST remain distinguishable from Lifecycle State.

SHOULD

PromoteArtifactsOnlyAfterSuccessfulValidation
DocumentLifecycleResponsibilities

MUST_NOT

SkipMandatoryLifecycleStates
PromoteArtifactsWithoutRequiredValidation
DiscardLifecycleHistory

## 13. AUTHORITATIVE WORKING ELEMENT (AWE)

PURPOSE

DefineTheControlledAuthoritativeEvolutionOfScientificArtifactsDuringActiveWorkingLineages.

### 14.1 AUTHORITATIVE WORKING ELEMENT

DEFINITION

The Authoritative Working Element is the normative scientific framework that governs the controlled authoritative evolution of a Scientific Artifact during an active working lineage.

### 14.2 AWE LINEAGE

DEFINITION

An AWE Lineage is the ordered sequence of authoritative Authoritative Working States belonging to one Authoritative Working Element.

RULE

At any time exactly one Authoritative Working Draft MUST be active within one active AWE Lineage.

### 14.3 AUTHORITATIVE WORKING DRAFT

DEFINITION

The Authoritative Working Draft is the single authoritative scientific working artifact within an active AWE Lineage. It serves as the continuously maintained integration point for accepted scientific changes and represents the sole authoritative basis for ongoing scientific development, evaluation, review, and controlled evolution within that lineage.

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

### 14.4 AWE WORKING CYCLE

WORKING_CYCLE

ReceiveScientificChange
>
ScientificEvaluation
>
IntegrationDecision
>
IntegrateAcceptedChange
>
RegenerateAuthoritativeWorkingDraft
>
ReplacePreviousAuthority
>
ContinueScientificDevelopment

RULE

All subsequent scientific work within an active AWE Lineage MUST continue from the current Authoritative Working Draft.

### 14.5 AWD CLOSURE AND CLEAN BASELINE DERIVATION

PURPOSE

DistinguishAuthoritativeWorkingEvolutionFromCleanBaselineRepresentation.

RULE

Developmental content belonging to an Authoritative Working Draft MUST remain preserved within its authoritative working lineage unless its disposition and preservation are governed by another persistent Scientific Artifact.

RULE

When an Authoritative Working Draft has completed the applicable review and validation process, its active AWE Lineage MAY be closed or frozen.

RULE

A Clean Baseline MAY be derived from a closed or frozen Authoritative Working Draft through a controlled transformation.

RULE

A Clean Baseline MUST preserve the complete applicable normative scientific content and MUST preserve traceability to the closed or frozen Authoritative Working Draft from which it was derived.

RULE

Developmental working content MAY be omitted from a Clean Baseline when that content is not part of the resulting normative state and its scientifically relevant change knowledge remains preserved and traceable.

RULE

A Clean Baseline is not an Authoritative Working Draft.

RULE

When controlled development of a Clean Baseline begins again, a new AWE Lineage MUST be established from the applicable baseline or other explicitly identified authoritative predecessor.

RULE

Artifact Version, AWE Generation, AWE Lineage and Clean Baseline representation MUST remain distinguishable.

### 14.6 ARCHITECTURAL RELATIONSHIPS

- An Authoritative Working Element owns one active AWE Lineage during controlled development.
- An active AWE Lineage contains exactly one active Authoritative Working Draft.
- The AWE Working Cycle evolves one Authoritative Working Draft into the next.
- Successful completion of the Working Cycle transfers authority to the regenerated Authoritative Working Draft.
- Closure or freeze ends active working evolution in that lineage.
- Clean Baseline derivation produces a non-AWD representation of the resulting authoritative scientific state.

### 14.7 NORMATIVE LANGUAGE AND TERMINOLOGY

Unless explicitly stated otherwise, normative requirements in this specification MUST be expressed exclusively using MUST, MUST NOT, SHOULD or MAY.

RULE

Normative terms MUST be used consistently throughout this specification.

| Preferred Term | Meaning |
|---|---|
| Authoritative Working Element (AWE) | Normative framework for controlled authoritative evolution |
| AWE Lineage | Ordered sequence of authoritative working states |
| Authoritative Working Draft (AWD) | Single active authoritative working artifact |
| Authoritative Working State | Authoritative state represented by the active AWD |
| AWE Working Cycle | Controlled evolution process |
| Clean Baseline | Controlled non-AWD representation derived from a closed or frozen authoritative working state |

## 14. SPECIFICATION GOVERNANCE

PURPOSE

DefineNormativeGovernanceForScientificSpecifications

RULE

RULE_NAME
MaintainSingleNormativeSpecification

MUST
PreserveVersionHistory
MaintainBackwardTraceability
DocumentArchitecturalRationale
DocumentNormativeChanges
ReviewNormativeChangesBeforeRelease
UseCompletePreviousSpecificationAsEditingBaseline
MaintainEditorialConsistency
MaintainTerminologyConsistency
SeparateNormativeContentFromWorkingNotes
SeparateDevelopmentalCandidateContentFromNormativeRequirements
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

Scientific state semantics MUST be defined by their applicable normative owner and MUST remain distinguishable from Change Management process coordination.

RULE

Change Management MUST reference applicable state definitions and MUST NOT redefine them.

PROCESS_SCOPE

Change Management MUST:

- coordinate scientific changes;
- preserve traceability;
- document impacts;
- support implementation;
- reference the applicable Specification Evolution model for Candidate State;
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
PreserveVersionHistory
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

DefineTheContinuousEvolutionOfScientificSpecifications.

Continuous Scientific Improvement SHOULD reuse the applicable Specification Evolution state model for scientific development states while defining the continuous improvement process.

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

SPECIFICATION_EVOLUTION_BINDING

Continuous Scientific Improvement MUST use the Specification Evolution architecture defined in Chapter 23.

RULE

Continuous improvement MUST use the controlled specification evolution architecture for every normative change.

RULE

Improvement knowledge MUST be persisted in candidate records and MUST_NOT depend exclusively on conversation history or temporary working notes.

## 23. SPECIFICATION EVOLUTION

PURPOSE

DefineControlledPersistentEvolutionOfNormativeSpecificationCandidates.

EVOLUTION_FLOW

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
ControlledClosure

### 24.1 SPECIFICATION CANDIDATE PROFILE

RULE

Every candidate normative extension MUST possess a unique Candidate Identifier.

REQUIRED_INFORMATION

CandidateIdentifier
CandidateState
ValidationStatus
ScientificMotivation
ExpectedBenefit
ValidationEvidence
IntegrationDecision
CandidateHistory

RULE

Candidate records MUST preserve the scientific motivation, evidence, review, decision and integration traceability required to understand the change.

RULE

Normative requirements MUST_NOT be introduced directly from an unreviewed candidate.

RULE

Candidate knowledge MUST_NOT be discarded without a documented disposition.

### 24.2 SPECIFICATION CANDIDATE REGISTER

MODEL_TYPE

ScientificArtifact

REGISTER_ROLE

AuthoritativeRegister

CONTAINS

SpecificationCandidateProfile

REQUIRED_FIELDS

RegisterIdentifier
RegisterStatus
CandidateProfiles

RULE

A Specification Candidate Register under active controlled development MUST conform to the Authoritative Working Element model.

RULE

Every Specification Candidate Profile MUST appear at most once within one Specification Candidate Register.

RULE

RegisterStatus describes the authoritative state of the register itself and MUST remain independent of the state or decision of contained Specification Candidate Profiles.

RULE

Candidate ordering MUST_NOT imply architectural priority unless an explicit Priority attribute is recorded.

RULE

Promotion MUST preserve a reference to the originating Specification Candidate Profile.

### 24.3 CANDIDATE STATE AND DECISION

CANDIDATE_DEVELOPMENT_STATES

Idea
Registered
Expanded
Reviewed
Validated
Decision
Closed

CANDIDATE_DECISIONS

Accepted
Promoted
Deferred
Rejected
Superseded
Withdrawn

RULE

Candidate Development State, Candidate Decision, Register Status and Scientific Artifact Lifecycle State MUST remain distinguishable.

RULE

Promoted candidates MUST reference the integrating specification release or baseline.

RULE

Superseded candidates MUST reference their successor.

RULE

Deferred candidates MUST remain persistently referenceable according to the documented deferral policy.

### 24.4 CONTROLLED CLOSURE AND ARCHIVAL

RULE

Completed candidate knowledge MUST remain persistently referenceable after closure.

RULE

Archived candidate knowledge MUST remain reachable through a stable traceable reference from its originating register lineage or its authoritative successor.

RULE

A closed Specification Candidate Profile or Specification Candidate Register MAY enter the Archived Scientific Artifact Lifecycle State.

RULE

Archival MUST preserve Candidate Identifier and Candidate Identity, final decision, applicable target release or baseline, evidence, review history, integration references and the complete relevant Candidate History from origin through controlled closure.

RULE

Candidate knowledge MUST_NOT be destructively removed before its persistent preservation and traceability have been verified.

RULE

Archival MUST_NOT require creation of a distinct Specification Candidate Archive artifact when the existing Scientific Artifact and its preserved history provide complete traceability.

RULE

Released or archived historical candidate states MUST_NOT be modified in place.

### 24.5 RELATIONSHIP TO AWE AND CLEAN BASELINES

RULE

Development of an individual Specification Candidate Profile outside an actively developed Specification Candidate Register MAY use an AWE Lineage and Authoritative Working Draft.

RULE

An actively developed Specification Candidate Register MUST conform to the Authoritative Working Element model as defined in Section 23.2.

RULE

After candidate knowledge has been integrated into the applicable specification and the candidate artifact has been controlledly closed, the candidate artifact MAY be frozen or archived.

RULE

A Clean Baseline MUST_NOT embed completed developmental candidate content unless that content is itself part of the normative specification.

RULE

The omission of developmental candidate content from a Clean Baseline MUST_NOT remove or weaken the persistent change knowledge and traceability preserved by the candidate artifacts and their AWE lineage.

