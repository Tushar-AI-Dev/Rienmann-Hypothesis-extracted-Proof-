# Riemann Hypothesis Lean Project (Extracted Archive)

This repository contains the extracted Lean source tree from the 14-part archive hosted at [alpo.ge](https://alpo.ge/lean.tar.gz.part01). The source is organized as a Lean project and includes the project configuration files and its `.lean` modules.

## Where the Riemann Hypothesis claim appears

- [`src/Main.lean`](src/Main.lean) declares `riemannHypothesis` and assigns it `rhOfAll`.
- [`src/Supplements/Kernels/MainTheorems.lean`](src/Supplements/Kernels/MainTheorems.lean) defines `rhOfAll` through `Formalism.VW.rh_of_every allChi`.
- [`src/Statements.lean`](src/Statements.lean) contains the formal statement `RiemannHypothesis`.

The formalization is distributed across many imported files; these entry points are a map into that source, not a standalone proof document. This repository records the archive's claim and does not certify that the claim is correct or that the project builds.

## Complete source folder tree

The 14 numbered archive parts were download chunks that combine into one project; they are not 14 separate proof chapters. The Lean modules are organized into the following source areas. The tree below lists every directory under `src/` (3,614 folders).

<details>
<summary>Expand the complete nested folder tree</summary>

```text
src/
├── BuildAid/
├── CompanionTheory/
│   ├── AutomorphicTheory/
│   │   ├── BesselOrbitBounds/
│   │   │   └── BesselMapUniqueness/
│   │   ├── BesselSmoothness/
│   │   ├── BesselWaveGrids/
│   │   │   └── InterlacingGrids/
│   │   ├── CompactTopologicalForms/
│   │   ├── DiscreteGroupWaves/
│   │   ├── HarishChandraMultiplicity/
│   │   ├── HeckeStandardModules/
│   │   ├── JacobiDiagonalBounds/
│   │   ├── KFiniteVectors/
│   │   ├── KrullDimension/
│   │   ├── LocalBesselUniqueness/
│   │   │   └── BesselModels/
│   │   ├── MirabolicRestriction/
│   │   │   └── MirabolicInduction/
│   │   ├── NumberFieldModels/
│   │   ├── PadicCyclotomicFields/
│   │   ├── PadicUnitaryWeights/
│   │   │   ├── CrystallineUnitParts/
│   │   │   ├── DixmierMalliavin/
│   │   │   └── UnitarySiegelSets/
│   │   ├── PieriRules/
│   │   │   ├── PieriDegreeBounds/
│   │   │   └── ThetaBesselIsometries/
│   │   ├── PlaceSeparation/
│   │   ├── ProductFormulaTheory/
│   │   │   ├── AbelianDeRham/
│   │   │   │   └── FreeAbelianDeRham/
│   │   │   ├── CuspidalExhaustion/
│   │   │   ├── DualAbelianSchemes/
│   │   │   ├── GrothendieckRingPolynomial/
│   │   │   └── SquareIntegrableSegments/
│   │   │       └── SegmentReordering/
│   │   ├── RankOneEstimates/
│   │   ├── RankOneTori/
│   │   ├── SchurLimitBounds/
│   │   │   ├── SchurOrthogonality/
│   │   │   └── ZuckermanDuality/
│   │   ├── SegmentRepresentations/
│   │   │   ├── IrreducibleSegments/
│   │   │   ├── JacquetShalikaBounds/
│   │   │   └── RapidDecayFamilies/
│   │   ├── SiegelUnitTheory/
│   │   ├── SiegelWeilFiniteness/
│   │   ├── TemperedLocalSpectra/
│   │   │   ├── AffineGL/
│   │   │   ├── BernsteinZelevinsky/
│   │   │   ├── CubicForms/
│   │   │   ├── DiscreteSeriesSU/
│   │   │   ├── LocalGeometry/
│   │   │   ├── ObstructionLifting/
│   │   │   ├── ZelevinskyClassification/
│   │   │   │   ├── ZelevinskyCosets/
│   │   │   │   └── ZelevinskySegments/
│   │   │   └── ZetaIntegralsL2/
│   │   ├── ThetaDilations/
│   │   ├── UniformLocalFormulas/
│   │   │   └── UniformLocalSums/
│   │   ├── UnitriangularMeasure/
│   │   │   └── AdeleCoordinateMeasure/
│   │   └── ZuckermanCommutation/
│   │       ├── CapelliEigenvalues/
│   │       └── ZuckermanFunctors/
│   ├── EightfoldTheory/
│   │   ├── VariationTheory/
│   │   │   ├── AutomorphicForms/
│   │   │   │   └── RealStructures/
│   │   │   ├── PublishedTheorems/
│   │   │   ├── SelfDualForms/
│   │   │   │   └── SelfDualWeylChambers/
│   │   │   └── TwistedTheory/
│   │   └── ZeroLevelTheory/
│   │       └── LocalLanglands/
│   ├── HarishChandraModules/
│   │   ├── BesselParameterIntegrals/
│   │   │   ├── BesselOrbitConvolutions/
│   │   │   ├── ParametricIntegralSmoothness/
│   │   │   ├── SecondCountableQuotients/
│   │   │   ├── SigmaFiniteQuotients/
│   │   │   ├── SmoothCyclicVectors/
│   │   │   └── UniformCoefficientBounds/
│   │   ├── KFiniteAnalyticVectors/
│   │   │   ├── AdmissibleSmoothVectors/
│   │   │   ├── AnalyticIntertwiners/
│   │   │   ├── FundamentalDomainCusps/
│   │   │   ├── HaarBumpFunctions/
│   │   │   ├── OrbitDerivatives/
│   │   │   └── SmoothIrreducibility/
│   │   ├── LowKTypeMultiplicity/
│   │   │   ├── DiscreteSeriesCharacters/
│   │   │   └── EigenspaceCyclicDensity/
│   │   │       └── CreationOperators/
│   │   └── NonemptyRepresentations/
│   ├── RealGroups/
│   │   ├── BaseChange/
│   │   │   └── ArchimedeanBaseChange/
│   │   │       └── TensorCompletions/
│   │   │           └── SkewFieldFrames/
│   │   ├── DiscreteSeries/
│   │   │   └── DiscreteSeriesClassification/
│   │   │       ├── DiscreteSeriesExhaustion/
│   │   │       │   ├── FarRegularity/
│   │   │       │   ├── HeckeAlgebraActions/
│   │   │       │   │   ├── HeckeDuality/
│   │   │       │   │   ├── HeckeUnits/
│   │   │       │   │   ├── HeckeUnitTensors/
│   │   │       │   │   ├── ScalarCharacters/
│   │   │       │   │   ├── SimpleBackwardTransfer/
│   │   │       │   │   └── TensorReflections/
│   │   │       │   ├── MatrixCoefficientDecay/
│   │   │       │   │   ├── HilbertSchmidtDecay/
│   │   │       │   │   │   ├── DecayAssembly/
│   │   │       │   │   │   ├── HilbertSchmidtNorms/
│   │   │       │   │   │   └── RightKTypes/
│   │   │       │   │   ├── InfinitesimalCharacterPaths/
│   │   │       │   │   └── LineFormulas/
│   │   │       │   └── SimpleDistinctness/
│   │   │       ├── EquivariantSections/
│   │   │       ├── HilbertSpaceModels/
│   │   │       ├── InfinitesimalCharacters/
│   │   │       └── RhoRepresentations/
│   │   ├── FormalDegrees/
│   │   │   └── ArchimedeanFormalDegrees/
│   │   │       ├── DegreeNormalization/
│   │   │       ├── FormalDegreeFormula/
│   │   │       ├── MomentRecursion/
│   │   │       ├── PositiveConjugation/
│   │   │       └── SignDefiniteness/
│   │   ├── GeneralUnitaryRepresentations/
│   │   │   ├── ArchimedeanJacquetSegments/
│   │   │   │   └── SegmentSubquotients/
│   │   │   └── WhittakerModels/
│   │   └── UnitaryAdmissibility/
│   │       └── ArchimedeanUnitaryDual/
│   │           └── ArchimedeanDenseStabilizers/
│   ├── SpectralGeometry/
│   │   ├── CountingDefinitions/
│   │   │   ├── AdelicEulerProducts/
│   │   │   └── VoronoiMeans/
│   │   └── LocalGlobalProofs/
│   │       ├── AdelicAnalysis/
│   │       ├── ConvexCones/
│   │       ├── GlobalTheory/
│   │       ├── HermitianCharacters/
│   │       ├── LocalMassSeries/
│   │       ├── NefEffectiveCones/
│   │       ├── SmoothMorphisms/
│   │       ├── StableLattices/
│   │       └── WeylGroupActions/
│   └── ThickeningEstimates/
│       ├── InnerProductFactorization/
│       ├── LieGroupReduction/
│       │   └── MetaplecticRepresentation/
│       └── SiegelDomainEstimates/
├── Development/
│   ├── AbelianVarietyTheory/
│   │   ├── BlockTheory/
│   │   │   ├── AbelianSchemeLaw/
│   │   │   ├── AdelicCMFields/
│   │   │   ├── ArchimedeanEta/
│   │   │   ├── ClassSums/
│   │   │   ├── CMModuli/
│   │   │   ├── DivisorBase/
│   │   │   ├── EvidentLattices/
│   │   │   ├── ExistenceTori/
│   │   │   ├── GlobalSignature/
│   │   │   ├── GoodPlaces/
│   │   │   ├── HeightDefect/
│   │   │   ├── IrreducibleCharacters/
│   │   │   ├── JetGauges/
│   │   │   ├── NonGaloisCusps/
│   │   │   ├── PoincareCuspForms/
│   │   │   ├── RationalLaws/
│   │   │   ├── SiegelEisenstein/
│   │   │   ├── SiegelWeilLocal/
│   │   │   ├── ThetaLiftGeometry/
│   │   │   ├── TorsionBlocks/
│   │   │   ├── TwistedDiscreteSeries/
│   │   │   └── UniformisationCharts/
│   │   ├── Counterexamples/
│   │   │   ├── AbelianLawCounterexamples/
│   │   │   ├── AdelicSplittingExamples/
│   │   │   ├── AnisotropicRankZero/
│   │   │   ├── DegenerateExamples/
│   │   │   ├── HeckeCharacterExamples/
│   │   │   ├── HeightSurvey/
│   │   │   ├── JetSurvey/
│   │   │   ├── LevelGroupExamples/
│   │   │   ├── MetricPositivity/
│   │   │   ├── ModuliSurvey/
│   │   │   ├── NonGaloisSurvey/
│   │   │   ├── PlaceInjectivity/
│   │   │   ├── RotationExamples/
│   │   │   ├── SubgroupCharacterSums/
│   │   │   ├── ThetaValuation/
│   │   │   ├── TransversalityLocal/
│   │   │   ├── TwistSurvey/
│   │   │   ├── UniformisationSurvey/
│   │   │   ├── UniqueMatching/
│   │   │   └── UpperHalfSurvey/
│   │   ├── CrystallinePeriods/
│   │   │   └── CrystallineLogarithm/
│   │   ├── Definitions/
│   │   │   ├── AbelianSchemeLaws/
│   │   │   ├── AdelicHermitianForms/
│   │   │   ├── ArchimedeanThetaValues/
│   │   │   ├── AutomorphicMembership/
│   │   │   ├── CMLattices/
│   │   │   ├── CommutativeAlgebra/
│   │   │   ├── Degenerations/
│   │   │   ├── Divisors/
│   │   │   ├── ExistenceOfLattices/
│   │   │   ├── Foundations/
│   │   │   ├── GaloisGeometry/
│   │   │   ├── GlobalTwisting/
│   │   │   ├── HeightFunctions/
│   │   │   ├── HermitianLattices/
│   │   │   ├── Jets/
│   │   │   ├── KeyFormula/
│   │   │   ├── LatticeFrames/
│   │   │   ├── ModuliSpaces/
│   │   │   ├── NonGaloisDescent/
│   │   │   ├── PlaceAdaptation/
│   │   │   ├── QuasicoherentCohomology/
│   │   │   ├── RegularCharts/
│   │   │   ├── SemilocalFrames/
│   │   │   ├── ShimuraVarieties/
│   │   │   ├── SpanningFamilies/
│   │   │   ├── TeichmullerDepth/
│   │   │   ├── ThetaMetrics/
│   │   │   ├── ThetaValues/
│   │   │   ├── TorusSections/
│   │   │   ├── TwistedInnerProducts/
│   │   │   ├── TwoChartAtlas/
│   │   │   ├── Uniformization/
│   │   │   └── UpperBounds/
│   │   ├── Proofs/
│   │   │   ├── AbelianSchemeLawProofs/
│   │   │   ├── AdelicLatticeProofs/
│   │   │   ├── AlgebraicCurves/
│   │   │   ├── CharacterTheory/
│   │   │   ├── CoherentCohomologyProofs/
│   │   │   ├── CovolumeBounds/
│   │   │   ├── CubicalLineBundles/
│   │   │   ├── CuspFormEvaluations/
│   │   │   ├── DecoratedLatticeProofs/
│   │   │   ├── DegenerationProofs/
│   │   │   ├── DivisorProofs/
│   │   │   ├── FlagMeasures/
│   │   │   ├── FormalGroupCharts/
│   │   │   ├── FoundationProofs/
│   │   │   ├── GenericRegularity/
│   │   │   ├── GlobalInterpolation/
│   │   │   ├── HeightProofs/
│   │   │   ├── HermitianTraceForms/
│   │   │   ├── HomogeneousIdeals/
│   │   │   ├── InertiaEigenvalues/
│   │   │   ├── IwasawaDecomposition/
│   │   │   ├── JetHarmonics/
│   │   │   ├── ModuliProofs/
│   │   │   ├── RingsOfIntegers/
│   │   │   ├── SatakeParameters/
│   │   │   ├── SiegelThetaTransformation/
│   │   │   ├── ThetaFamilyOrigin/
│   │   │   ├── ThetaLawProofs/
│   │   │   ├── ThetaShiftProofs/
│   │   │   ├── ToricGeometry/
│   │   │   ├── TorusHaarMeasure/
│   │   │   ├── TorusSplitting/
│   │   │   ├── TwistedOperators/
│   │   │   ├── UniformizationProofs/
│   │   │   ├── UnitaryExistence/
│   │   │   └── UnramifiedDepth/
│   │   ├── PublishedTheorems/
│   │   │   ├── AbelianLaws/
│   │   │   ├── AdelicLattices₂/
│   │   │   ├── AutomorphicForms₂/
│   │   │   ├── BesselIntegrals/
│   │   │   ├── DefiniteCompactness/
│   │   │   ├── DiscreteSeriesUnitary₂/
│   │   │   ├── DiscreteSeries₂/
│   │   │   ├── Divisors₂/
│   │   │   ├── GaloisCohomology₂/
│   │   │   ├── GaloisGeometry₂/
│   │   │   ├── GlobalTheta/
│   │   │   ├── Landherr₂/
│   │   │   ├── PublishedFoundations/
│   │   │   ├── RelativeAmpleness/
│   │   │   ├── RosatiTraces/
│   │   │   ├── SemiabelianTori/
│   │   │   ├── SemistableReduction₂/
│   │   │   ├── SiegelWeil₂/
│   │   │   ├── ThetaCharacteristics/
│   │   │   ├── TwistedTraceFormula/
│   │   │   └── WeberRayClassFields/
│   │   └── Statements/
│   │       ├── ChartPoints/
│   │       ├── CuspFrameWeights/
│   │       ├── CuspidalUnitaryTwists/
│   │       ├── DiscreteSeriesShifts/
│   │       ├── EllipticCurveLevels/
│   │       ├── FundamentalDomains/
│   │       ├── HaarFundamentalDomain/
│   │       ├── HeckeInFamilies/
│   │       ├── HeckeThetaIntegrals/
│   │       ├── HeightBoundStatement/
│   │       ├── HyperbolicHypotheses/
│   │       ├── LocalTrivialization/
│   │       ├── PlaceShiftStatements/
│   │       ├── PrincipalLattices/
│   │       ├── SemistableTorsion/
│   │       ├── ShortVectorBound/
│   │       ├── ThetaLevelCharacters/
│   │       ├── TorsionEndomorphisms/
│   │       └── WeilDeligneCrystalline/
│   ├── AutomorphicArithmetic/
│   │   ├── AdelicGluing/
│   │   ├── AdelicQuotients/
│   │   ├── AdelicSL2/
│   │   ├── AutomorphicVarieties/
│   │   │   ├── AdditiveValuationNorms/
│   │   │   ├── AlgebraTools/
│   │   │   │   ├── ConnectedPrimeFields/
│   │   │   │   ├── DeterminantRepresentations/
│   │   │   │   ├── HidaCompleteRings/
│   │   │   │   ├── InducedAutomorphicForms/
│   │   │   │   └── MonomialRepresentations/
│   │   │   ├── AutomorphicCases/
│   │   │   ├── AutomorphicForms/
│   │   │   │   ├── ArchimedeanCompact/
│   │   │   │   ├── AutomorphicRankinSelberg/
│   │   │   │   ├── CoefficientSpans/
│   │   │   │   ├── CuspidalFiniteness/
│   │   │   │   ├── CuspidalTwists/
│   │   │   │   ├── FormsFiniteness/
│   │   │   │   ├── HeckeAdjoints/
│   │   │   │   ├── HermitianTwists/
│   │   │   │   ├── HomologyRank/
│   │   │   │   ├── L2Cusps/
│   │   │   │   ├── NewformCoefficients/
│   │   │   │   ├── QuadraticTwists/
│   │   │   │   ├── RealTransport/
│   │   │   │   ├── SiegelHeights/
│   │   │   │   ├── SignAgreement/
│   │   │   │   ├── SmoothRepresentationsGL/
│   │   │   │   ├── StrongMultiplicityOne/
│   │   │   │   ├── TemperedLocalComponents/
│   │   │   │   ├── TupleActions/
│   │   │   │   └── TwistedAutomorphicForms/
│   │   │   ├── BuildingsResidueChars/
│   │   │   ├── CharacterLevelBounds/
│   │   │   ├── CMFieldExponentialBounds/
│   │   │   ├── CommutativeAlgebra/
│   │   │   │   └── GradedModulesLength/
│   │   │   ├── CommutativeAlgebraHeight/
│   │   │   ├── ConjugateRepresentations/
│   │   │   │   ├── CobordismLinearRelations/
│   │   │   │   ├── ConjugateCuspidalReps/
│   │   │   │   ├── CuspidalSupport/
│   │   │   │   ├── LocalLimitConjugates/
│   │   │   │   └── PartitionSolutions/
│   │   │   ├── ConvexNerveComplexes/
│   │   │   ├── CurveDVRSpecialization/
│   │   │   │   └── SelfTwistEigenvalues/
│   │   │   ├── CyclotomicInertiaSpan/
│   │   │   ├── DotProductSymmetry/
│   │   │   ├── EisensteinModularTowers/
│   │   │   ├── FrobeniusSmoothVectors/
│   │   │   ├── GaloisCochains/
│   │   │   ├── GaloisLibrary/
│   │   │   │   ├── BernoulliNumbers/
│   │   │   │   ├── ClassFieldRamification/
│   │   │   │   ├── CrystallineBaseChange/
│   │   │   │   ├── FerreroWashingtonIndex/
│   │   │   │   ├── GaloisCohomologyLength/
│   │   │   │   ├── InfinitesimalCharacterPullback/
│   │   │   │   ├── KummerTheory/
│   │   │   │   ├── LocalRingsCompletion/
│   │   │   │   ├── SelmerTransport/
│   │   │   │   ├── SimultaneousEigenvectors/
│   │   │   │   ├── StickelbergerTheorem/
│   │   │   │   ├── WeylAlgebraQuantumDet/
│   │   │   │   ├── WeylCharacterRegularity/
│   │   │   │   └── WignerHighestWeights/
│   │   │   ├── GaussSumFiltrations/
│   │   │   ├── GeneratorCountTuples/
│   │   │   ├── GeometricSideEstimates/
│   │   │   ├── HeckeAlgebras/
│   │   │   │   ├── HeckeFixedLevelSpaces/
│   │   │   │   ├── HeckePolynomialTorsion/
│   │   │   │   ├── LocalUnitCase/
│   │   │   │   ├── OrdinaryHeckeCharacters/
│   │   │   │   └── UpOperatorEigenvalues/
│   │   │   ├── HeckeLevelRows/
│   │   │   ├── HeightAndVanishing/
│   │   │   ├── HermiteNormalForms/
│   │   │   ├── IdeleGenerators/
│   │   │   │   ├── AdjointLowWeight/
│   │   │   │   ├── ClosedHeckeCosets/
│   │   │   │   ├── HolomorphicIrreducibility/
│   │   │   │   ├── NormCongruenceUnits/
│   │   │   │   ├── QuadraticSplitting/
│   │   │   │   ├── ScalarStabilizers/
│   │   │   │   ├── ShortLatticeUnitarize/
│   │   │   │   │   └── CompactBoxLattices/
│   │   │   │   └── TorsionOrderFrobenius/
│   │   │   ├── IntegralityNearIdentity/
│   │   │   ├── IntegralPowerSeriesBounds/
│   │   │   ├── KisinPhiModules/
│   │   │   ├── LayeredIsomorphisms/
│   │   │   ├── LevelCohomology/
│   │   │   ├── LiteratureResults/
│   │   │   │   ├── AbelianUnitPowers/
│   │   │   │   ├── BorelHarmonicForms/
│   │   │   │   ├── CocycleCoefficients/
│   │   │   │   ├── DifferentialTranslates/
│   │   │   │   ├── JacquetLanglandsLattices/
│   │   │   │   ├── KatoEulerSystems/
│   │   │   │   ├── KisinCrystalline/
│   │   │   │   ├── KTheoryStability/
│   │   │   │   │   ├── FinitelyGeneratedTorsion/
│   │   │   │   │   ├── HomologicalStability/
│   │   │   │   │   │   └── LinkExactnessStability/
│   │   │   │   │   └── ReductionBoundsTorsion/
│   │   │   │   │       ├── AffineSplittingSpan/
│   │   │   │   │       ├── ArithmeticGapBounds/
│   │   │   │   │       ├── BaseChangeStability/
│   │   │   │   │       ├── CentralPositiveSemidefinite/
│   │   │   │   │       ├── CompactLocalSets/
│   │   │   │   │       ├── CycleBoundaryInjectivity/
│   │   │   │   │       ├── EvaluationSums/
│   │   │   │   │       ├── FiniteIndexCase/
│   │   │   │   │       ├── HeckeDoubleCosets/
│   │   │   │   │       ├── HeightContinuity/
│   │   │   │   │       ├── IntegralMomentReduction/
│   │   │   │   │       ├── IteratedHeckeBounds/
│   │   │   │   │       ├── MeanLatticeCounts/
│   │   │   │   │       ├── MomentEntryBounds/
│   │   │   │   │       │   └── UnitaryConeEstimates/
│   │   │   │   │       ├── OddSpanRank/
│   │   │   │   │       ├── OddWeightCycles/
│   │   │   │   │       ├── PartitionUnitySmooth/
│   │   │   │   │       ├── PermutationSigns/
│   │   │   │   │       ├── PrimitiveDiscriminants/
│   │   │   │   │       ├── PrimitiveSubmatrices/
│   │   │   │   │       ├── PrincipalPrimes/
│   │   │   │   │       ├── RationalSuccAbove/
│   │   │   │   │       ├── SeparationCase/
│   │   │   │   │       ├── SmoothCompositionIdentity/
│   │   │   │   │       ├── StokesSimplices/
│   │   │   │   │       ├── SurjectivityCase/
│   │   │   │   │       ├── TensorPrimeModuli/
│   │   │   │   │       ├── TorsionIntegers/
│   │   │   │   │       └── WhittakerSmoothForms/
│   │   │   │   ├── LieGeometryGrowth/
│   │   │   │   ├── MixedUnitCongruences/
│   │   │   │   ├── PrimeShapes/
│   │   │   │   ├── SymmetricAdjointFrobenius/
│   │   │   │   └── UnitaryDescent/
│   │   │   ├── ModularityArgument/
│   │   │   │   ├── ArchimedeanSchwartz/
│   │   │   │   │   ├── ArchimedeanDerivatives/
│   │   │   │   │   └── GenericFunctionalEquation/
│   │   │   │   ├── AutomorphyLifting/
│   │   │   │   │   ├── AdmissibleLevelRestriction/
│   │   │   │   │   ├── AutomorphyDescent/
│   │   │   │   │   │   └── InertiaRankTwo/
│   │   │   │   │   ├── LocalConditionCharacters/
│   │   │   │   │   ├── PAdicTorsionHoms/
│   │   │   │   │   ├── PolarizedLinkage/
│   │   │   │   │   ├── PrimeIndexConstruction/
│   │   │   │   │   ├── QuadraticCharpolySplitting/
│   │   │   │   │   ├── SubquotientSupport/
│   │   │   │   │   └── UnitaryGaloisFamilies/
│   │   │   │   ├── BaseChangeUnits/
│   │   │   │   │   ├── BaseChangeNorms/
│   │   │   │   │   ├── CentralResidueGroups/
│   │   │   │   │   └── SymmetricCubeUnits/
│   │   │   │   ├── ClassCounting/
│   │   │   │   │   ├── LatticeBlockClasses/
│   │   │   │   │   ├── LeftMultiplication/
│   │   │   │   │   ├── RingEquivalences/
│   │   │   │   │   ├── SelmerOrderCounts/
│   │   │   │   │   └── TorsionRankCounts/
│   │   │   │   ├── ClozelCohomology/
│   │   │   │   │   └── ContinuousEntryPairings/
│   │   │   │   ├── CrystallineOrdinaryIdeals/
│   │   │   │   ├── CuspidalDescent/
│   │   │   │   │   ├── GLDenseRanges/
│   │   │   │   │   │   └── InertiaPartMaps/
│   │   │   │   │   ├── SphericalTwists/
│   │   │   │   │   │   └── UnramifiedTwists/
│   │   │   │   │   └── UnitaryTorusDescent/
│   │   │   │   ├── CuspidalTwists/
│   │   │   │   │   └── FiniteOrderCongruences/
│   │   │   │   ├── GammaLaurentFactors/
│   │   │   │   │   ├── LaurentBlockInduction/
│   │   │   │   │   └── LocalEmbeddingNorms/
│   │   │   │   ├── InductionEstimates/
│   │   │   │   │   ├── BorelHeckeBounds/
│   │   │   │   │   │   └── HeckeShiftSums/
│   │   │   │   │   ├── IntegralCompression/
│   │   │   │   │   │   └── ContinuousEntryCharacters/
│   │   │   │   │   ├── IwahoriBlocks/
│   │   │   │   │   │   └── IwahoriCentralBorel/
│   │   │   │   │   ├── IwahoriHeckeInjectivity/
│   │   │   │   │   │   └── IdempotentTraces/
│   │   │   │   │   ├── SpectralOperatorNorms/
│   │   │   │   │   │   ├── ChebyshevNormEstimates/
│   │   │   │   │   │   └── HeightTwoBlocks/
│   │   │   │   │   ├── SplitUnramifiedInduction/
│   │   │   │   │   └── UnipotentBlockMatrices/
│   │   │   │   │       ├── ClosedKernelMinors/
│   │   │   │   │       └── ClosureOrbits/
│   │   │   │   ├── IntegralDeterminants/
│   │   │   │   ├── KatoQuadraticCharacters/
│   │   │   │   │   ├── EulerFactorBounds/
│   │   │   │   │   │   └── FrobeniusConjugateInertia/
│   │   │   │   │   ├── FrobeniusHodgeTateLaws/
│   │   │   │   │   ├── NewformTwistNorms/
│   │   │   │   │   ├── SmoothedZetaClasses/
│   │   │   │   │   ├── SphericalDecomposition/
│   │   │   │   │   ├── SymmetricPowerSymbols/
│   │   │   │   │   │   ├── ExponentialInjectivity/
│   │   │   │   │   │   ├── HolomorphicIntegrality/
│   │   │   │   │   │   ├── LocallyConstantFinite/
│   │   │   │   │   │   └── UniformizerIntegrality/
│   │   │   │   │   └── UnramifiedZeta/
│   │   │   │   ├── LeviSmoothLocalization/
│   │   │   │   │   ├── AdjointEta/
│   │   │   │   │   ├── LeviBlockInduction/
│   │   │   │   │   └── PrincipalSeriesMatching/
│   │   │   │   ├── LinkedUnramifiedChains/
│   │   │   │   │   ├── CrystallineCardinalities/
│   │   │   │   │   ├── DerivativeDivisibility/
│   │   │   │   │   ├── LogarithmicNormBounds/
│   │   │   │   │   ├── ScalarIrreducibility/
│   │   │   │   │   ├── TeichmullerParts/
│   │   │   │   │   │   └── SubalgebraIntegrality/
│   │   │   │   │   └── WeightInfinitesimalCharacters/
│   │   │   │   ├── MultiplicityOne/
│   │   │   │   │   ├── GeometricTraces/
│   │   │   │   │   └── HeckeIntegrability/
│   │   │   │   ├── OrdinaryJacquetModules/
│   │   │   │   ├── ScatteringLimits/
│   │   │   │   │   └── ConvolutionSpectra/
│   │   │   │   ├── SemisimpleLevels/
│   │   │   │   ├── SymmetricPowerTransfer/
│   │   │   │   │   ├── EndoscopicGroupCriteria/
│   │   │   │   │   ├── GeneralizedEigenspaces/
│   │   │   │   │   │   ├── CharacterShapes/
│   │   │   │   │   │   │   └── FiniteOrbits/
│   │   │   │   │   │   ├── GlobalRationalGL/
│   │   │   │   │   │   │   └── IntegralConjugation/
│   │   │   │   │   │   ├── PlacesOverFinite/
│   │   │   │   │   │   ├── ProjectionComponents/
│   │   │   │   │   │   ├── SmoothDepth/
│   │   │   │   │   │   │   └── OpenLevelSubgroups/
│   │   │   │   │   │   └── WeightKernels/
│   │   │   │   │   │       └── TwistRatios/
│   │   │   │   │   ├── GlobalUnitaryForms/
│   │   │   │   │   │   ├── IntegralStabilizers/
│   │   │   │   │   │   └── ScalarTuples/
│   │   │   │   │   ├── LocalHermitianForms/
│   │   │   │   │   │   ├── BilinearSmul/
│   │   │   │   │   │   ├── FixedPointCriteria/
│   │   │   │   │   │   ├── IrreducibleParity/
│   │   │   │   │   │   ├── LatticeFrames/
│   │   │   │   │   │   ├── LatticeProperties/
│   │   │   │   │   │   ├── LocalOrbitCounts/
│   │   │   │   │   │   ├── ScalingExistence/
│   │   │   │   │   │   └── SplitUnitElements/
│   │   │   │   │   ├── SignatureIntegrality/
│   │   │   │   │   │   └── SignatureTorusFixedPoints/
│   │   │   │   │   ├── TraceFormulaEigenvalues/
│   │   │   │   │   │   └── TraceFibreCardinality/
│   │   │   │   │   ├── UnlinkedHalfIntegral/
│   │   │   │   │   │   └── UnlinkedHeckeRoots/
│   │   │   │   │   ├── WeightTraceProducts/
│   │   │   │   │   │   └── WeightDeterminantTwists/
│   │   │   │   │   └── WeilDeligneUnramified/
│   │   │   │   │       └── WeilCharpolySupport/
│   │   │   │   ├── ThresholdArguments/
│   │   │   │   │   └── DenseThresholdCases/
│   │   │   │   ├── TopTheorem/
│   │   │   │   ├── TraceFormula/
│   │   │   │   │   ├── GaloisFromTraceFormula/
│   │   │   │   │   ├── GL1SpectralBounds/
│   │   │   │   │   ├── GL4GeometricSide/
│   │   │   │   │   ├── GL4HoweTheory/
│   │   │   │   │   ├── GlobalTraceComparison/
│   │   │   │   │   │   ├── AutomorphicRepresentations/
│   │   │   │   │   │   ├── CuspidalContribution/
│   │   │   │   │   │   ├── OrbitalCosetFiniteness/
│   │   │   │   │   │   └── TraceAsymptotics/
│   │   │   │   │   ├── OrbitalIntegrals/
│   │   │   │   │   │   └── TwistedOrbitalIntegrals/
│   │   │   │   │   └── SplitRigidity/
│   │   │   │   └── UpperTriangularPlaces/
│   │   │   │       └── NormalValuationBounds/
│   │   │   ├── NumberFieldTowers/
│   │   │   ├── OddResidueBounds/
│   │   │   ├── PadicHodgeTheory/
│   │   │   ├── PatchingModules/
│   │   │   │   ├── AnnihilatorBaseChange/
│   │   │   │   ├── ArchimedeanH0Cards/
│   │   │   │   ├── AutomorphicDetection/
│   │   │   │   ├── ChebotarevFamilies/
│   │   │   │   ├── ClosureConjugation/
│   │   │   │   ├── DegreeCountCohomology/
│   │   │   │   ├── DeterminantPadicFree/
│   │   │   │   ├── EpsilonEtaMatrices/
│   │   │   │   ├── NilpotentLevelLowering/
│   │   │   │   ├── PatchingBaseChange/
│   │   │   │   ├── SelmerScaling/
│   │   │   │   └── SeparableMatrixStability/
│   │   │   ├── PlacesOfRationals/
│   │   │   ├── PrimitiveFrobeniusFixed/
│   │   │   ├── PublishedTheorems/
│   │   │   ├── QuadraticExtensions/
│   │   │   ├── SelmerModuleFiniteness/
│   │   │   ├── SmallClassNumbers/
│   │   │   ├── StickelbergerCharacterEval/
│   │   │   ├── StickelbergerElements/
│   │   │   ├── SymplecticGSp4/
│   │   │   ├── TensorHomCubes/
│   │   │   ├── TheoremsMuLinked/
│   │   │   │   ├── CharacteristicPolynomials/
│   │   │   │   ├── ContinuousSubActions/
│   │   │   │   ├── CyclicReductionCohomology/
│   │   │   │   ├── DualModuleCocycles/
│   │   │   │   ├── GaloisRepresentationTypes/
│   │   │   │   ├── HidaOrdinaryHecke/
│   │   │   │   ├── MatrixIrreducibility/
│   │   │   │   ├── NilpotentHeckeOperators/
│   │   │   │   ├── NormsAndPolarizations/
│   │   │   │   ├── PurityTempered/
│   │   │   │   └── SpectralEigenvalues/
│   │   │   ├── TorsionBoundsChains/
│   │   │   ├── UnitaryThreeDeformations/
│   │   │   ├── UnitaryThreeGroups/
│   │   │   ├── WeakShimuraTheory/
│   │   │   │   ├── AdicExtensionMatrices/
│   │   │   │   ├── AdicLattices/
│   │   │   │   ├── AdjointCoefficients/
│   │   │   │   ├── AutomorphicCharacters/
│   │   │   │   ├── BlockMatrixPlaces/
│   │   │   │   ├── CharacteristicPolynomialRoots/
│   │   │   │   ├── CompactIntegralFields/
│   │   │   │   ├── DirichletGroupPowers/
│   │   │   │   ├── EigenbasisLifts/
│   │   │   │   ├── FibreTraces/
│   │   │   │   ├── FlagsAndDiagonals/
│   │   │   │   ├── FrobeniusDensity/
│   │   │   │   ├── FrobeniusFields/
│   │   │   │   ├── GradedFlagMoves/
│   │   │   │   ├── PhiCharacterResidues/
│   │   │   │   ├── PolynomialTori/
│   │   │   │   ├── ProjectiveLineFlags/
│   │   │   │   ├── RamifiedLineCharacters/
│   │   │   │   ├── RealPlaceConjugation/
│   │   │   │   ├── ResidualChains/
│   │   │   │   ├── ResidueFlagPoints/
│   │   │   │   ├── RootsOfUnityShapes/
│   │   │   │   ├── StabilizerIndexBounds/
│   │   │   │   ├── SymplecticIwahori/
│   │   │   │   ├── TwistedFourierKernels/
│   │   │   │   ├── UnipotentIdempotents/
│   │   │   │   └── ValuationCharacters/
│   │   │   ├── WeilGroupCharacters/
│   │   │   │   └── WeilCharactersModular/
│   │   │   └── WindowBoundReduction/
│   │   ├── BlochKatoExtensions/
│   │   ├── BlowupCategories/
│   │   ├── CharacterBoxes/
│   │   ├── CMTraceEmbeddings/
│   │   ├── CMTraceForms/
│   │   ├── CommutativeAlgebra/
│   │   │   └── EtaleCohomology/
│   │   │       └── EtaleAxioms/
│   │   ├── ConductorsKronecker/
│   │   ├── CoprimeRanks/
│   │   ├── CrystallineRing/
│   │   ├── CupPullbacks/
│   │   ├── CyclotomicBounds/
│   │   │   ├── ClassNumberBounds/
│   │   │   │   ├── AdditiveValuation/
│   │   │   │   ├── CyclotomicTotient/
│   │   │   │   ├── ExplicitConstants/
│   │   │   │   ├── HeckeCharacterChoice/
│   │   │   │   ├── IdealCounting/
│   │   │   │   ├── IdealValuations/
│   │   │   │   ├── InertiaRamification/
│   │   │   │   ├── IrreducibleSpans/
│   │   │   │   ├── SelmerDuality/
│   │   │   │   ├── TotallyRealRoots/
│   │   │   │   └── UnimodularGram/
│   │   │   ├── CyclotomicOrders/
│   │   │   ├── DeRhamLattices/
│   │   │   ├── NormSums/
│   │   │   ├── RamifiedDiscriminants/
│   │   │   ├── RootsOfUnity/
│   │   │   ├── TraceDuality/
│   │   │   └── WildJets/
│   │   ├── DedekindLFunctions/
│   │   │   └── LandauTheorems/
│   │   ├── DivisorFrames/
│   │   ├── EtaleIdempotents/
│   │   ├── EvenBoxes/
│   │   ├── ExponentialBounds/
│   │   ├── Foundations/
│   │   │   ├── BaseChangeIdentities/
│   │   │   │   ├── FrameMatching/
│   │   │   │   │   ├── GelfandReading/
│   │   │   │   │   ├── HeckeEigenvalueFiniteness/
│   │   │   │   │   └── HeckeWordBounds/
│   │   │   │   └── RealTraceClifford/
│   │   │   ├── Convolution/
│   │   │   │   ├── BlockEvaluation/
│   │   │   │   ├── BlockHeckeSlices/
│   │   │   │   │   └── CuspidalNormBounds/
│   │   │   │   ├── CentreSplitting/
│   │   │   │   ├── ConvolutionKernels/
│   │   │   │   │   ├── AnalyticSeries/
│   │   │   │   │   └── KernelTransforms/
│   │   │   │   ├── EndomorphismSlices/
│   │   │   │   │   ├── FiniteAdelicEstimates/
│   │   │   │   │   └── HeckeComponentVectors/
│   │   │   │   ├── GeneralizedMeasures/
│   │   │   │   │   └── MeasureConditions/
│   │   │   │   ├── HermitianDescent/
│   │   │   │   ├── IntegrableConvolution/
│   │   │   │   ├── LocalGroupAnalysis/
│   │   │   │   ├── NormCharacterPowers/
│   │   │   │   ├── OrbitNormCounting/
│   │   │   │   ├── PolynomialCoefficientBounds/
│   │   │   │   ├── PowerSumTraces/
│   │   │   │   ├── RealGroupAnalysis/
│   │   │   │   │   ├── CuspRegions/
│   │   │   │   │   ├── FockOperators/
│   │   │   │   │   ├── GaussianForms/
│   │   │   │   │   ├── GaussianProducts/
│   │   │   │   │   ├── IsotypicQuotients/
│   │   │   │   │   ├── ReductionDomains/
│   │   │   │   │   ├── SpecialLinearCosets/
│   │   │   │   │   ├── ThetaBounds/
│   │   │   │   │   ├── ThetaReindexing/
│   │   │   │   │   ├── UnitaryActions/
│   │   │   │   │   ├── UnramifiedSplitting/
│   │   │   │   │   └── WeilRepresentation/
│   │   │   │   ├── SphericalHeckeOperators/
│   │   │   │   ├── SphericalIdeles/
│   │   │   │   ├── SplitEigenfunctions/
│   │   │   │   │   ├── CharacterNorms/
│   │   │   │   │   ├── InfinitePlaceGluing/
│   │   │   │   │   └── OrbitMeasurability/
│   │   │   │   ├── TraceSplitting/
│   │   │   │   ├── TwistedLocalOrbits/
│   │   │   │   └── WeightRankUnits/
│   │   │   ├── EtaleClopenDescent/
│   │   │   ├── GaloisRepresentations/
│   │   │   │   ├── AdmissibleResidues/
│   │   │   │   │   └── CharpolyConjugation/
│   │   │   │   ├── AnnihilatorModels/
│   │   │   │   │   └── BrauerTraceSplitting/
│   │   │   │   ├── BaseChangeDescent/
│   │   │   │   ├── BasicOpenSections/
│   │   │   │   ├── BlockCharacterApproximation/
│   │   │   │   ├── CharpolyFromTrace/
│   │   │   │   ├── ClosedPhiFunctoriality/
│   │   │   │   ├── CommRingSections/
│   │   │   │   ├── CrystallineTowers/
│   │   │   │   ├── DefiniteTraceForms/
│   │   │   │   ├── FiniteEtaleModels/
│   │   │   │   ├── HeckeGaloisCriteria/
│   │   │   │   ├── InertiaQuadraticRamification/
│   │   │   │   ├── IntegralStructures/
│   │   │   │   │   ├── CongruenceOddLevel/
│   │   │   │   │   ├── CrystallineDescent/
│   │   │   │   │   ├── CrystallineInputs/
│   │   │   │   │   ├── GeometricFlagBases/
│   │   │   │   │   │   ├── FiniteEtaleClopen/
│   │   │   │   │   │   └── PrimeLevelLocalization/
│   │   │   │   │   │       └── CongruenceReduction/
│   │   │   │   │   ├── InertCharpoly/
│   │   │   │   │   └── ZetaCharacterDivisibility/
│   │   │   │   ├── IsogenyEtaleTranslation/
│   │   │   │   ├── IwahoriTypeSupport/
│   │   │   │   ├── JacobianTraceQuotients/
│   │   │   │   ├── KunnethLefschetz/
│   │   │   │   │   ├── DiagonalPullbacks/
│   │   │   │   │   ├── EtaleCharts/
│   │   │   │   │   │   ├── FlatSectionExtension/
│   │   │   │   │   │   └── PolynomialChartSpans/
│   │   │   │   │   └── ProjectiveBaseChange/
│   │   │   │   ├── LefschetzSigmaSums/
│   │   │   │   ├── LiftFactorization/
│   │   │   │   ├── LocalDoubleCosets/
│   │   │   │   ├── LocalMaximality/
│   │   │   │   ├── MixedUnlinkedExponents/
│   │   │   │   ├── PAdicHensel/
│   │   │   │   ├── PAdicWittLattices/
│   │   │   │   ├── PlainTorsionPairs/
│   │   │   │   ├── ProjectiveAutomorphicHecke/
│   │   │   │   │   └── CyclotomicConjugation/
│   │   │   │   ├── RadicalStalks/
│   │   │   │   ├── RankTwoPatching/
│   │   │   │   ├── RegularSemisimpleFibres/
│   │   │   │   │   ├── FrobeniusLocalPairs/
│   │   │   │   │   └── PowerMatchingTraces/
│   │   │   │   ├── ResidueExistence/
│   │   │   │   ├── ScalarCommutation/
│   │   │   │   ├── SchurDeterminants/
│   │   │   │   ├── SeparatingAlgebras/
│   │   │   │   ├── SphericalCoordinates/
│   │   │   │   │   └── AlgebraEquivSetup/
│   │   │   │   ├── SphericalGaloisCompatibility/
│   │   │   │   │   ├── PAdicSplitting/
│   │   │   │   │   └── ToralDeRham/
│   │   │   │   ├── StringRepresentations/
│   │   │   │   ├── ThetaParseval/
│   │   │   │   │   ├── BlockDeterminants/
│   │   │   │   │   │   └── ExponentialEntries/
│   │   │   │   │   ├── CartanIdeles/
│   │   │   │   │   ├── GoodLifts/
│   │   │   │   │   ├── HalfIndexLattices/
│   │   │   │   │   ├── IdeleNormCharacters/
│   │   │   │   │   ├── SatakeLifts/
│   │   │   │   │   ├── SplitLineSubtraction/
│   │   │   │   │   └── ThetaKernels/
│   │   │   │   ├── TraceLimits/
│   │   │   │   ├── TranscendenceTraces/
│   │   │   │   ├── TypeConditions/
│   │   │   │   └── WeightCharacters/
│   │   │   ├── IwahoriReduction/
│   │   │   │   ├── LangPolynomials/
│   │   │   │   ├── NormProducts/
│   │   │   │   └── SiegelFixedPoints/
│   │   │   ├── LocalLanglands/
│   │   │   │   └── LocalCentralUnits/
│   │   │   ├── PullbackRestriction/
│   │   │   ├── SubgroupJ/
│   │   │   └── UnitarySphericalFixing/
│   │   │       └── SatakeParameters/
│   │   │           ├── PotentialCrystallinity/
│   │   │           ├── SeparableConjugates/
│   │   │           └── SplitLevelConjugates/
│   │   ├── FrobeniusLocalisation/
│   │   ├── FrobeniusTwistedNorms/
│   │   ├── GenericGermInjectivity/
│   │   ├── IdeleLatticeFacts/
│   │   ├── IntegralCasts/
│   │   │   ├── AlgebraicInfinityType/
│   │   │   ├── CapelliIdentities/
│   │   │   │   ├── CapelliComplements/
│   │   │   │   └── SchwartzBilinear/
│   │   │   ├── CrystallinePeriods/
│   │   │   └── TransposeInverse/
│   │   ├── IwahoriCommensurability/
│   │   ├── KaehlerVanishing/
│   │   ├── LocalEmbeddings/
│   │   ├── LocalTestFunctions/
│   │   ├── LyingOver/
│   │   ├── MeanSquareBounds/
│   │   ├── NaturalDivisibility/
│   │   ├── OrbitLabellings/
│   │   ├── PAdicLatticeApproximation/
│   │   ├── PrimeDiscriminants/
│   │   ├── PrimitiveCosets/
│   │   ├── QuadraticCharacters/
│   │   ├── RealSpanData/
│   │   ├── RepresentationRank/
│   │   ├── ResidueCharacters/
│   │   ├── SemilinearForms/
│   │   ├── ShortNorms/
│   │   ├── SimultaneousEigenspaces/
│   │   ├── SpecialMaps/
│   │   ├── Splittings/
│   │   ├── TeichmullerLogarithm/
│   │   ├── ThetaCorrespondence/
│   │   │   ├── AlgebraicCharacters/
│   │   │   ├── BesselModels/
│   │   │   ├── CrystallineComparison/
│   │   │   ├── CuspidalSupport/
│   │   │   ├── FockModels/
│   │   │   │   ├── BoxIntegrals/
│   │   │   │   └── TiltedDrinfeld/
│   │   │   ├── GaloisRepresentations/
│   │   │   ├── GeneralLinearGroups/
│   │   │   ├── GoodReduction/
│   │   │   ├── HoweDuality/
│   │   │   ├── LocalComparison/
│   │   │   ├── LocalLanglands/
│   │   │   ├── PrismaticDieudonne/
│   │   │   ├── RallisInnerProduct/
│   │   │   ├── RealBands/
│   │   │   ├── ThetaPairLifts/
│   │   │   │   ├── HodgeBundleWeights/
│   │   │   │   ├── LocalTypeDictionary/
│   │   │   │   └── ThirdPlaceSeries/
│   │   │   └── WeilRepresentation/
│   │   ├── ThickFrames/
│   │   ├── TwistedTraces/
│   │   ├── UnipotentInvariants/
│   │   ├── UnitaryInvolutions/
│   │   ├── UnitTensorPairings/
│   │   ├── WeightCongruences/
│   │   └── WhittakerHecke/
│   ├── AutomorphicSpectrum/
│   │   ├── Definitions/
│   │   │   ├── AdelicLattices/
│   │   │   ├── CommutativeAlgebra/
│   │   │   ├── DivisibilityTowers/
│   │   │   ├── GlobalGeometry/
│   │   │   ├── JetCones/
│   │   │   ├── MembershipCriteria/
│   │   │   ├── MetricPeriods/
│   │   │   ├── NonGaloisLines/
│   │   │   ├── SemilocalProjection/
│   │   │   └── TwistedFlags/
│   │   ├── ParallelStatements/
│   │   │   ├── FiniteSums/
│   │   │   └── ParallelGeometry/
│   │   ├── Proofs/
│   │   │   ├── AdelicProofs/
│   │   │   ├── AlgebraProofs/
│   │   │   ├── BlockDecomposition/
│   │   │   ├── DivisibilityProofs/
│   │   │   ├── GeometryProofs/
│   │   │   ├── GlobalProofs/
│   │   │   ├── HermitianForms/
│   │   │   ├── JetProofs/
│   │   │   ├── MembershipProofs/
│   │   │   ├── MetricProofs/
│   │   │   ├── NonGaloisProofs/
│   │   │   ├── SemilocalMultiplicity/
│   │   │   └── TwistedProofs/
│   │   ├── PublishedTheorems/
│   │   │   ├── Algebra₂/
│   │   │   ├── Divisibility₂/
│   │   │   ├── Geometry₂/
│   │   │   ├── Jets₂/
│   │   │   ├── Metrics₂/
│   │   │   ├── PublishedGlobalResults/
│   │   │   └── SiegelWeil₂/
│   │   ├── RootSurvey/
│   │   │   └── GeometrySurvey/
│   │   └── Statements/
│   │       ├── AlgebraStatements/
│   │       ├── GeometryStatements/
│   │       ├── MetricStatements/
│   │       └── TowerExistence/
│   ├── DiscreteGroups/
│   │   ├── GlobalIrreducibility/
│   │   └── PiInvariants/
│   │       ├── CasimirInfinity/
│   │       └── CompactSupportTwists/
│   ├── EtaleCohomology/
│   │   ├── CohomologicalPurity/
│   │   ├── CyclotomicDiscriminants/
│   │   ├── DivisorCycles/
│   │   ├── EtaleDuality/
│   │   ├── EtaleSheaves/
│   │   │   ├── AdjoinRootExtension/
│   │   │   ├── AlgebraicIntegralClosure/
│   │   │   ├── BoundaryKernel/
│   │   │   ├── CechLevelIsomorphism/
│   │   │   ├── CechLevels/
│   │   │   ├── CechLevelsGeneration/
│   │   │   ├── ClosedPointLifts/
│   │   │   ├── CokernelKilling/
│   │   │   ├── ConeExcision/
│   │   │   ├── DescentInduction/
│   │   │   ├── DiagramChase/
│   │   │   ├── EtaleEmbedding/
│   │   │   ├── EtaleSpreading/
│   │   │   ├── HalfDegreeVanishing/
│   │   │   ├── IntegralNormalization/
│   │   │   ├── KernelLocalization/
│   │   │   ├── KummerFields/
│   │   │   ├── KummerInduction/
│   │   │   ├── KummerSequence/
│   │   │   ├── LocalDescent/
│   │   │   ├── LocalSlices/
│   │   │   ├── ProperLineCovers/
│   │   │   ├── PropertyDescent/
│   │   │   ├── SecondDegreeKilling/
│   │   │   ├── SheafIsomorphism/
│   │   │   ├── SpectrumLimits/
│   │   │   ├── StrictHenselColimits/
│   │   │   ├── StrictLocalStalks/
│   │   │   ├── SurjectiveCharts/
│   │   │   ├── TwistGenerators/
│   │   │   ├── UnitExistence/
│   │   │   └── ZeroSheafMaps/
│   │   ├── EtaleTrace/
│   │   │   └── LocalSplitting/
│   │   ├── KummerExtensions/
│   │   ├── KummerTheory/
│   │   ├── TateTwists/
│   │   │   └── TensorVanishing/
│   │   └── WeilConjectures/
│   ├── ResolutionOfSingularities/
│   │   ├── EmbeddedResolution/
│   │   │   ├── AlgebraicPreliminaries/
│   │   │   ├── DerivativeIdeal/
│   │   │   ├── EtaleCoordinates/
│   │   │   ├── IdealPrincipalization/
│   │   │   │   ├── ClosedEmbedding/
│   │   │   │   ├── DivisorReduction/
│   │   │   │   ├── MarkedBlowupSequence/
│   │   │   │   ├── MarkedOrderReduction/
│   │   │   │   ├── MonomialCase/
│   │   │   │   └── OrderReduction/
│   │   │   ├── IteratedBlowups/
│   │   │   ├── MaximalContactHypersurfaces/
│   │   │   ├── ResolutionDescent/
│   │   │   ├── StrictTransformCharts/
│   │   │   ├── StrictTransformIsolation/
│   │   │   └── StrongResolution/
│   │   └── Foundations/
│   │       ├── Blowup/
│   │       └── Schemes/
│   └── WeilBound/
│       ├── CoreStatements/
│       │   ├── AbelianDeRhamStructure/
│       │   │   └── AbelianDeRhamPages/
│       │   ├── AbelianHeightsDuality/
│       │   │   ├── AbelianHodgeDeRham/
│       │   │   ├── ArakelovSingularities/
│       │   │   ├── DividedPowerAlgebras/
│       │   │   ├── DixmierMalliavin/
│       │   │   ├── FubiniStudyChowHeight/
│       │   │   ├── GelfandKazhdanDuality/
│       │   │   ├── PublishedTheoremStatements/
│       │   │   ├── UnitarisableLocalReps/
│       │   │   ├── UnitaryDensity/
│       │   │   └── ZarhinTrick/
│       │   ├── AdicCompleteSpans/
│       │   ├── AmpleLineBundles/
│       │   ├── ArcCellEmbeddings/
│       │   ├── AutomorphicKernels/
│       │   │   ├── AbelianDeRham/
│       │   │   │   ├── AbelianHodgeDeRham/
│       │   │   │   ├── AbelianPullbackLattices/
│       │   │   │   ├── AbelianSchemeCharts/
│       │   │   │   ├── AbelianWedgeProducts/
│       │   │   │   └── ClosedPoints/
│       │   │   ├── ArchimedeanJacquetFirstTerm/
│       │   │   │   └── ArchimedeanWhittakerTrace/
│       │   │   ├── BernsteinUnitaryProducts/
│       │   │   │   ├── BernsteinTheoremA/
│       │   │   │   │   ├── ConjugationInvariantDistributions/
│       │   │   │   │   ├── FiberLocalization/
│       │   │   │   │   ├── FrobeniusReciprocity/
│       │   │   │   │   ├── LeviTransposeDistributions/
│       │   │   │   │   ├── TheoremAFromLeviTranspose/
│       │   │   │   │   └── UnitaryKirillovModel/
│       │   │   │   └── IrreducibleAdmissibleReps/
│       │   │   │       ├── AdmissibleParabolicInduction/
│       │   │   │       └── UnitaryAdmissibleComplements/
│       │   │   ├── DeligneRibet/
│       │   │   │   └── WeightedSummability/
│       │   │   ├── DepthZeroCuspidal/
│       │   │   │   └── DepthZeroMonomial/
│       │   │   ├── DeRhamPotentiallySemistable/
│       │   │   │   ├── DeRhamPlusCondition/
│       │   │   │   └── DeRhamTwists/
│       │   │   ├── DualAbelianScheme/
│       │   │   │   └── AbelianDeRhamDuality/
│       │   │   ├── EisensteinSeriesG2/
│       │   │   │   ├── AdelicHomeomorphisms/
│       │   │   │   ├── BlockTriangularFrames/
│       │   │   │   ├── CompactStandardSubgroup/
│       │   │   │   ├── G2HaarMeasure/
│       │   │   │   ├── G2RootData/
│       │   │   │   ├── HeisenbergTheta/
│       │   │   │   │   └── HeisenbergThetaConstant/
│       │   │   │   ├── RankOneEisenstein/
│       │   │   │   ├── SiegelGrowthForms/
│       │   │   │   ├── TubeDomainExtension/
│       │   │   │   └── UnitsBorelSpace/
│       │   │   ├── GrothendieckRingPolynomial/
│       │   │   ├── IsobaricBaseChange/
│       │   │   │   └── IntegralCoefficientBaseChange/
│       │   │   │       ├── ResidualRigidity/
│       │   │   │       ├── SplitRigidityRegularAlgebra/
│       │   │   │       └── UnitaryBaseChangeCharacters/
│       │   │   │           ├── UnitaryBaseChangeLemmas/
│       │   │   │           └── UnitaryBaseChangeLinks/
│       │   │   ├── LanglandsExhaustion/
│       │   │   ├── LocalGlobalCompatibility/
│       │   │   │   └── TemperedLocalGlobal/
│       │   │   │       └── WeilGroupRestriction/
│       │   │   ├── LocalLanglandsExistence/
│       │   │   ├── MoriwakiBigness/
│       │   │   │   ├── HilbertSamuelApplications/
│       │   │   │   ├── HilbertSamuelBlock/
│       │   │   │   ├── MoriwakiBigTheorem/
│       │   │   │   ├── MoriwakiRankBounds/
│       │   │   │   ├── MoriwakiSymmetry/
│       │   │   │   └── SegreJoinGeneration/
│       │   │   ├── NadelVanishing/
│       │   │   ├── RamifiedExponentBounds/
│       │   │   ├── ResidualSpectrumHilbertSum/
│       │   │   │   └── ResidualSpectrumTensors/
│       │   │   ├── SiegelWeilFormula/
│       │   │   │   ├── AdelicDilations/
│       │   │   │   ├── AdelicEisensteinSeries/
│       │   │   │   ├── AdelicFormCongruences/
│       │   │   │   ├── AwayActions/
│       │   │   │   ├── BilinearFormExamples/
│       │   │   │   ├── CayleyTransform/
│       │   │   │   ├── DarbouxCharts/
│       │   │   │   ├── DiagonalColumns/
│       │   │   │   ├── DilationDecomposition/
│       │   │   │   ├── EisensteinMeromorphy/
│       │   │   │   ├── FiniteLineActions/
│       │   │   │   ├── FockSpaces/
│       │   │   │   ├── FockVacuumBounds/
│       │   │   │   ├── FourierCompactness/
│       │   │   │   ├── HeightLattices/
│       │   │   │   ├── HolomorphicTheta/
│       │   │   │   ├── KFiniteVectors/
│       │   │   │   ├── LagrangianDecomposition/
│       │   │   │   │   └── DiagonalColumnInclusion/
│       │   │   │   ├── LocalCharacterIntegrals/
│       │   │   │   ├── LocalInvariantNeighborhoods/
│       │   │   │   ├── LocalOperatorBlocks/
│       │   │   │   ├── LocalUnitExistence/
│       │   │   │   ├── LocalWeilOperators/
│       │   │   │   ├── MassOneBase/
│       │   │   │   ├── MassOneCounts/
│       │   │   │   ├── NontrivialLocalCharacter/
│       │   │   │   ├── ParabolicBlockForms/
│       │   │   │   ├── PolynomialGaussianIntegrals/
│       │   │   │   ├── RationalCoordinates/
│       │   │   │   │   └── RationalCoordinateCountability/
│       │   │   │   ├── RationalHermitianMeasures/
│       │   │   │   ├── RationalWeilElements/
│       │   │   │   ├── RealAdelicFockSpace/
│       │   │   │   ├── RealGaussianTraces/
│       │   │   │   ├── SchrodingerCommutation/
│       │   │   │   ├── SiegelDensities/
│       │   │   │   ├── SiegelWeilActions/
│       │   │   │   ├── SiegelWeilStandard/
│       │   │   │   ├── SingularHermitian/
│       │   │   │   ├── ThetaAutomorphy/
│       │   │   │   ├── ThetaBijections/
│       │   │   │   ├── ThetaParabolic/
│       │   │   │   ├── ThetaPlaces/
│       │   │   │   ├── ThetaSchwartzSums/
│       │   │   │   ├── ThetaSplitting/
│       │   │   │   ├── TracePairSums/
│       │   │   │   ├── UnfoldingCompactness/
│       │   │   │   ├── UnipotentBorelTuples/
│       │   │   │   ├── UnitaryChartEquiv/
│       │   │   │   ├── UnramifiedWhittaker/
│       │   │   │   ├── VacuumIwasawa/
│       │   │   │   ├── WeilRepresentationGenerators/
│       │   │   │   ├── WeylIntegralCovariance/
│       │   │   │   ├── WeylTheta/
│       │   │   │   ├── WhittakerCovolume/
│       │   │   │   ├── WhittakerEqualRank/
│       │   │   │   ├── WhittakerGlobalFactors/
│       │   │   │   ├── WhittakerLowRank/
│       │   │   │   └── ZetaEulerProducts/
│       │   │   ├── SquareIntegrableSegments/
│       │   │   │   ├── SegmentProductEquivalence/
│       │   │   │   └── SegmentSubquotients/
│       │   │   ├── TemperedUnitNorm/
│       │   │   ├── UnitaryDualGL/
│       │   │   │   ├── GenericUnitaryDual/
│       │   │   │   ├── RecurrenceBaseChange/
│       │   │   │   └── TemperedEigenvalueNorms/
│       │   │   ├── UnitarySchrodingerModel/
│       │   │   │   └── UnitarySchrodingerLemmas/
│       │   │   │       ├── AlgebraMapEventually/
│       │   │   │       ├── BlockHeightDeterminants/
│       │   │   │       ├── BlockMulVec/
│       │   │   │       ├── FiniteMatchingK2/
│       │   │   │       ├── FockLatticeHeights/
│       │   │   │       ├── HaarFamilies/
│       │   │   │       ├── IwasawaReduction/
│       │   │   │       ├── LowRankSiegelDensities/
│       │   │   │       ├── MatrixInfinitySpan/
│       │   │   │       ├── RationalHermitianCountable/
│       │   │   │       ├── SchrodingerMatching/
│       │   │   │       ├── SphericalBigCell/
│       │   │   │       └── UnramifiedSchwartzDensity/
│       │   │   └── WeilSiegelFormula/
│       │   │       └── WeilSiegelSchwartz/
│       │   │           └── HermitianIntegrability/
│       │   ├── BetaInfinityCoefficients/
│       │   ├── BranchingTraces/
│       │   │   ├── BranchingComatrices/
│       │   │   ├── CasimirDecomposition/
│       │   │   └── HilbertSchmidtTraces/
│       │   ├── CentralCharts/
│       │   ├── CommonZeroEvaluation/
│       │   ├── CompactAveragingSplitting/
│       │   │   └── EigenvectorLifting/
│       │   ├── ComplexPeriods/
│       │   │   ├── ComplexPointPeriods/
│       │   │   └── FlatDegreeResidues/
│       │   ├── CrystallinePeriodRings/
│       │   ├── EqualVolumeCompactOpens/
│       │   ├── EulerCharacteristicCounts/
│       │   ├── FiniteTypeHarishChandra/
│       │   │   ├── GreenCuspLabels/
│       │   │   └── IntertwiningIsomorphisms/
│       │   ├── FlagImmersions/
│       │   ├── GaussianSeminormBounds/
│       │   │   └── RealSeminormFiltration/
│       │   ├── HeckeCharacterDeRham/
│       │   │   └── DeRhamHeckeResults/
│       │   │       ├── LAdicHeckeDeRham/
│       │   │       │   └── LAdicHeckeFields/
│       │   │       └── PotentiallySemistableDeRham/
│       │   │           └── SemistableDeRhamStatement/
│       │   ├── HodgeTatePoints/
│       │   ├── HomogeneousNonvanishing/
│       │   │   └── SpectralNormIntegrality/
│       │   ├── IdealCycleValues/
│       │   ├── IntegralPointHeights/
│       │   │   └── NegativeIntegralPoints/
│       │   ├── IntegralTransfer/
│       │   ├── JacobiBlockDeterminants/
│       │   ├── LocallyConstantCoinvariants/
│       │   ├── LocalModelCharts/
│       │   ├── LocalThetaKernels/
│       │   ├── MeasureExistence/
│       │   ├── MinimalPrimeDimensions/
│       │   ├── MultihomogeneousSquares/
│       │   ├── NefModelVolumes/
│       │   ├── OrbitDecayEstimates/
│       │   │   └── CurveDerivativeDecay/
│       │   ├── PadicHodgeComparison/
│       │   │   ├── CocharacterLieDivisors/
│       │   │   │   └── CocharacterLieAlgebra/
│       │   │   ├── EtaleCohomologyComparison/
│       │   │   │   ├── AcrisKummerUnits/
│       │   │   │   ├── BocksteinBaseChange/
│       │   │   │   │   ├── AdicCyclicCup/
│       │   │   │   │   ├── AdicTorsionCup/
│       │   │   │   │   ├── AdmissibleMinors/
│       │   │   │   │   ├── AtlasGroupActions/
│       │   │   │   │   ├── BocksteinSheafHomotopy/
│       │   │   │   │   ├── GammaIndependence/
│       │   │   │   │   ├── LimitBilinearCup/
│       │   │   │   │   ├── SmoothGaloisGeometry/
│       │   │   │   │   ├── TiltSectionUnits/
│       │   │   │   │   └── TranscendentalPeriodUnits/
│       │   │   │   ├── CechPairings/
│       │   │   │   ├── DifferentialFormsCech/
│       │   │   │   │   ├── AffineHodgeIsomorphisms/
│       │   │   │   │   ├── CechDifferentialPullback/
│       │   │   │   │   ├── CoverRefinementHodge/
│       │   │   │   │   └── GlobalDifferentialForms/
│       │   │   │   │       └── AffineOpenCaps/
│       │   │   │   ├── HodgeMatrices/
│       │   │   │   ├── HodgeTateResidues/
│       │   │   │   │   └── HodgeTateSpectral/
│       │   │   │   ├── KummerCupProducts/
│       │   │   │   ├── PerfectoidPullbacks/
│       │   │   │   │   ├── ConeSectionRestriction/
│       │   │   │   │   ├── DividedPowerReduction/
│       │   │   │   │   ├── FrobeniusFactorisation/
│       │   │   │   │   ├── FrobeniusWittActions/
│       │   │   │   │   │   └── FrobeniusNormBounds/
│       │   │   │   │   ├── GlobalSerreRelations/
│       │   │   │   │   ├── GradedChartDegrees/
│       │   │   │   │   ├── LevelChainValuations/
│       │   │   │   │   │   ├── GaloisCupProducts/
│       │   │   │   │   │   ├── RestrictionInclusions/
│       │   │   │   │   │   ├── RhoActionCup/
│       │   │   │   │   │   └── ValuationChainProofs/
│       │   │   │   │   ├── LocalisationLadders/
│       │   │   │   │   ├── LocalSystemQuotients/
│       │   │   │   │   ├── LogarithmicDerivatives/
│       │   │   │   │   ├── PeriodBaseChange/
│       │   │   │   │   ├── PolynomialSiteTraces/
│       │   │   │   │   ├── SplittingFieldLattices/
│       │   │   │   │   └── TwistedRepresentations/
│       │   │   │   ├── TeichmullerRootsUnity/
│       │   │   │   │   └── RootsUnityPullback/
│       │   │   │   ├── WittExactSequences/
│       │   │   │   └── ZariskiEtaleLifting/
│       │   │   ├── GoodCoverEigenspaces/
│       │   │   │   └── CubeCechEquivalences/
│       │   │   │       └── CechCubeBaseChange/
│       │   │   ├── HodgeSurjectivity/
│       │   │   │   ├── CupSurjectivity/
│       │   │   │   ├── EtaleChartBaseChange/
│       │   │   │   ├── NullClassVanishing/
│       │   │   │   └── RelativeLiftCosieves/
│       │   │   ├── KatzMessingTheorem/
│       │   │   ├── NormalSchemeSpectra/
│       │   │   ├── SaturatedBaseChange/
│       │   │   ├── TransferCocycles/
│       │   │   └── UniqueSaturation/
│       │   ├── PeriodRingComparison/
│       │   │   ├── AinfAlgebraMaps/
│       │   │   ├── AinfInverseMaps/
│       │   │   ├── CrystallinePeriodRings/
│       │   │   ├── PadicPeriodAlgebraMaps/
│       │   │   ├── PrimitiveEpsilon/
│       │   │   ├── RationalRingEquivalences/
│       │   │   ├── TeichmullerLogarithm/
│       │   │   └── ThetaKernelDeRham/
│       │   ├── PlaceConnectedComponents/
│       │   ├── PluriharmonicCharts/
│       │   ├── PlurisubharmonicCones/
│       │   ├── ProjectiveValuations/
│       │   ├── PublishedTheorems/
│       │   │   ├── CasselmanWallach/
│       │   │   ├── ClozelPurity/
│       │   │   ├── CuspidalMultiplicityOne/
│       │   │   ├── FiniteGLInvariants/
│       │   │   │   └── AffineLieInvariants/
│       │   │   ├── GlobalEulerCharacteristic/
│       │   │   │   └── GaloisCohomologyRatios/
│       │   │   ├── GlobalFiniteness/
│       │   │   ├── HeckeLAdicCharacters/
│       │   │   ├── JacquetShalikaBound/
│       │   │   ├── JacquetShalikaRigidity/
│       │   │   ├── LanglandsClassification/
│       │   │   ├── NadelVanishingPairs/
│       │   │   │   └── NadelVanishingLemmas/
│       │   │   ├── NefNumerics/
│       │   │   │   └── NefRiemannRoch/
│       │   │   ├── PoincareDeRhamDuality/
│       │   │   │   └── DeRhamPerfectPairing/
│       │   │   ├── PoitouTateDuality/
│       │   │   │   └── PoitouTateNineTerm/
│       │   │   ├── PolarizedGaloisRepresentations/
│       │   │   ├── PotentialSemistability/
│       │   │   ├── SegmentRepresentations/
│       │   │   ├── SiegelWeilSchrodinger/
│       │   │   └── SmoothVectorEstimates/
│       │   ├── RationalSupMetrics/
│       │   ├── RegularisedThetaMirabolic/
│       │   │   ├── CuspidalMirabolic/
│       │   │   └── KFiniteCuspForms/
│       │   ├── ResolutionCharZero/
│       │   ├── SatakeConjugation/
│       │   ├── SesquilinearFractions/
│       │   ├── StandardPublishedResults/
│       │   │   └── StandardTheoremStatements/
│       │   ├── TemperedRepresentationTheory/
│       │   │   ├── AffineGLForms/
│       │   │   │   ├── BlockMatrixIdentity/
│       │   │   │   └── CuspInvariantsFinite/
│       │   │   ├── ArakelovCycleHeights/
│       │   │   │   └── CycleHeightFormulas/
│       │   │   ├── BernsteinNarrowness/
│       │   │   │   └── BernsteinClosure/
│       │   │   ├── BernsteinZelevinskyGL/
│       │   │   ├── ChernDegreeComplex/
│       │   │   ├── ClozelPurity/
│       │   │   ├── CubeTheorem/
│       │   │   ├── CuspRapidDecayGL/
│       │   │   ├── DeRhamJacobian/
│       │   │   ├── DiscreteSeriesSU/
│       │   │   ├── EisensteinGrowthForms/
│       │   │   ├── FarguesExactness/
│       │   │   ├── FlatHermitianReps/
│       │   │   ├── FormalAlgebraisation/
│       │   │   ├── GelfandSpectralNormalisation/
│       │   │   │   └── NormalisedInvariants/
│       │   │   ├── GeometricSplitting/
│       │   │   ├── GermIntegrals/
│       │   │   ├── HodgeWedgeFields/
│       │   │   ├── HoweMaximalTori/
│       │   │   ├── IwasawaUnitaryAdelic/
│       │   │   ├── LeftZeroDuality/
│       │   │   ├── MetaplecticLowRank/
│       │   │   ├── MirabolicDerivatives/
│       │   │   │   ├── CuspGenericWhittaker/
│       │   │   │   ├── LeibnizDerivatives/
│       │   │   │   ├── SegmentCuspLines/
│       │   │   │   ├── TwistedKernels/
│       │   │   │   └── UnipotentDerivatives/
│       │   │   ├── MultiplicityOneRigidity/
│       │   │   ├── NefDivisors/
│       │   │   ├── PairSums/
│       │   │   ├── PlaneSupports/
│       │   │   ├── PoincareLelong/
│       │   │   ├── PrincipalSeriesSupport/
│       │   │   │   └── SeparatingWords/
│       │   │   ├── RegularClassTraces/
│       │   │   ├── SiegelFormulaSchwartz/
│       │   │   ├── SquareIdealLifts/
│       │   │   ├── SquareIntegrableTempered/
│       │   │   │   ├── CasselmanCriterion/
│       │   │   │   ├── CentredSegments/
│       │   │   │   └── TemperedProducts/
│       │   │   ├── WeilSiegelTheta/
│       │   │   ├── WeilThetaConvergence/
│       │   │   ├── ZarhinDualPolarisation/
│       │   │   │   └── FlatFiniteFibres/
│       │   │   └── ZelevinskyJacquet/
│       │   │       ├── FineJacquetModules/
│       │   │       ├── ZelevinskyCosocles/
│       │   │       ├── ZelevinskyExhaustion/
│       │   │       └── ZelevinskyInterleaving/
│       │   ├── ThetaDilations/
│       │   ├── TorusUniformisation/
│       │   │   ├── ChowMahlerFamilies/
│       │   │   ├── RepresentationHypotheses/
│       │   │   └── SiegelCompactSupport/
│       │   ├── TotallyDisjointProducts/
│       │   │   └── SLGLProductIrreducibility/
│       │   └── VolumeEquality/
│       ├── CuspidalAdmissibility/
│       ├── HeckeVectors/
│       │   ├── HeckeDoubleCosets/
│       │   │   ├── DoubleCosetLemmas/
│       │   │   └── HeckeCoefficientDegrees/
│       │   └── SmoothVectors/
│       │       ├── ContinuousUnits/
│       │       └── SobolevApproximation/
│       ├── KatoCoprimality/
│       │   └── CoprimePowers/
│       │       └── CoprimePowerSubOne/
│       ├── LevelCriteria/
│       ├── NonsplitUniqueness/
│       ├── RepresentationTheoryGL/
│       │   ├── ArchimedeanBaseChange/
│       │   │   ├── ArchimedeanBaseChangeProof/
│       │   │   │   ├── ArchimedeanGelfandKernels/
│       │   │   │   │   ├── EquivariantCalculus/
│       │   │   │   │   ├── FriedrichsKernels/
│       │   │   │   │   ├── GelfandEvenSmoothness/
│       │   │   │   │   ├── InfinitesimalCharacterGL/
│       │   │   │   │   └── LeftEquivariantFunctions/
│       │   │   │   │       ├── ComplexMatrixCalculus/
│       │   │   │   │       │   ├── AdjugateDifferentiability/
│       │   │   │   │       │   ├── ConjugateTransposeDerivatives/
│       │   │   │   │       │   ├── ContractionDerivatives/
│       │   │   │   │       │   ├── DeterminantPowerSmoothness/
│       │   │   │   │       │   ├── HaarGramPositivity/
│       │   │   │   │       │   ├── InverseLineDerivatives/
│       │   │   │   │       │   │   ├── DeterminantRankOneUpdate/
│       │   │   │   │       │   │   └── TraceModelAlgebra/
│       │   │   │   │       │   ├── KroneckerSmoothness/
│       │   │   │   │       │   └── MultiDiagonalTraces/
│       │   │   │   │       ├── GelfandFlags/
│       │   │   │   │       └── GLMatrixDerivatives/
│       │   │   │   ├── DescentTheorem/
│       │   │   │   ├── EigenvalueSeparation/
│       │   │   │   │   ├── AlmostEverywhereEigen/
│       │   │   │   │   │   └── PositiveMeasureNorms/
│       │   │   │   │   └── StableEigenspaces/
│       │   │   │   │       ├── CentralEigenvalues/
│       │   │   │   │       ├── FiniteTypes/
│       │   │   │   │       ├── SizeBounds/
│       │   │   │   │       └── StableHulls/
│       │   │   │   ├── FixedVectorVanishing/
│       │   │   │   ├── HeckeFubiniCompatibility/
│       │   │   │   ├── InfinitesimalCharacterLimits/
│       │   │   │   │   ├── ContinuousAdmissibleReps/
│       │   │   │   │   ├── InfinitesimalCharacterSpaces/
│       │   │   │   │   ├── IsometrySymmetry/
│       │   │   │   │   ├── LieSumDecompositions/
│       │   │   │   │   ├── LimitPairSpaces/
│       │   │   │   │   ├── PairSpaceGluing/
│       │   │   │   │   ├── SquareIntegrableAtPlace/
│       │   │   │   │   ├── TensorOperatorTrees/
│       │   │   │   │   ├── TreePrecursors/
│       │   │   │   │   ├── TwistLimitStatement/
│       │   │   │   │   ├── TwistStripLimits/
│       │   │   │   │   └── UntwistedCharacters/
│       │   │   │   ├── IsotropicMahlerBounds/
│       │   │   │   │   └── LogAbsoluteWedges/
│       │   │   │   ├── IwahoriFactorisation/
│       │   │   │   │   ├── MultiplicityOneBase/
│       │   │   │   │   ├── StrictDominance/
│       │   │   │   │   │   ├── JointGeneralisedEigenvectors/
│       │   │   │   │   │   ├── SatakeSocle/
│       │   │   │   │   │   └── UnitaryExtremality/
│       │   │   │   │   └── TwistedConjugationNorms/
│       │   │   │   │       └── HilbertNinetyNorms/
│       │   │   │   ├── IwahoriTrivialCase/
│       │   │   │   │   └── IwahoriTrivialLemmas/
│       │   │   │   ├── QuotientVanishing/
│       │   │   │   │   └── LocalQuotientIntegrals/
│       │   │   │   ├── RealDescent/
│       │   │   │   │   ├── LyingOverPrimes/
│       │   │   │   │   └── RealLeviDescent/
│       │   │   │   │       └── GlobalHarmonicExistence/
│       │   │   │   │           └── InvolutionIntegrals/
│       │   │   │   ├── SatakeExponents/
│       │   │   │   │   ├── FiniteDiscreteFamilies/
│       │   │   │   │   │   └── LocalCompatibilityGL/
│       │   │   │   │   ├── SatakeRigidity/
│       │   │   │   │   ├── SphericalEmbeddings/
│       │   │   │   │   └── UniformizerValuations/
│       │   │   │   │       ├── AdelicHeckeBlocks/
│       │   │   │   │       ├── BaseChangeWeyl/
│       │   │   │   │       ├── CharacterIntegrability/
│       │   │   │   │       ├── FixedSpaceRankOne/
│       │   │   │   │       ├── FrameBoundSpaces/
│       │   │   │   │       ├── FrameReading/
│       │   │   │   │       │   ├── BlockCandidates/
│       │   │   │   │       │   ├── FrobeniusWeights/
│       │   │   │   │       │   ├── GelfandValueContinuity/
│       │   │   │   │       │   └── LocalActionPowers/
│       │   │   │   │       ├── GrowthWeightBounds/
│       │   │   │   │       │   └── WeightExtensions/
│       │   │   │   │       │       └── WeightExtensionExistence/
│       │   │   │   │       ├── HermitianConvolution/
│       │   │   │   │       ├── HyperbolicEntryBounds/
│       │   │   │   │       ├── InertEigenvalues/
│       │   │   │   │       ├── InertFrames/
│       │   │   │   │       ├── LeviMatchingWords/
│       │   │   │   │       │   └── LeviMatchingBlocks/
│       │   │   │   │       ├── LocalOperatorSums/
│       │   │   │   │       ├── LocalSeparation/
│       │   │   │   │       │   └── LeafSeparation/
│       │   │   │   │       ├── PolynomialPairSpaces/
│       │   │   │   │       ├── QuadraticCharacterNorms/
│       │   │   │   │       ├── ShuffleChoices/
│       │   │   │   │       ├── SphericalHeckeUnitary/
│       │   │   │   │       ├── StrictJoinCandidates/
│       │   │   │   │       │   └── IntertwiningCandidates/
│       │   │   │   │       └── WordFrameBounds/
│       │   │   │   ├── ThetaCellCovers/
│       │   │   │   └── ThetaNormCommutation/
│       │   │   │       ├── FactorFields/
│       │   │   │       ├── LocalComparisonSplitting/
│       │   │   │       │   └── EulerFactorLevels/
│       │   │   │       └── WeylSplitting/
│       │   │   └── DiscreteSeriesTopClasses/
│       │   ├── CasimirAlgebra/
│       │   │   ├── KugaCoordinates/
│       │   │   │   ├── ArchimedeanWhittakerDerivatives/
│       │   │   │   ├── CasimirBounds/
│       │   │   │   ├── CochainExpansions/
│       │   │   │   ├── CoefficientGluing/
│       │   │   │   ├── CompactUnitaryGroups/
│       │   │   │   ├── DeterminantDerivative/
│       │   │   │   ├── EmbeddingConjugation/
│       │   │   │   ├── FrameExistence/
│       │   │   │   ├── GelfandValueOne/
│       │   │   │   ├── KugaAbsoluteValues/
│       │   │   │   ├── KugaGluing/
│       │   │   │   ├── MatrixConjugateSums/
│       │   │   │   ├── TensorFormCoordinates/
│       │   │   │   ├── UnitaryCurves/
│       │   │   │   └── UnitaryTwistCoordinates/
│       │   │   └── TensorRelationsGL/
│       │   ├── ConstantTermFiniteness/
│       │   │   ├── CuspidalConstantTerms/
│       │   │   └── LieInvariants/
│       │   ├── DiscreteSeries/
│       │   │   └── DiscreteSeriesCovers/
│       │   │       ├── DiscreteSeriesHilbert/
│       │   │       ├── EquivariantSections/
│       │   │       └── RhoRepresentations/
│       │   ├── EisensteinResidues/
│       │   │   └── AnisotropicGlobalForms/
│       │   │       └── SectionTrace/
│       │   ├── EisensteinSeries/
│       │   │   ├── SiegelEisensteinContinuation/
│       │   │   │   ├── EisensteinChartSplitting/
│       │   │   │   │   └── PositiveSumGrowth/
│       │   │   │   └── UniformTransfer/
│       │   │   └── SiegelEisensteinHalfPlane/
│       │   │       ├── IntegralUnitCoefficients/
│       │   │       ├── MirabolicGenerators/
│       │   │       ├── SchwartzBruhatMajorants/
│       │   │       ├── SiegelOneDescent/
│       │   │       ├── SphericalSplitting/
│       │   │       ├── StrongEisensteinBounds/
│       │   │       └── UnitTestFunctions/
│       │   ├── FormalDegree/
│       │   │   └── FormalDegreeHilbert/
│       │   │       ├── DegreeGapNorms/
│       │   │       ├── FormalDegreeFormula/
│       │   │       ├── KTypeRanges/
│       │   │       ├── MomentRecursion/
│       │   │       ├── OperatorNormSigns/
│       │   │       └── PositiveDefiniteConjugates/
│       │   ├── GaloisPermutationReps/
│       │   │   ├── SubquotientEquivalence/
│       │   │   │   └── CechDescentTests/
│       │   │   └── TameCongruences/
│       │   ├── GenericUnitaryGL/
│       │   │   ├── ComplementarySeries/
│       │   │   │   ├── HighestDerivativeProducts/
│       │   │   │   └── SegmentJacquetSubquotients/
│       │   │   ├── CuspidalGenericity/
│       │   │   ├── GenericUnlinkedGL/
│       │   │   ├── LeibnizOrders/
│       │   │   ├── NuPairInjectivity/
│       │   │   ├── SegmentDerivatives/
│       │   │   ├── SwapProducts/
│       │   │   ├── UnlinkedIrreducibility/
│       │   │   ├── WhittakerCuspidal/
│       │   │   ├── WhittakerHeredity/
│       │   │   └── WhittakerRankHeredity/
│       │   ├── HolomorphicDiscreteSeries/
│       │   │   ├── EmbeddedFrames/
│       │   │   ├── FlipDecomposition/
│       │   │   ├── HarishChandraDescent/
│       │   │   │   ├── AdjointSignSymmetry/
│       │   │   │   ├── ApproximationLemma/
│       │   │   │   ├── CasimirAdjoint/
│       │   │   │   ├── CasimirCommutation/
│       │   │   │   ├── CommutantLemma/
│       │   │   │   ├── DiscreteSeriesData/
│       │   │   │   ├── EmbeddingContinuity/
│       │   │   │   ├── FarWeightBounds/
│       │   │   │   ├── FrobeniusSpanDescent/
│       │   │   │   ├── HalfSumRootsIntegrality/
│       │   │   │   ├── IdentityLemma/
│       │   │   │   ├── IntegerLowerBounds/
│       │   │   │   ├── IntegralWeights/
│       │   │   │   ├── IrreducibleKTypes/
│       │   │   │   ├── MarkovInequality/
│       │   │   │   ├── MatrixEntryBounds/
│       │   │   │   ├── NormDifferenceBounds/
│       │   │   │   ├── PositiveNegativeWeights/
│       │   │   │   ├── ProjectionCommutation/
│       │   │   │   ├── RealInnerProducts/
│       │   │   │   ├── RealScalarParts/
│       │   │   │   ├── RhoAbsoluteBounds/
│       │   │   │   ├── RootDotNonnegativity/
│       │   │   │   ├── RootInnerBounds/
│       │   │   │   ├── SmoothTranslates/
│       │   │   │   ├── SquareAbsoluteBounds/
│       │   │   │   └── TraceSingleMoments/
│       │   │   ├── IntertwinerAdjoints/
│       │   │   ├── LowestKTypeModels/
│       │   │   ├── SchurEigenProjections/
│       │   │   │   ├── HolomorphicMoments/
│       │   │   │   ├── SchurFiniteDimensionality/
│       │   │   │   └── SeedBaseCases/
│       │   │   ├── WeightOccurrence/
│       │   │   └── WordSpans/
│       │   ├── JacquetShalikaBounds/
│       │   │   ├── AbsoluteRigidity/
│       │   │   │   ├── AbsoluteCharacterNorms/
│       │   │   │   ├── AbsoluteRigidityLemma/
│       │   │   │   ├── CauchyLocalisation/
│       │   │   │   ├── ConjugateAnalyticity/
│       │   │   │   ├── DeterminantCharacterSplit/
│       │   │   │   ├── DeterminantOneCharacters/
│       │   │   │   ├── DiagonalTermNorms/
│       │   │   │   ├── EulerLogarithms/
│       │   │   │   ├── LandauIteratedDerivatives/
│       │   │   │   ├── NewtonLowerBounds/
│       │   │   │   ├── NonnegativeCoefficients/
│       │   │   │   ├── PrimeNonSummability/
│       │   │   │   ├── RemovableSingularities/
│       │   │   │   ├── RigidityCriterion/
│       │   │   │   ├── SatakeTwists/
│       │   │   │   └── SubtypeIteSums/
│       │   │   └── CauchyIdentity/
│       │   │       ├── AlternantEvaluation/
│       │   │       ├── BetaGenerators/
│       │   │       ├── CauchyFormula/
│       │   │       ├── ContinuityOfH/
│       │   │       ├── HGenerators/
│       │   │       ├── JacobiTrudiPadding/
│       │   │       ├── PaddingMonotonicity/
│       │   │       ├── PolynomialGeometricSums/
│       │   │       ├── ProductCoefficients/
│       │   │       └── StaircaseDeterminants/
│       │   ├── LimitMultiplicityWeights/
│       │   │   └── RegularClassIntegrals/
│       │   ├── PeriodRingBases/
│       │   │   ├── AinfPlusInjectivity/
│       │   │   ├── BaseThetaVanishing/
│       │   │   ├── FixedBaseSurjectivity/
│       │   │   ├── PeriodRingUnits/
│       │   │   └── ThetaAlgebraMap/
│       │   ├── PointAveraging/
│       │   │   └── MinkowskiBalls/
│       │   ├── RegularisedSiegelWeil/
│       │   │   ├── HermitianCellMeasures/
│       │   │   ├── ResidueVanishing/
│       │   │   ├── SingularNullSets/
│       │   │   └── ThetaIdempotents/
│       │   │       └── ThetaCoefficients/
│       │   ├── ResidualSpectrum/
│       │   │   ├── DiscreteSpectrumUnitarity/
│       │   │   ├── ExponentialNegativity/
│       │   │   │   ├── AutomorphicLipschitz/
│       │   │   │   ├── BoxVolumes/
│       │   │   │   ├── CommonEigenvectors/
│       │   │   │   ├── ConjugationDifferences/
│       │   │   │   ├── ConstantTermSteps/
│       │   │   │   ├── DiagonalInfinityValues/
│       │   │   │   ├── ExponentialGluing/
│       │   │   │   ├── GapPairings/
│       │   │   │   ├── L2Gluing/
│       │   │   │   ├── LatticeReduction/
│       │   │   │   ├── NormalisedExistence/
│       │   │   │   ├── SquareIntegrableCovers/
│       │   │   │   ├── UniformInitialGrowth/
│       │   │   │   └── UnipotentVanishing/
│       │   │   ├── IwasawaCompletion/
│       │   │   └── SliceTensors/
│       │   │       └── PolynomialKilling/
│       │   ├── SiegelWeil/
│       │   │   └── ArchimedeanSiegelWeil/
│       │   │       └── PlaceIntegrals/
│       │   ├── SiegelWeilProof/
│       │   │   ├── BaseOneSide/
│       │   │   ├── BinaryMassMeans/
│       │   │   │   └── SingleRowSide/
│       │   │   ├── HolomorphicContinuation/
│       │   │   │   ├── AbsoluteConvergence/
│       │   │   │   ├── AnalyticDeterminants/
│       │   │   │   ├── CayleyCosetSums/
│       │   │   │   ├── GaussianPlaneIntegrals/
│       │   │   │   ├── GlobalGaussLaws/
│       │   │   │   ├── MinorFormulas/
│       │   │   │   ├── MollifiedIntegrability/
│       │   │   │   └── PolynomialDerivatives/
│       │   │   ├── IwasawaUnipotent/
│       │   │   └── PaddedMatrixIdentity/
│       │   ├── StandardBasisDerivatives/
│       │   │   └── ArchimedeanBasisDerivatives/
│       │   ├── TubeMeasures/
│       │   │   └── DisjointTubes/
│       │   │       ├── BoxExistence/
│       │   │       ├── ConstantSupremum/
│       │   │       ├── ExponentialThreeBound/
│       │   │       ├── FormalDegreeRankTwo/
│       │   │       ├── FrameCovolume/
│       │   │       ├── InverseMultiplication/
│       │   │       ├── LevelStabilisers/
│       │   │       ├── MeasureSumBounds/
│       │   │       ├── ProductMapEquality/
│       │   │       └── UpperFactors/
│       │   ├── TwistedFactors/
│       │   │   ├── AffineCharacterGenerators/
│       │   │   ├── CuspDecayHeights/
│       │   │   ├── GaloisGenerators/
│       │   │   ├── IntegralUnitBaseChange/
│       │   │   ├── LocalBaseChange/
│       │   │   │   ├── ElementaryCosets/
│       │   │   │   ├── ExponentSeparationLemma/
│       │   │   │   ├── GenericPrincipalSeries/
│       │   │   │   ├── LocalUnitNormIndex/
│       │   │   │   ├── StrictDominanceCasselman/
│       │   │   │   ├── TwistClassAssociation/
│       │   │   │   └── TwistedIndependenceLemma/
│       │   │   ├── SelmerRankBounds/
│       │   │   └── TruncatedCuspIrreducibility/
│       │   └── UnitaryDualProof/
│       │       ├── BernsteinExponentBounds/
│       │       ├── CentralProducts/
│       │       │   ├── CentralGenerators/
│       │       │   ├── EigenInjectivity/
│       │       │   ├── LeviScalars/
│       │       │   ├── PositiveProducts/
│       │       │   ├── SubquotientBounds/
│       │       │   └── UnitarisableHypotheses/
│       │       ├── CompactOrbits/
│       │       │   ├── AdjointSemisimple/
│       │       │   ├── Descent/
│       │       │   │   ├── CharpolyNilpotence/
│       │       │   │   ├── CommutingInverses/
│       │       │   │   ├── NilpotentPowers/
│       │       │   │   ├── OpenSlices/
│       │       │   │   │   └── LatticeIndices/
│       │       │   │   └── SliceVanishing/
│       │       │   │       ├── SemisimpleAdjoint/
│       │       │   │       └── Unimodularity/
│       │       │   ├── LocalContinuity/
│       │       │   ├── NilpotentOrbits/
│       │       │   │   ├── BaseOrbits/
│       │       │   │   ├── FourierTransforms/
│       │       │   │   ├── NilpotentHypotheses/
│       │       │   │   └── OrbitIntegrals/
│       │       │   │       ├── CentralizerRepresentatives/
│       │       │   │       ├── CompactPowers/
│       │       │   │       ├── IdempotentFibres/
│       │       │   │       ├── ModulusBounds/
│       │       │   │       ├── ModulusInduction/
│       │       │   │       └── SupportedComposition/
│       │       │   └── TraceAlgebra/
│       │       │       ├── CoefficientTraces/
│       │       │       ├── LinearConjugation/
│       │       │       ├── NilpotentTraces/
│       │       │       └── RestrictionHomomorphisms/
│       │       ├── FrobeniusReciprocity/
│       │       ├── GenericIrreducibility/
│       │       │   ├── CentralCharacterTheta/
│       │       │   ├── CentralCharacterZero/
│       │       │   ├── ContragredientSwap/
│       │       │   ├── FirstPairExistence/
│       │       │   ├── GenericUnitary/
│       │       │   ├── IrreducibleFactors/
│       │       │   └── ThetaProducts/
│       │       ├── HermitianForms/
│       │       │   ├── SelfAdjointForms/
│       │       │   │   ├── BesselEstimates/
│       │       │   │   ├── BlockContinuity/
│       │       │   │   ├── ColumnAlgebra/
│       │       │   │   ├── MirabolicVectors/
│       │       │   │   ├── SelfAdjointBounds/
│       │       │   │   ├── Stabilizers/
│       │       │   │   └── TwistedKernels/
│       │       │   ├── TransversalSums/
│       │       │   ├── UnipotentBounds/
│       │       │   └── UnitaryLattices/
│       │       │       ├── IsotropicAtoms/
│       │       │       ├── LatticeIndexLifts/
│       │       │       ├── PositiveShells/
│       │       │       ├── SmoothColumnLifts/
│       │       │       ├── SubquotientEigenvectors/
│       │       │       ├── UnitaryDensity/
│       │       │       └── UnitaryHypotheses/
│       │       ├── OpenCellDecomposition/
│       │       │   ├── OpenCellBlockShapes/
│       │       │   ├── OpenCellUnipotents/
│       │       │   └── PiTensorNontriviality/
│       │       ├── TraceDistributionsGL/
│       │       └── TwistedPieces/
│       │           ├── FiniteDimensionalDescent/
│       │           │   ├── ClosedOrbitPieces/
│       │           │   │   └── FrobeniusSections/
│       │           │   └── RestrictedCharpolys/
│       │           ├── IntegralParts/
│       │           │   ├── BaseVanishing/
│       │           │   ├── BezoutHypotheses/
│       │           │   ├── HaarFourierSupport/
│       │           │   ├── IntegralPartFibres/
│       │           │   ├── LocallyConstantCosets/
│       │           │   └── QuasiOrbits/
│       │           │       ├── HomomorphismContinuity/
│       │           │       ├── ModulusHeights/
│       │           │       ├── ModulusSquares/
│       │           │       └── OrbitRepresentatives/
│       │           └── LocalTraceForms/
│       │               └── SymmetricIndices/
│       ├── SimpleEigenvalues/
│       │   └── SimpleEigenvalueExtension/
│       ├── SupplementaryPages/
│       └── ThetaLifts/
│           ├── CartanFactorisation/
│           ├── ConeHypotheses/
│           ├── DoubleEigenvalues/
│           ├── EigenvalueEndgame/
│           │   ├── CuspidalAverages/
│           │   ├── EigenKilling/
│           │   ├── OrthogonalDecomposition/
│           │   ├── SignatureSplitting/
│           │   └── UnipotentGroups/
│           ├── FrameEstimates/
│           │   └── InitialPairs/
│           ├── LatticeBasics/
│           ├── LeviDeterminants/
│           │   ├── CharacterAdmissibility/
│           │   ├── LagrangianUniqueness/
│           │   └── MixedModels/
│           │       └── MixedModelPlanes/
│           ├── LocalTheory/
│           │   ├── ArchimedeanBumps/
│           │   ├── ConeShifts/
│           │   ├── DixmierCommutants/
│           │   ├── StandardValuations/
│           │   ├── ToralCohomology/
│           │   └── UnramifiedCohomology/
│           ├── Reductions/
│           │   ├── FiniteClosure/
│           │   ├── MetaplecticDerivatives/
│           │   ├── TopPolarZero/
│           │   ├── WeightConstants/
│           │   └── WeilPairs/
│           │       ├── WeilPairData/
│           │       └── WeilPairExistence/
│           ├── SchwartzMoments/
│           ├── SmallCones/
│           ├── SphericalLattices/
│           │   └── SphericalClosure/
│           ├── SphericalSplitting/
│           ├── TowerModels/
│           │   └── TwistedSums/
│           └── WeilDomination/
├── Formalism/
│   ├── AdicCompletionExports/
│   │   ├── AdicCompleteRingEquiv/
│   │   └── NonnegativeDivisors/
│   ├── AdmissibleDesigns/
│   ├── AlgebraicWeights/
│   ├── AlphaUniqueness/
│   ├── ArtinHasse/
│   │   └── ArtinHasseProofs/
│   ├── BehrendSets/
│   │   └── BehrendVariance/
│   ├── BranchSandwichDivisors/
│   │   └── BranchIsometryProofs/
│   ├── CharacterColumnKernels/
│   │   └── IdempotentNormalForms/
│   ├── CMTypeGalois/
│   │   └── CMTypeFrobenius/
│   ├── CoboundaryTransfers/
│   │   └── GammaStableTransfers/
│   ├── ConjugateSelfDual/
│   ├── CorankShare/
│   │   └── CorankShareProofs/
│   ├── CyclotomicNorms/
│   │   └── NonsquarefreeBounds/
│   ├── DegreeFormula/
│   │   └── PointDegree/
│   ├── DirichletDensity/
│   │   └── DirichletDensityProofs/
│   ├── DistinguishedUnitIdeals/
│   │   └── DistinguishedOrderProofs/
│   ├── DivisorInequality/
│   │   └── DivisorInequalityProofs/
│   ├── DoubleCosetMeasures/
│   │   └── LowerUnipotentOrbits/
│   ├── DropLevelBounds/
│   │   └── ConstantCoeffVanishing/
│   ├── EisensteinCokernelLengths/
│   │   └── FactorialValuationBounds/
│   ├── EllipticTorsion/
│   │   └── EllipticTorsionProofs/
│   ├── FilteredPoleLength/
│   │   ├── LocalDescentLevels/
│   │   └── ReducedBasisBounds/
│   ├── FlagUnipotentLattices/
│   │   └── MinkowskiFactorialBounds/
│   ├── FockGram/
│   │   └── FockGramProofs/
│   ├── FormalDegreeBessel/
│   │   └── FormalDegreeRatio/
│   ├── FormalGroupLog/
│   │   └── FormalGroupLogProofs/
│   ├── FormalGroupWitt/
│   │   └── FormalGroupWittProofs/
│   ├── FrobeniusBaseCase/
│   │   └── FrobeniusBaseCaseProofs/
│   ├── FrobeniusContraction/
│   │   └── FrobeniusContractionProofs/
│   ├── FrobeniusOrbits/
│   │   └── FrobeniusOrbitsProofs/
│   ├── GaloisCohomology/
│   │   └── GaloisCohomologyProofs/
│   ├── GaloisIrreducibility/
│   │   └── GaloisIrreducibilityProofs/
│   ├── GammaFactorNonvanishing/
│   ├── GaussIdealIdentity/
│   │   └── GaussIdealPrimality/
│   ├── GaussJetBounds/
│   │   ├── GaussJetProofs/
│   │   └── OneLetterGaussJets/
│   │       └── OneLetterGaussProofs/
│   ├── GaussValuationBounds/
│   │   └── GaussValueContraction/
│   ├── GelfandTransference/
│   │   └── HadamardGelfand/
│   ├── GL3MeanSquares/
│   │   ├── GenusMeanAsymptotics/
│   │   │   ├── JacobiCharacterSums/
│   │   │   │   └── ExceptionalCharacterBounds/
│   │   │   ├── LogEightBound/
│   │   │   └── UnimodularClassRepresentatives/
│   │   └── HookFormulaTorsion/
│   ├── GradedWeylDivisibility/
│   │   └── FockSpaceTableaux/
│   ├── GrowthSums/
│   │   └── FactorialBaseGrowth/
│   ├── HalfLinks/
│   ├── HarderNarasimhan/
│   │   └── HarderNarasimhanProofs/
│   ├── HermitianCurvature/
│   │   └── HermitianCurvatureProofs/
│   │       └── BesselDecayBounds/
│   │           ├── BesselIntegrability/
│   │           ├── BesselUnitNorm/
│   │           │   └── BesselNormSteps/
│   │           │       ├── BesselLine/
│   │           │       └── UnitNorm/
│   │           ├── DecayZeroRight/
│   │           ├── GrowthIntegrals/
│   │           ├── HaarCompactGrowth/
│   │           ├── NonnegNormSums/
│   │           └── SchurDecayBounds/
│   ├── HermitianLattices/
│   │   └── HermitianLatticesProofs/
│   ├── HyperbolicPlaceProducts/
│   │   └── SubgroupIndexCounts/
│   ├── IncomingBounds/
│   │   └── FlowDegreeBounds/
│   ├── JacobiWeightFamilies/
│   ├── JacquetSubsetSums/
│   ├── JumpKernelCokernel/
│   │   └── JumpShiftProofs/
│   ├── LagrangeIdealLifts/
│   │   └── CocyclePolynomialDivision/
│   ├── LandauZeroFreeBounds/
│   │   └── ExceptionalZeroBounds/
│   ├── LatticeLocalGlobal/
│   ├── LatticeRigidity/
│   │   └── HeightMinimum/
│   ├── LatticeSlopes/
│   │   └── LatticeSlopesProofs/
│   ├── LatticeTheta/
│   │   └── LatticeThetaProofs/
│   ├── LFunctionBounds/
│   │   └── LFunctionBoundsProofs/
│   ├── LocalRingCardinality/
│   │   ├── AdicCompletionLocal/
│   │   └── SpanPowerMembership/
│   ├── LocalToGlobal/
│   │   ├── AdelicCompactOpens/
│   │   ├── AlgebraicTheory/
│   │   │   └── AlgebraicTheoryProofs/
│   │   ├── BesselHermitianTheta/
│   │   ├── CharacterGerms/
│   │   ├── CMDeterminantIdeals/
│   │   │   └── CMIdealValuations/
│   │   ├── Columns/
│   │   │   ├── CoefficientsModP/
│   │   │   ├── ColumnDeterminants/
│   │   │   └── ColumnsProofs/
│   │   ├── CyclotomicLocalNorms/
│   │   ├── Divisibility/
│   │   │   ├── DivisibilityConstruction/
│   │   │   ├── DivisibilityProofs/
│   │   │   ├── DivisibilityRemainder/
│   │   │   │   ├── AdmissibleClasses/
│   │   │   │   ├── LinkedMeasures/
│   │   │   │   ├── NoColumnCase/
│   │   │   │   ├── RationalColumns/
│   │   │   │   ├── RemainderBounds/
│   │   │   │   ├── SharpFunctions/
│   │   │   │   └── ValueBounds/
│   │   │   └── JetBounds/
│   │   │       ├── JetBoundsProofs/
│   │   │       └── JetCounting/
│   │   │           ├── JetCountingProofs/
│   │   │           └── ScaledNorms/
│   │   ├── ExponentGrids/
│   │   │   └── ExponentGridsProofs/
│   │   ├── GaloisLevelStructure/
│   │   ├── GenusGluing/
│   │   │   └── GenusApproximation/
│   │   │       └── GenusApproximationProofs/
│   │   ├── GlobalTheory/
│   │   │   ├── BlockActions/
│   │   │   ├── CoordinateLengths/
│   │   │   ├── GL1/
│   │   │   │   └── CompactFixesLattice/
│   │   │   ├── GL2/
│   │   │   ├── GL3/
│   │   │   │   └── CubicFields/
│   │   │   │       ├── ComplexMultiplication/
│   │   │   │       ├── ConjugateSets/
│   │   │   │       ├── DedekindFactorization/
│   │   │   │       ├── DifferentIdeal/
│   │   │   │       ├── EisensteinSeries/
│   │   │   │       ├── EpsteinZeta/
│   │   │   │       ├── PeriodRelations/
│   │   │   │       └── WeierstrassUniqueness/
│   │   │   ├── GL4/
│   │   │   ├── GL5/
│   │   │   ├── GL6/
│   │   │   │   └── DiagonalSlopes/
│   │   │   ├── JetPositivity/
│   │   │   ├── UnramifiedDiagonal/
│   │   │   ├── UnramifiedTrace/
│   │   │   └── VolumeCarry/
│   │   ├── GroupLattices/
│   │   │   ├── CloudFilling/
│   │   │   ├── ComparisonMaps/
│   │   │   ├── FockModels/
│   │   │   │   ├── FlatModels/
│   │   │   │   └── TransposeWords/
│   │   │   │       └── TransposeWordsProofs/
│   │   │   ├── JointServices/
│   │   │   ├── LevelCharts/
│   │   │   ├── LevelGatherings/
│   │   │   ├── PendingLemmas/
│   │   │   ├── PerfectRings/
│   │   │   ├── StabilizerCount/
│   │   │   ├── TiedFamilies/
│   │   │   └── TrivialTransfer/
│   │   ├── HeckeThetaElements/
│   │   ├── HermitianColumns/
│   │   ├── HermitianForms/
│   │   ├── HilbertRowConditions/
│   │   ├── IndefiniteForms/
│   │   │   └── IndefiniteTree/
│   │   │       └── RealCubicMeans/
│   │   │           ├── LeafBounds/
│   │   │           │   ├── ArchimedeanLeaf/
│   │   │           │   ├── IntegralLeaf/
│   │   │           │   ├── LeafMeans/
│   │   │           │   ├── MeanMaxLeaf/
│   │   │           │   ├── OneSquareLeaf/
│   │   │           │   └── PackedMeans/
│   │   │           │       └── IndexMeans/
│   │   │           └── LogMeanShares/
│   │   │               └── LogMeanStatements/
│   │   ├── IndefiniteReal/
│   │   │   ├── DoubleCosetOperators/
│   │   │   ├── FinitePlaces/
│   │   │   ├── FockTheta/
│   │   │   ├── FrameExistence/
│   │   │   ├── HaarTransfer/
│   │   │   ├── HeckeNonvanishing/
│   │   │   ├── LeafObjects/
│   │   │   ├── LevelTypeEquivalence/
│   │   │   ├── LocalNormSurjectivity/
│   │   │   ├── NormalDecomposition/
│   │   │   ├── RationalAdjoints/
│   │   │   ├── RealSeparation/
│   │   │   └── SobolevIteration/
│   │   ├── InertKernelTheory/
│   │   │   └── InertCoprimeLemmas/
│   │   ├── JointCharacters/
│   │   ├── KernelLattices/
│   │   │   ├── ColumnData/
│   │   │   │   └── ColumnDataEquations/
│   │   │   ├── DeterminantCokernelCount/
│   │   │   │   └── CokernelIndexFactors/
│   │   │   └── KernelLocalFactors/
│   │   │       ├── HermitianHalfLattice/
│   │   │       ├── LocalProductMeasures/
│   │   │       ├── SelfDualLatticeNorms/
│   │   │       └── ThetaLocalEquivalence/
│   │   ├── LatticeGeometry/
│   │   │   ├── GeometryDefinitions/
│   │   │   ├── OperatorNormFibers/
│   │   │   ├── PluckerHadamard/
│   │   │   └── RealizationNorms/
│   │   ├── LocalInduction/
│   │   ├── NormalizedHeckeFactors/
│   │   ├── NumberFieldFamilies/
│   │   ├── PairingIndexBounds/
│   │   │   ├── HalvesRecursion/
│   │   │   │   ├── BoundedHalfModels/
│   │   │   │   │   └── AdicBoxOpenness/
│   │   │   │   └── RecursiveLatticeMembership/
│   │   │   ├── LatticeNormPowers/
│   │   │   │   └── CloseUnitNorms/
│   │   │   ├── ModelLatticeMoves/
│   │   │   │   └── ModelIndexPairings/
│   │   │   ├── OrthogonalChartLevels/
│   │   │   ├── PendingAdmissibility/
│   │   │   │   └── LocalFDerivAdmissibility/
│   │   │   ├── RowActionCoefficients/
│   │   │   │   └── AdmissibleInterpolation/
│   │   │   └── SplitPairEquations/
│   │   │       ├── IntegralSquareRoots/
│   │   │       ├── SplitTripleEquations/
│   │   │       ├── SquareSplitPairs/
│   │   │       └── TripleSumIndependence/
│   │   ├── PlaceMapInjectivity/
│   │   ├── ProjectiveLattices/
│   │   │   ├── ArchimedeanQuadraticData/
│   │   │   │   ├── ArchimedeanUniqueness/
│   │   │   │   ├── ArcLineFunctions/
│   │   │   │   ├── ArcWitnessExistence/
│   │   │   │   ├── DegreeInfimum/
│   │   │   │   ├── FinitePlaceArcs/
│   │   │   │   └── MaximalCuspKernels/
│   │   │   ├── LocalIntegralPolynomials/
│   │   │   ├── LocalUnitReduction/
│   │   │   └── RosatiLatticeNorms/
│   │   ├── RatioJoints/
│   │   ├── SiegelLatticeTheory/
│   │   │   ├── BesselDiscreteSeries/
│   │   │   ├── CasimirReductionTheory/
│   │   │   │   └── OneParameterDerivatives/
│   │   │   │       ├── AdmissibleCasimirScalars/
│   │   │   │       │   └── SmoothGeneratorAverages/
│   │   │   │       ├── TauReduction/
│   │   │   │       │   └── BlockGramReduction/
│   │   │   │       └── WeilIndicatorMeasures/
│   │   │   ├── CasimirVolumeRatios/
│   │   │   │   └── VolumeClassRepresentatives/
│   │   │   ├── ClosedLocalOrbits/
│   │   │   │   └── GaugeLatticeShifts/
│   │   │   │       ├── IndexCocycleOrbits/
│   │   │   │       ├── LieAveraging/
│   │   │   │       ├── RelativeIndexFlags/
│   │   │   │       └── StabilizerIndexVolumes/
│   │   │   ├── ClosedVolumeStatements/
│   │   │   ├── CokernelGLCounts/
│   │   │   │   └── RankPointCounts/
│   │   │   │       ├── DualFamilyCounting/
│   │   │   │       ├── RowFrameCoherence/
│   │   │   │       ├── SharpDualSpans/
│   │   │   │       └── ThetaModuleTransport/
│   │   │   │           ├── HeadColumnCoordinates/
│   │   │   │           │   ├── CornerDeterminantCounts/
│   │   │   │           │   ├── DeterminantUnitTheta/
│   │   │   │           │   ├── FormInverseCounting/
│   │   │   │           │   ├── FormPairAlgebra/
│   │   │   │           │   ├── SharpSpanCounting/
│   │   │   │           │   ├── ThetaLocalCount/
│   │   │   │           │   ├── UnitaryGramLifts/
│   │   │   │           │   ├── UnitaryThetaVanishing/
│   │   │   │           │   └── UnitShiftSplitting/
│   │   │   │           └── LocalCountConclusions/
│   │   │   ├── FlagStabilizerTensors/
│   │   │   │   └── RootLatticeThresholds/
│   │   │   │       ├── CompactCellConvergence/
│   │   │   │       └── CompactCovering/
│   │   │   ├── FundamentalEquivalence/
│   │   │   │   └── FundamentalContinuity/
│   │   │   ├── HaarTransversals/
│   │   │   │   └── UnitaryHaarProducts/
│   │   │   │       ├── LocalWeightCharts/
│   │   │   │       └── SplitPrimeCounts/
│   │   │   ├── SiegelMassRatios/
│   │   │   ├── TraceIntegralEstimates/
│   │   │   └── WeightedGaugeFactors/
│   │   ├── ThetaOperatorCommutation/
│   │   ├── TorsionIntegrality/
│   │   │   ├── CMGoodModels/
│   │   │   ├── ComplexLatticeClosure/
│   │   │   │   └── LatticeAreaPositivity/
│   │   │   ├── EisensteinTranslationProducts/
│   │   │   │   └── AnalyticIdentityTheorems/
│   │   │   ├── FrobeniusFibreCurves/
│   │   │   │   └── LogarithmicSubstitution/
│   │   │   ├── GaussianEigenFrames/
│   │   │   │   └── GramFrameComposition/
│   │   │   ├── GaussSumParity/
│   │   │   │   └── KummerThetaLogarithms/
│   │   │   ├── QuadraticSemicharacters/
│   │   │   │   └── CayleyGaussianIntegrals/
│   │   │   ├── RamifiedCurveKernels/
│   │   │   │   └── PairedSquareJets/
│   │   │   ├── SecondCoefficientNorms/
│   │   │   │   └── BinomialSeriesCoefficients/
│   │   │   ├── TorsionTranslationPowers/
│   │   │   │   └── NonsingularJetNorms/
│   │   │   ├── UniformGaussModels/
│   │   │   │   └── OrthogonalGaussModels/
│   │   │   │       └── HermitianBlockFrames/
│   │   │   └── WeierstrassTwoTorsion/
│   │   │       └── WeierstrassSubstitution/
│   │   └── UnitaryNorms/
│   ├── LogFactorialBounds/
│   │   └── LogFactorialProofs/
│   ├── LogFactorialIndices/
│   │   └── SignedSubspaceIndex/
│   ├── LogSumExpBounds/
│   │   └── CharacterSumPhase/
│   ├── LogVandermondeBounds/
│   │   └── LogVandermondeProofs/
│   ├── MahlerMeasure/
│   │   └── MahlerMeasureProofs/
│   ├── MeanHeightDescent/
│   │   └── AverageDegreeBounds/
│   ├── MirabolicMackeyTheory/
│   │   └── MirabolicMackeyProofs/
│   ├── MoebiusJetDuality/
│   ├── MonomialMeanResidues/
│   │   └── MonomialMeanProofs/
│   ├── NormUnitaryBounds/
│   │   └── DetPolynomialWeights/
│   ├── PadicSubsetSums/
│   │   ├── CentralIdempotents/
│   │   └── StableGradedCounts/
│   ├── PairingDivisors/
│   │   └── PairingDivisorProofs/
│   ├── PeriodIntegrals/
│   │   ├── AdmissibleModel/
│   │   ├── ExplicitFormulaCounts/
│   │   ├── GeometricProductPowers/
│   │   ├── HermitianGenusExtension/
│   │   │   └── SemilocalHermitianLattices/
│   │   ├── JointBlockShapes/
│   │   ├── NablaSpans/
│   │   ├── OrbitalBoundsConclusion/
│   │   └── UnitaryGroupMassFormula/
│   │       ├── AdaptedCharacterForm/
│   │       ├── AdditiveIntegralGroups/
│   │       ├── AdelicClassFiniteness/
│   │       ├── AdelicIndexEquality/
│   │       ├── AdelicLocalCompactness/
│   │       ├── AdelicUnimodularity/
│   │       ├── AdelicUnitaryOrbits/
│   │       ├── AdicCompactDensity/
│   │       ├── AdicFiniteOrder/
│   │       ├── AdicIntegersCompact/
│   │       ├── AdjointInverseTranslate/
│   │       ├── AlgebraicValuesFinite/
│   │       ├── ArchimedeanCoefficientNonzero/
│   │       ├── ArchimedeanOrbitMeasures/
│   │       ├── ArtinSchreierRoots/
│   │       ├── BallQuotientLength/
│   │       ├── BaseLengthBound/
│   │       ├── BesselDerivatives/
│   │       ├── BesselLeviAction/
│   │       ├── BesselSquareIntegrable/
│   │       ├── BetaIndependence/
│   │       ├── BetaModuloX/
│   │       ├── BetaUniqueness/
│   │       ├── BiadditiveCubes/
│   │       ├── BiadditivePadicLinear/
│   │       ├── BigCellConjugation/
│   │       ├── BlockEigenvalues/
│   │       ├── BochnerTheorem/
│   │       ├── BorderMinorRotation/
│   │       ├── BorderSignIdentity/
│   │       ├── BoundarySlices/
│   │       ├── CapelliEigenvalues/
│   │       ├── CauchyBinet/
│   │       ├── CayleyIrreducibility/
│   │       ├── CentralCharacters/
│   │       ├── ChainRuleSecondOrder/
│   │       ├── ChainRuleSmooth/
│   │       ├── CharacterExtension/
│   │       ├── CharacterIdempotents/
│   │       ├── CharacterNormMatrixInverse/
│   │       ├── ChebyshevPrimeBounds/
│   │       ├── CircleGaugeAction/
│   │       ├── ClassNumberIntegrality/
│   │       ├── CMDegreeEquality/
│   │       ├── CMDiscriminantSquare/
│   │       ├── CMEulerProducts/
│   │       ├── CMLatticeAreaFormula/
│   │       ├── CMTraceSurjective/
│   │       ├── CMTypeEmbeddings/
│   │       ├── CoefficientBaseChange/
│   │       ├── CommutingMultiplicity/
│   │       ├── CompactGelfandAverage/
│   │       ├── CompactGroupIntegrability/
│   │       ├── CompactTensorDensity/
│   │       ├── CompletionDegrees/
│   │       ├── CompletionExistence/
│   │       ├── ComplexDoubleCosets/
│   │       ├── CongruenceGainBound/
│   │       ├── ConjugateNormBound/
│   │       ├── ConjugateTransposeLeibniz/
│   │       ├── ConjugationInvariance/
│   │       ├── ConstantCoefficientKernel/
│   │       ├── ConvolutionProjection/
│   │       ├── CountableBasisPullback/
│   │       ├── CountingFormula/
│   │       ├── CountNonIntegrality/
│   │       ├── CountPositivity/
│   │       ├── CovariantDeterminantScaling/
│   │       ├── CovariantHatDecomposition/
│   │       ├── CovariantHatPairReindex/
│   │       ├── CovariantLinearProduct/
│   │       ├── CovariantVectorMove/
│   │       ├── CoveringRadius/
│   │       ├── CovolumeFrames/
│   │       ├── CrossDiagonalMatching/
│   │       ├── CubeFormalIdentities/
│   │       ├── CubicExponentialFactor/
│   │       ├── CyclicSplitting/
│   │       ├── DensityLemma/
│   │       ├── DerivativePreservation/
│   │       ├── DeterminantIdentity/
│   │       ├── DeterminantKernelFiniteness/
│   │       ├── DeterminantKernelOrder/
│   │       ├── DiagonalPadicSubstitution/
│   │       ├── DiagonalRank/
│   │       ├── DoubleSumSwap/
│   │       ├── DualCountBound/
│   │       ├── DualGramSubstitution/
│   │       ├── DyadicPrimeIntervals/
│   │       ├── DyadicStableLattices/
│   │       ├── EagonNorthcottComplex/
│   │       ├── EagonNorthcottIntegral/
│   │       ├── EmbeddingPermutations/
│   │       ├── EmbeddingTraceSum/
│   │       ├── EmbeddingTraceSumAlt/
│   │       ├── EntrywiseSandwichCommute/
│   │       ├── EvenPowerSeries/
│   │       ├── ExplicitFormula/
│   │       ├── ExponentialCoefficientSeries/
│   │       ├── ExponentialFactorIdentity/
│   │       ├── ExponentialFirstColumn/
│   │       ├── ExponentialIntegrality/
│   │       ├── ExponentialMinorLower/
│   │       ├── ExponentialMinorRays/
│   │       ├── ExponentialTriangular/
│   │       ├── FibreOrbits/
│   │       ├── FiltrationLength/
│   │       ├── FiniteAdelicComparison/
│   │       ├── FiniteExtensionTopology/
│   │       ├── FiniteOrderReduction/
│   │       ├── FiniteOrderValuation/
│   │       ├── FixedDimensionCount/
│   │       ├── FlagClassConstancy/
│   │       ├── FlagGramNonnegativity/
│   │       ├── FlagScalarRelevance/
│   │       ├── FockDegreeOne/
│   │       ├── FockHarmonicSplitting/
│   │       ├── FockJointMultiplicity/
│   │       ├── FockRaisingLowering/
│   │       ├── FockWeightDegree/
│   │       ├── FoldingUnfolding/
│   │       ├── FormalDegreeGap/
│   │       ├── FormalDegreeScaling/
│   │       ├── FormalDegreeSquareIntegrable/
│   │       ├── FormalGroupChords/
│   │       ├── FormalGroupCommon/
│   │       ├── FormalGroupPoints/
│   │       ├── FormalGroupSplitting/
│   │       ├── FormalGroupTriangles/
│   │       ├── FourSquareQuaternions/
│   │       ├── FrameDeterminant/
│   │       ├── FrameInduction/
│   │       ├── FrameTransport/
│   │       ├── FunctionalEquationSeries/
│   │       ├── FundamentalDomainTransfer/
│   │       ├── GaloisTorsionConjugacy/
│   │       ├── GaussianDualMeasure/
│   │       ├── GaussianUniqueness/
│   │       ├── GelfandPairConvolution/
│   │       ├── GelfandTsetlinBranching/
│   │       ├── GelfandTsetlinLowering/
│   │       ├── GelfandTsetlinTopCoefficient/
│   │       ├── GeneralLinearCardBound/
│   │       ├── GeneralLinearLevel/
│   │       ├── GenericRatioBound/
│   │       ├── GeometricProductBound/
│   │       ├── GlobalFormGenerator/
│   │       ├── GordanIntegerMultiple/
│   │       ├── GramDifferenceRenaming/
│   │       ├── GramFibrationFormulas/
│   │       ├── GramInjectivity/
│   │       ├── GramIsometryCoefficient/
│   │       ├── GramSchmidtFrames/
│   │       ├── GramSubstitutionIntegral/
│   │       ├── GramUnitMultiplication/
│   │       ├── GreenLabelCharpoly/
│   │       ├── GreenLabelSurjective/
│   │       ├── HaarFibreUniqueness/
│   │       ├── HaarScaling/
│   │       ├── HalfIntegerGap/
│   │       ├── HarishChandraLabels/
│   │       ├── HasseDerivativeFiltration/
│   │       ├── HasseJacobsonPowers/
│   │       ├── HasseOrderBound/
│   │       ├── HeckeLocalProduct/
│   │       ├── HenselianStabilizerConjugacy/
│   │       ├── HenselOpenValuation/
│   │       ├── HermitianClassFiniteness/
│   │       ├── HermitianCovectors/
│   │       ├── HermitianDefiniteOrthonormal/
│   │       ├── HermitianDiagonalization/
│   │       ├── HermitianFormalDegree/
│   │       ├── HermitianFrameExistence/
│   │       ├── HermitianFrameIso/
│   │       ├── HermitianGroupLattices/
│   │       ├── HermitianHaarMeasure/
│   │       ├── HermitianLatticeFiniteness/
│   │       ├── HighestWeightConjugacy/
│   │       ├── HighestWeightFixedLine/
│   │       ├── HighestWeightFixedVectors/
│   │       ├── HighestWeightIrreducible/
│   │       ├── HighestWeightUniqueness/
│   │       ├── HilbertSchmidtBlocks/
│   │       ├── HodgeFontaineExactness/
│   │       ├── HookLengthBound/
│   │       ├── HostFieldFacts/
│   │       ├── HostPrimeSplitting/
│   │       ├── IdealLatticeBasis/
│   │       ├── IdeleClassFiniteness/
│   │       ├── IdeleUnitsOpen/
│   │       ├── IdempotentTransfer/
│   │       ├── IdentityCellTrace/
│   │       ├── ImaginaryQuadraticClassBound/
│   │       ├── IndexCalculation/
│   │       ├── IndexUpperBound/
│   │       ├── InertDensity/
│   │       ├── InertPrimeJacobi/
│   │       ├── InertPrimeTeichmuller/
│   │       ├── InertUnitProduct/
│   │       ├── InfiniteEtaGenerators/
│   │       ├── InfiniteMeasureTransfer/
│   │       ├── InfinityTypeCharacter/
│   │       ├── IntegerCoordinatesZero/
│   │       ├── IntegerProductCast/
│   │       ├── IntegerSubgroupIntersection/
│   │       ├── IntegralityAtPrimeLattices/
│   │       ├── IntegralityUnderRingMap/
│   │       ├── IntegralSpanAlgebra/
│   │       ├── IntegralSymplectic/
│   │       ├── InvariantAlgebraComparison/
│   │       ├── InvariantMetricIsometry/
│   │       ├── InvariantTopologyComparison/
│   │       ├── InvertibleIdealIndex/
│   │       ├── IrreducibleCharacterSeries/
│   │       ├── IrreducibleFinrankOne/
│   │       ├── IsometryDerivative/
│   │       ├── IsometryDeterminant/
│   │       ├── IsometryDualPair/
│   │       ├── IsometryFunctionSpace/
│   │       ├── IsometryScaleCount/
│   │       ├── IwasawaMeasureExistence/
│   │       ├── JacobianCommutation/
│   │       ├── JacobianTransvectionSplitting/
│   │       ├── JetIntegrality/
│   │       ├── KernelSplitting/
│   │       ├── KFiniteSmoothVectors/
│   │       ├── KoszulExactness/
│   │       ├── LandherrUnitNorm/
│   │       ├── LargeStabilizerInverse/
│   │       ├── LatticeArea/
│   │       ├── LatticeAutomorphismApprox/
│   │       ├── LatticeAutomorphismFiniteness/
│   │       ├── LatticeColumns/
│   │       ├── LatticeCountingBound/
│   │       ├── LatticeIndexDeterminant/
│   │       ├── LatticeIndices/
│   │       ├── LatticeMultiplicity/
│   │       ├── LatticeReferenceFrame/
│   │       ├── LatticeSizeContinuity/
│   │       ├── LatticeSupremumLine/
│   │       ├── LatticeTransference/
│   │       ├── LeafCoefficientValuation/
│   │       ├── LeftPhaseRule/
│   │       ├── LeftQuantumMinor/
│   │       ├── LengthIndex/
│   │       ├── LevelImageArithmetic/
│   │       ├── LevelLiftBasics/
│   │       ├── LevelProductIndex/
│   │       ├── LevelSplitting/
│   │       ├── LevelStructures/
│   │       ├── LevelTransfer/
│   │       ├── LFunctionEvaluation/
│   │       ├── LFunctionMinors/
│   │       ├── LinearProgramLowerBound/
│   │       ├── LineScalingNorm/
│   │       ├── LocalBasisAtPrime/
│   │       ├── LocalCartanPairs/
│   │       ├── LocalDensityCorank/
│   │       ├── LocalDifferentGenerators/
│   │       ├── LocalDualGenerator/
│   │       ├── LocalEndomorphisms/
│   │       ├── LocalGlobalInclusion/
│   │       ├── LocalGlobalLattice/
│   │       ├── LocalGluing/
│   │       ├── LocalHaarSubgroup/
│   │       ├── LocalJacobianOrder/
│   │       ├── LocalJacobianType/
│   │       ├── LocalLatticeEquality/
│   │       ├── LocalLatticeIsomorphism/
│   │       ├── LocalLatticeSaturation/
│   │       ├── LocalMassOrder/
│   │       ├── LocalMassType/
│   │       ├── LocalOrderProjection/
│   │       ├── LocalPrimitiveFrame/
│   │       ├── LocalProductFormula/
│   │       ├── LocalResidueCharacter/
│   │       ├── LocalUnimodularLattice/
│   │       ├── LocalUnitaryOrbits/
│   │       ├── LocalVolumeIndices/
│   │       ├── LowerShearHaar/
│   │       ├── LowerSmoothStability/
│   │       ├── LowerUnipotentSplit/
│   │       ├── MajorantVanishing/
│   │       ├── MassComputations/
│   │       ├── MatrixCoefficientBound/
│   │       ├── MaximalCompactConjugacy/
│   │       ├── MeasureDecomposition/
│   │       ├── MeasureInverseContraction/
│   │       ├── MertensLogSum/
│   │       ├── MinimalLatticeNorm/
│   │       ├── MinkowskiBound/
│   │       ├── MinkowskiIdealBound/
│   │       ├── MinkowskiTorsionFree/
│   │       ├── MinorExpansion/
│   │       ├── MinorSmoothness/
│   │       ├── MinorSpanComplement/
│   │       ├── MirabolicBound/
│   │       ├── MirabolicIndex/
│   │       ├── MiracleFlatness/
│   │       ├── MirrorDecomposition/
│   │       ├── MonicShiftEvaluation/
│   │       ├── MonomialFrameSpan/
│   │       ├── MultiplicityMeasurability/
│   │       ├── NilpotentVolumeOne/
│   │       ├── NonzeroDiscriminants/
│   │       ├── NormFormOneUnitary/
│   │       ├── NormOneCharacters/
│   │       ├── NormOneInverseMembership/
│   │       ├── NormOnePowerPrincipal/
│   │       ├── NormRepresentationChange/
│   │       ├── NormRepresentationLift/
│   │       ├── NormTransitivityGroup/
│   │       ├── OddDualWeylJacobian/
│   │       ├── OrbitJetDegreeBound/
│   │       ├── OrbitJetLogarithm/
│   │       ├── OrbitJetRestriction/
│   │       ├── OrbitPowerSeriesCoefficients/
│   │       ├── OrbitQuotientTopology/
│   │       ├── OrbitRestrictionDegreeOne/
│   │       ├── OrbitSumCount/
│   │       ├── OrbitValuationBounds/
│   │       ├── OrthogonalFamilyExistence/
│   │       ├── PairCorankPositivity/
│   │       ├── PairCountNoncommuting/
│   │       ├── ParahoricIndexCount/
│   │       ├── PartialDerivativeMinors/
│   │       ├── PeriodPairIndependence/
│   │       ├── PhiBigCellForm/
│   │       ├── PhiDerivative/
│   │       ├── PoincareSeriesMeasurability/
│   │       ├── PoleLengthBound/
│   │       ├── PolydiscIntegrality/
│   │       ├── PolynomialDifferentialWords/
│   │       ├── PolynomialModelIsometry/
│   │       ├── PolynomialProperness/
│   │       ├── PositiveDefiniteness/
│   │       ├── PowerBoundedIntegrality/
│   │       ├── PowerSeriesNormUnits/
│   │       ├── PowerSpans/
│   │       ├── PrimeLogarithmTail/
│   │       ├── ProductFormulaHaar/
│   │       ├── projection2/
│   │       ├── ProjectionGramMatrices/
│   │       ├── ProjectionLattices/
│   │       ├── ProjectionRows/
│   │       ├── QuadraticDedekindZeta/
│   │       ├── QuadraticDifference/
│   │       ├── QuadraticFormLevel/
│   │       ├── QuadraticFormTwoTwo/
│   │       ├── QuadraticInvariants/
│   │       ├── QuantumDeterminantCommute/
│   │       ├── QuantumMinorLemma/
│   │       ├── QuarticIndependence/
│   │       ├── QuasiRegularSequence/
│   │       ├── QuotientIntegralBound/
│   │       ├── QuotientInvariantMeasurability/
│   │       ├── QuotientMeasureUniqueness/
│   │       ├── QuotientSigmaFiniteness/
│   │       ├── RamificationBound/
│   │       ├── RamificationRankSum/
│   │       ├── RankTwoDimensionFormula/
│   │       ├── RationalKernels/
│   │       ├── RationalPointsComparison/
│   │       ├── RationalRealBlocks/
│   │       ├── RealFieldComparison/
│   │       ├── RealInducedCharacters/
│   │       ├── RegularLocalRegularSequence/
│   │       ├── RelativeEquivalence/
│   │       ├── RelevantCarrierNonempty/
│   │       ├── RepresentationIndependence/
│   │       ├── ResidueLatticeCount/
│   │       ├── RightSingleRule/
│   │       ├── RootsOfUnityModPrime/
│   │       ├── RootSubgroupBasics/
│   │       ├── RootSubgroupHaar/
│   │       ├── RootSubgroupJacobian/
│   │       ├── RowDerivationChainRule/
│   │       ├── RowExpansionMinor/
│   │       ├── RowFormPermutationSplit/
│   │       ├── RowWeightSpan/
│   │       ├── SandwichChart/
│   │       ├── ScalarConvolutionTrace/
│   │       ├── ScalarDegree/
│   │       ├── ScalarEquivalenceGeneral/
│   │       ├── ScalarEquivalenceGenerators/
│   │       ├── ScalarPairOrthogonal/
│   │       ├── ScalarRelationReflexive/
│   │       ├── SchurConvolution/
│   │       ├── SchurOrthogonality/
│   │       ├── SchurUnitaryInner/
│   │       ├── SelfDualContinuity/
│   │       ├── SelfDualDifferent/
│   │       ├── SelfDualLocalBasis/
│   │       ├── SemidirectVolume/
│   │       ├── SemilocalBasis/
│   │       ├── SemisimpleTraceForm/
│   │       ├── SesquilinearRowSplitting/
│   │       ├── SiegelWeilVolume/
│   │       ├── SizeAbsorption/
│   │       ├── SizeCount/
│   │       ├── SkewAnalyticGroup/
│   │       ├── SkipSuccessorIndex/
│   │       ├── SmallArtinSchreier/
│   │       ├── SmithNormalForm/
│   │       ├── SmoothTranslationMeasure/
│   │       ├── SpectralGapLarge/
│   │       ├── SplitDensity/
│   │       ├── SplitPrimeIntegers/
│   │       ├── SplitZeroClosedness/
│   │       ├── SquarefreeDivisorDegree/
│   │       ├── SquarefreePrimeFactor/
│   │       ├── SquarefreeRootShift/
│   │       ├── SquarefreeRootsInjective/
│   │       ├── SquarePairGluing/
│   │       ├── SquarePairLocal/
│   │       ├── StabilizerFlagSplitting/
│   │       ├── StabilizerOrbitVolume/
│   │       ├── StabilizerPairs/
│   │       ├── StabilizerVolume/
│   │       ├── StandardCharacterTrace/
│   │       ├── StandardSlopeBound/
│   │       ├── StrongApproximation/
│   │       ├── SupportDatum/
│   │       ├── SymmetricDistance/
│   │       ├── TameSurjectivity/
│   │       ├── TaylorInversePower/
│   │       ├── TensorFrameConstruction/
│   │       ├── TensorOperator/
│   │       ├── TensorSpanning/
│   │       ├── TermAttractorConstant/
│   │       ├── TermCarrierStability/
│   │       ├── TermsFiniteAtPoint/
│   │       ├── ThetaExistence/
│   │       ├── ThetaSeriesExistence/
│   │       ├── ThetaSeriesUniqueness/
│   │       ├── TiltedDivisibility/
│   │       ├── TorsionFreeGenerators/
│   │       ├── TorusConjugationRule/
│   │       ├── TorusInvariance/
│   │       ├── TraceDualLocal/
│   │       ├── TraceFormEquality/
│   │       ├── TransferIndices/
│   │       ├── TranslationInvariantLattice/
│   │       ├── TwistedCharacterOne/
│   │       ├── TwistedEisensteinCoset/
│   │       ├── TwistedNormLattice/
│   │       ├── UnfoldingEquivalence/
│   │       ├── UnfoldingIdentity/
│   │       ├── UnimodularGenus/
│   │       ├── UnimodularIndex/
│   │       ├── UnimodularLocalStandard/
│   │       ├── UnimodularOrthogonal/
│   │       ├── UnipotentApproximation/
│   │       ├── UnipotentCardinality/
│   │       ├── UnipotentCocompact/
│   │       ├── UnipotentComposition/
│   │       ├── UnipotentCorrectionU1/
│   │       ├── UnipotentCost/
│   │       ├── UnipotentValuation/
│   │       ├── UnitaryApproximation/
│   │       ├── UnitaryClassFiniteness/
│   │       ├── UnitaryClassMass/
│   │       ├── UnitaryConjugation/
│   │       ├── UnitaryDensity/
│   │       ├── UnitaryQuotientCompactness/
│   │       ├── UnitarySecondCountable/
│   │       ├── UnitDeterminantRoot/
│   │       ├── UnitKronecker/
│   │       ├── UnitNormRoot/
│   │       ├── UnitPowerNormScale/
│   │       ├── UnramifiedSameDiagonal/
│   │       ├── VacuumEntire/
│   │       ├── ValuationGluing/
│   │       ├── ValuationLocalVolumes/
│   │       ├── WeakApproximationDVR/
│   │       ├── WeierstrassUniformization/
│   │       ├── WeightDualExistence/
│   │       ├── WeightDualUniqueness/
│   │       ├── WeightedLimitGauge/
│   │       ├── WeightedMeasureSplitting/
│   │       ├── WeilLatticeAction/
│   │       ├── WeilQuotientHaar/
│   │       ├── WeilQuotientMeasure/
│   │       ├── WeilStabilizerVolume/
│   │       ├── WeylCellRange/
│   │       ├── WeylConjugationFixedColumn/
│   │       ├── WeylFormulaCompact/
│   │       ├── WeylFormulaUnitary/
│   │       ├── WeylProduct/
│   │       ├── WhittakerFunctionalDual/
│   │       ├── WittCoefficients/
│   │       ├── WittDecomposition/
│   │       ├── WittEndomorphism/
│   │       ├── WittLogarithm/
│   │       ├── WittSubstitution/
│   │       ├── WittUnramified/
│   │       ├── WordInduction/
│   │       ├── ZeroLevelGeneralLinear/
│   │       ├── ZeroLevelIndex/
│   │       ├── ZeroWindow/
│   │       └── ZuckermanTensor/
│   ├── PieriBlockIdeals/
│   │   └── PieriColumnMinors/
│   ├── PolynomialDimension/
│   │   └── MultinomialDepth/
│   ├── PrimeAboveExistence/
│   ├── ProductFormula/
│   ├── QuotientMetricDivisors/
│   │   └── HermitianTwistDivisors/
│   ├── RankGapBounds/
│   │   └── RankGapProofs/
│   ├── RealPlaceAnalysis/
│   │   └── RealPlaceTaylor/
│   ├── ResultantValuation/
│   │   └── ResultantAdjugateProofs/
│   ├── SatakeDualWeyl/
│   │   └── AdelicIwasawaHecke/
│   ├── SelfDualUnimodular/
│   │   └── LocalLatticeDictionary/
│   ├── SharpRestriction/
│   │   ├── AbelianModels/
│   │   ├── AdmissibleParameterJoins/
│   │   ├── CuspSpanNormBounds/
│   │   │   ├── BruhatCellsKronecker/
│   │   │   ├── CayleyDegreeNondegeneracy/
│   │   │   ├── DiscreteSeriesExistence/
│   │   │   ├── FrobeniusCoefficientMemLp/
│   │   │   │   └── SigmaFiniteAmplitudes/
│   │   │   ├── NonemptyParameterModels/
│   │   │   └── UnimodularSchurMeasures/
│   │   ├── Divisibility/
│   │   │   ├── AbelianOpenPart/
│   │   │   ├── AdmissibleRank/
│   │   │   ├── ChainOperators/
│   │   │   ├── ClosedSizeLink/
│   │   │   ├── GeneratorPowers/
│   │   │   ├── HookProducts/
│   │   │   ├── JetPolynomialLogs/
│   │   │   ├── LocalNonemptiness/
│   │   │   ├── RankTruncation/
│   │   │   ├── SlopeExcess/
│   │   │   └── StatementFT/
│   │   ├── GenusPolyhedralBounds/
│   │   │   └── RelativeIndexClassSets/
│   │   ├── GlobalSchurBounds/
│   │   │   ├── GeneralLinearActions/
│   │   │   └── GlobalRankLatticeProofs/
│   │   │       └── UnitTraceSumBounds/
│   │   ├── GrowthBounds/
│   │   │   ├── AdmissibleIntegers/
│   │   │   ├── AevalValuation/
│   │   │   ├── BaseLevels/
│   │   │   ├── BinomialPolynomialIdentities/
│   │   │   ├── BinomialRatio/
│   │   │   ├── ChartComparison/
│   │   │   ├── ChartedClasses/
│   │   │   ├── ChartRank/
│   │   │   ├── CoarseMultiplicity/
│   │   │   ├── ColumnSpanDensity/
│   │   │   │   └── QuadraticBasis/
│   │   │   ├── DiagonalSupport/
│   │   │   ├── DualFockLinear/
│   │   │   ├── ExponentialPartialDerivatives/
│   │   │   ├── FittingIdeal/
│   │   │   ├── FockGramWindow/
│   │   │   ├── FrobeniusPaths/
│   │   │   ├── HermitianTensor/
│   │   │   │   └── ShapeCovering/
│   │   │   ├── IntegralWeylLatticeSpan/
│   │   │   ├── LatticeMultiplicityLemmas/
│   │   │   │   └── LatticeMultiplicityCheck/
│   │   │   ├── LogarithmicSums/
│   │   │   ├── MonomialFactorials/
│   │   │   ├── MonomialOrderSegments/
│   │   │   ├── MonomialSupport/
│   │   │   ├── MultisetValuation/
│   │   │   ├── PathWeight/
│   │   │   ├── PlaneCoefficients/
│   │   │   ├── PolynomialLevels/
│   │   │   ├── RootWeights/
│   │   │   ├── ScaleEdges/
│   │   │   ├── SegmentDegree/
│   │   │   ├── StandardPolynomials/
│   │   │   ├── TensorLatticeBounds/
│   │   │   ├── TruncatedChains/
│   │   │   ├── TwistedLevelAgreement/
│   │   │   └── TwistedSubstitution/
│   │   │       └── TwistedMonomialFiltration/
│   │   ├── InertJacobiLevels/
│   │   ├── LevelLetterCocycles/
│   │   │   ├── CohomologyScalarsVanish/
│   │   │   ├── CyclotomicPowerSeries/
│   │   │   ├── DvrLatticeRank/
│   │   │   ├── JointConditionsZpowers/
│   │   │   ├── LevelKernelDetection/
│   │   │   ├── PrimesOverLiterature/
│   │   │   ├── QuotientImageDivisibility/
│   │   │   ├── RepresentationCongruences/
│   │   │   ├── SmallTwists/
│   │   │   └── StatementFamilies/
│   │   ├── RamificationFrobenius/
│   │   │   └── TotientGaloisClasses/
│   │   │       └── InertiaGaloisSymmetry/
│   │   ├── SmoothDesignExistence/
│   │   └── ValuationFrobeniusEpsilon/
│   │       ├── LeastPrimeTwists/
│   │       │   ├── PrimesOverExistence/
│   │       │   ├── QuotientShiftIrreducible/
│   │       │   │   └── NoetherianQuotientCalc/
│   │       │   └── StrictlyAntitoneWeights/
│   │       │       ├── AntitoneWeightsLemma/
│   │       │       └── HatTripleRepresentations/
│   │       └── ScaledValuations/
│   ├── SizeWindowBrackets/
│   │   └── ChainSlopeWindows/
│   ├── SmithDeterminants/
│   │   └── DivisibilityChains/
│   ├── SobolevGaussianKernels/
│   │   └── GaussianKernelBounds/
│   ├── SubspaceCounting/
│   │   └── SubspaceCountingProofs/
│   ├── SuccessiveMinima/
│   │   └── SuccessiveMinimaProofs/
│   ├── TameInertiaTowers/
│   │   └── CentralOrderTwo/
│   ├── ThetaLiftIndependence/
│   │   └── ThetaOrbitSums/
│   ├── ThetaLogCoordinates/
│   │   ├── BihomogeneousPairs/
│   │   │   └── LetterChainEmbeddings/
│   │   ├── DualWeylCoordinates/
│   │   │   └── DualWeylProofs/
│   │   ├── FockResolutionOnto/
│   │   │   └── FockMonomialProofs/
│   │   ├── JacobiPathWeights/
│   │   │   └── JacobiMinorProofs/
│   │   ├── PartnerDischarge/
│   │   │   └── PartnerDischargeProofs/
│   │   ├── PartnerMeanCoordinates/
│   │   │   └── PartnerMeanProofs/
│   │   ├── ProductIdealMonotone/
│   │   │   └── ProductIdealProofs/
│   │   ├── ResidueClassEstimates/
│   │   │   └── VandermondeRankEstimates/
│   │   ├── SandwichModelDomains/
│   │   │   └── SandwichModelProofs/
│   │   ├── TraceIsometryWeights/
│   │   │   └── SchurTraceProofs/
│   │   └── UniformThetaSubstitution/
│   │       └── FrobeniusLiftNorms/
│   ├── ThetaSupremumBounds/
│   │   └── GaussianShiftBounds/
│   ├── ThickAverageLoss/
│   │   └── ThickAverageProofs/
│   ├── TorsionNormIteration/
│   │   └── InverseIntegralClasses/
│   ├── TowerValuationBounds/
│   │   └── TowerValuationProofs/
│   ├── TranslateCocycles/
│   │   └── TranslateCocycleProofs/
│   ├── TruncatedSeriesCounting/
│   │   └── TruncatedSeriesProofs/
│   ├── TwistFamilyExistence/
│   ├── UnipotentAdelicQuotients/
│   │   └── EllipticRegularity/
│   ├── WachLatticeTwists/
│   │   ├── CharacterSplitJumps/
│   │   │   └── CharacterJumpProofs/
│   │   ├── CoprimeLiftBounds/
│   │   │   └── CoprimeLiftProofs/
│   │   ├── CupProductVanishing/
│   │   │   └── CupProductProofs/
│   │   ├── DenseTopActions/
│   │   │   └── DenseTopActionProofs/
│   │   ├── HerrComplexInjectivity/
│   │   │   └── HerrComplexProofs/
│   │   ├── HodgeTateChains/
│   │   │   └── HodgeTateFiltrations/
│   │   ├── LagrangeExtensionCocycles/
│   │   │   └── ExtensionCocycleProofs/
│   │   ├── LatticeDualFibres/
│   │   │   └── LatticeDualProofs/
│   │   ├── RamifiedBlockRings/
│   │   │   └── RamifiedBlockProofs/
│   │   ├── RealClassMaps/
│   │   │   └── RealClassMapProofs/
│   │   ├── RealDisplaySplitting/
│   │   │   └── RealDisplayProofs/
│   │   ├── SandwichH1Classes/
│   │   │   └── SandwichH1Proofs/
│   │   ├── ShapeRowIsomorphisms/
│   │   │   └── ShapeRowProofs/
│   │   ├── SplitClassesAll/
│   │   │   └── SplitClassesProofs/
│   │   ├── SplitLocalLifts/
│   │   │   └── SplitLocalLiftProofs/
│   │   ├── TorsionKernelSplitting/
│   │   │   └── TorsionKernelProofs/
│   │   ├── TorsionLengthCounts/
│   │   └── WachProductBases/
│   │       └── WachProductProofs/
│   ├── WachModuleLifts/
│   │   └── WachModuleProofs/
│   ├── WeaklyAdmissibleFiltrations/
│   │   └── CrystallineStableLifts/
│   ├── WeightedDeltaMeans/
│   ├── WideWeightTheorem/
│   ├── WindowSums/
│   │   └── AnnihilatorPolynomials/
│   ├── YangianSpanCharacter/
│   │   └── YangianRTTProofs/
│   ├── ZeroFreeRegion/
│   │   └── ZetaLogDerivativeBounds/
│   └── ZetaNonvanishing/
├── GroundTheory/
│   ├── ArithmeticGeometry/
│   │   ├── AbelianVarieties/
│   │   │   └── JacobianSmoothness/
│   │   ├── EtaleCompletion/
│   │   ├── IwasawaModules/
│   │   ├── ModularCurves/
│   │   ├── SchemeCohomology/
│   │   │   ├── CechNaturality/
│   │   │   ├── ProjectiveCohomology/
│   │   │   └── ProperCohomology/
│   │   ├── SelmerPairing/
│   │   └── ToricVarieties/
│   ├── AutomorphicForms/
│   │   ├── AdelicUnitaryGroups/
│   │   ├── ArchimedeanWhittaker/
│   │   │   └── ComplexWhittaker/
│   │   ├── AutomorphicFormSpaces/
│   │   ├── ContragredientTranspose/
│   │   ├── CuspidalDiscreteness/
│   │   ├── CuspidalProjection/
│   │   ├── DefiniteClassNumber/
│   │   ├── FourierWhittaker/
│   │   ├── GKModules/
│   │   ├── GL2/
│   │   ├── GL2Classical/
│   │   ├── HarishChandraCentre/
│   │   ├── HarishChandraInvariance/
│   │   ├── HarishChandraRegularity/
│   │   ├── L2LocalComponents/
│   │   ├── MultiplicityOne/
│   │   │   ├── GL2BumpFunctions/
│   │   │   └── GL2ProductCompleteness/
│   │   ├── PartialDifferential/
│   │   ├── TensorProductTheorem/
│   │   ├── UnitaryAdmissible/
│   │   └── UnitaryRepresentations/
│   ├── Brauer/
│   ├── FunctionField/
│   ├── GlobalFields/
│   │   ├── Adele/
│   │   │   └── BaseChange/
│   │   ├── AnalyticClassNumber/
│   │   ├── Artin/
│   │   ├── ClassFieldConsequences/
│   │   ├── CompletionAtPlace/
│   │   ├── ComplexMultiplication/
│   │   ├── CyclotomicCharacters/
│   │   ├── ExistenceTheorem/
│   │   ├── FirstInequality/
│   │   ├── GlobalArtinMap/
│   │   ├── GlobalReciprocity/
│   │   ├── HerbrandQuotients/
│   │   ├── IdeleClassGroup/
│   │   ├── IdeleGroups/
│   │   │   ├── GaloisOnAdeles/
│   │   │   ├── IdeleNorms/
│   │   │   ├── SIdeleGroups/
│   │   │   └── SIdeleHerbrand/
│   │   ├── InfiniteNormIndex/
│   │   ├── KummerTheory/
│   │   │   └── KummerIndexLemma/
│   │   ├── NormResidueSymbol/
│   │   ├── PowerSubgroupIndex/
│   │   ├── SecondInequality/
│   │   ├── SemilocalAlgebras/
│   │   ├── SplittingFromInequality/
│   │   ├── TateThesis/
│   │   └── WeilGroups/
│   ├── HeightsAndTheta/
│   │   ├── Heights/
│   │   │   ├── AnalyticLimit/
│   │   │   ├── Antisymmetric/
│   │   │   ├── ArithmeticBezout/
│   │   │   ├── ChowForms/
│   │   │   ├── ChowlaSelberg/
│   │   │   ├── ComplexAnalyticSets/
│   │   │   ├── ComplexMetrics/
│   │   │   ├── CountingLowerBound/
│   │   │   ├── DiscreteValuationNumbers/
│   │   │   ├── EffectiveHilbertSamuel/
│   │   │   ├── EisensteinTails/
│   │   │   ├── ElementarySymmetric/
│   │   │   ├── FactorialBounds/
│   │   │   ├── FieldsOfNumbers/
│   │   │   ├── FiniteCovolume/
│   │   │   ├── FlagBundles/
│   │   │   ├── FlatDegree/
│   │   │   ├── FubiniStudyInvariance/
│   │   │   ├── HeightComparison/
│   │   │   ├── HeightKernels/
│   │   │   ├── HeightsOfSets/
│   │   │   ├── HilbertSamuel/
│   │   │   │   ├── IrreducibleConnected/
│   │   │   │   └── SectionNormSquares/
│   │   │   ├── HodgeLowerBound/
│   │   │   │   ├── CoordinateIdeals/
│   │   │   │   ├── Counterexample/
│   │   │   │   ├── FlagIndices/
│   │   │   │   ├── FrameDefinitions/
│   │   │   │   ├── GramMatrices/
│   │   │   │   └── PlueckerCoordinates/
│   │   │   ├── HomogeneousLocalization/
│   │   │   ├── IntegralModels/
│   │   │   ├── Intersections/
│   │   │   ├── IterateExamples/
│   │   │   ├── KleimanAmpleness/
│   │   │   │   └── TwistFiniteness/
│   │   │   ├── LatticeLemmas/
│   │   │   ├── LocalDensities/
│   │   │   ├── LocalFiniteness/
│   │   │   ├── MatrixCharts/
│   │   │   ├── MonomialBases/
│   │   │   ├── MultinomialWeights/
│   │   │   ├── OrbitLimits/
│   │   │   ├── Proportionality/
│   │   │   ├── QuadraticFields/
│   │   │   ├── ReducedTensors/
│   │   │   ├── Regularisation/
│   │   │   ├── RemainderTerms/
│   │   │   ├── SemipositiveHeights/
│   │   │   ├── Slopes/
│   │   │   ├── StabilizerCovolume/
│   │   │   ├── StrongApproximation/
│   │   │   ├── ThetaKeyFormula/
│   │   │   ├── VerticalDivisors/
│   │   │   └── WeightedHomogeneous/
│   │   └── Theta/
│   │       ├── AlgebraicHecke/
│   │       ├── Capelli/
│   │       ├── EisensteinZeta/
│   │       │   ├── AdicFrames/
│   │       │   ├── DedekindZetaSeries/
│   │       │   ├── MirabolicInduction/
│   │       │   ├── UnitLevels/
│   │       │   └── WeilPolarization/
│   │       ├── FiniteGL/
│   │       ├── LieCoordinates/
│   │       ├── LocallyCompactField/
│   │       ├── SchroedingerTranslates/
│   │       ├── SplitLinear/
│   │       ├── Unimodular/
│   │       ├── UnitaryReduction/
│   │       └── Weil/
│   ├── IdeleRoots/
│   │   ├── ClassicalIdeles/
│   │   ├── ConstantFrames/
│   │   │   └── GaugeExistence/
│   │   └── TorusPowers/
│   ├── LocalFields/
│   │   ├── AbstractLocalReciprocity/
│   │   ├── FormalGroups/
│   │   ├── LubinTateReciprocity/
│   │   └── QuadraticAbelian/
│   ├── PAdicHodge/
│   ├── PowerSubgroups/
│   │   └── CountableNeighbourhoods/
│   ├── ProfiniteCohomology/
│   │   ├── ClassFormations/
│   │   ├── CohomologicalDimension/
│   │   ├── CohomologyFunctoriality/
│   │   ├── CoinducedModules/
│   │   ├── CompactSupportCohomology/
│   │   ├── ContinuousCochains/
│   │   ├── CupProducts/
│   │   ├── DiscreteModules/
│   │   ├── GaloisCohomology/
│   │   ├── GaloisModules/
│   │   ├── GlobalClassFormation/
│   │   │   ├── IdeleCohomology/
│   │   │   ├── IdeleInvariants/
│   │   │   ├── IdeleLimits/
│   │   │   ├── IdeleRestriction/
│   │   │   ├── LocalDegrees/
│   │   │   └── LocalLimits/
│   │   ├── GlobalEulerCharacteristic/
│   │   ├── InflationRestriction/
│   │   ├── LocalClassFormation/
│   │   │   └── FiniteVanishing/
│   │   ├── LocalEulerCharacteristic/
│   │   ├── LocalTateDuality/
│   │   ├── MackeyFormula/
│   │   ├── PoincareDuality/
│   │   ├── PoincarePairs/
│   │   ├── PoitouTate/
│   │   │   └── PoitouTateInfinite/
│   │   ├── RealPlaces/
│   │   └── RestrictedRamification/
│   └── TateCohomology/
├── Lemmata/
│   ├── AddValuationProducts/
│   ├── B110/
│   ├── B1959r/
│   ├── B1962s/
│   ├── Cancellation/
│   ├── CharacterDirections/
│   ├── ClearingDenominators/
│   ├── CofiniteContinuousBounds/
│   ├── ComplementLifts/
│   ├── CurryModusPonens/
│   ├── Denominators/
│   ├── DetMonotoneStarMulSelf/
│   ├── DetNormLeProdRows/
│   ├── DiscreteValuationQuotients/
│   ├── DualWeylPullback/
│   ├── FiberEquations/
│   ├── FirstBlockLemmaA/
│   ├── FirstBlockLemmaB/
│   ├── FirstBlockLemmaC/
│   ├── FirstBlockLemmaD/
│   ├── FirstBlockLemmaE/
│   ├── FirstBlockLemmaF/
│   ├── FirstBlockLemmaG/
│   ├── FirstBlockLemmaH/
│   ├── FirstBlockLemmaI/
│   ├── FirstBlockLemmaJ/
│   ├── FirstBlockLemmaK/
│   ├── FirstBlockLemmaL/
│   ├── FunctionAtZero/
│   ├── GeneralBFact/
│   ├── GeneralBFactAltForm/
│   ├── GeneralBFactBis/
│   ├── GeneralBFactBisAlt/
│   ├── GeneralBFactBisForm/
│   ├── GeneralBFactExtra/
│   ├── GeneralBFactForm/
│   ├── GeneralBFactFurther/
│   ├── GeneralBFactLast/
│   ├── GeneralBFactLeft/
│   ├── GeneralBFactLeftAlt/
│   ├── GeneralBFactLeftAltForm/
│   ├── GeneralBFactLeftBis/
│   ├── GeneralBFactLeftBisAlt/
│   ├── GeneralBFactLeftBisForm/
│   ├── GeneralBFactLeftExtra/
│   ├── GeneralBFactLeftForm/
│   ├── GeneralBFactLeftFurther/
│   ├── GeneralBFactLeftLast/
│   ├── GeneralBFactLeftMore/
│   ├── GeneralBFactLeftRest/
│   ├── GeneralBFactLeftSide/
│   ├── GeneralBFactLeftTail/
│   ├── GeneralBFactLeftTer/
│   ├── GeneralBFactLeftTerForm/
│   ├── GeneralBFactLeftVariant/
│   ├── GeneralBFactLeftVersion/
│   ├── GeneralBFactMore/
│   ├── GeneralBFactRest/
│   ├── GeneralBFactRight/
│   ├── GeneralBFactRightAlt/
│   ├── GeneralBFactRightAltForm/
│   ├── GeneralBFactRightBis/
│   ├── GeneralBFactRightBisAlt/
│   ├── GeneralBFactRightBisForm/
│   ├── GeneralBFactRightExtra/
│   ├── GeneralBFactRightForm/
│   ├── GeneralBFactRightFurther/
│   ├── GeneralBFactRightLast/
│   ├── GeneralBFactRightMore/
│   ├── GeneralBFactRightRest/
│   ├── GeneralBFactRightSide/
│   ├── GeneralBFactRightTer/
│   ├── GeneralBFactRightTerForm/
│   ├── GeneralBFactRightVariant/
│   ├── GeneralBFactRightVersion/
│   ├── GeneralBFactSecond/
│   ├── GeneralBFactSecondAlt/
│   ├── GeneralBFactSecondAltForm/
│   ├── GeneralBFactSecondBis/
│   ├── GeneralBFactSecondBisAlt/
│   ├── GeneralBFactSecondBisForm/
│   ├── GeneralBFactSecondExtra/
│   ├── GeneralBFactSecondForm/
│   ├── GeneralBFactSecondFurther/
│   ├── GeneralBFactSecondLast/
│   ├── GeneralBFactSecondMore/
│   ├── GeneralBFactSecondRest/
│   ├── GeneralBFactSecondSide/
│   ├── GeneralBFactSecondTail/
│   ├── GeneralBFactSecondTer/
│   ├── GeneralBFactSecondTerForm/
│   ├── GeneralBFactSecondVariant/
│   ├── GeneralBFactSecondVersion/
│   ├── GeneralBFactSide/
│   ├── GeneralBFactTail/
│   ├── GeneralBFactTer/
│   ├── GeneralBFactTerForm/
│   ├── GeneralBFactThird/
│   ├── GeneralBFactThirdAlt/
│   ├── GeneralBFactThirdAltForm/
│   ├── GeneralBFactThirdBis/
│   ├── GeneralBFactThirdBisAlt/
│   ├── GeneralBFactThirdBisForm/
│   ├── GeneralBFactThirdExtra/
│   ├── GeneralBFactThirdForm/
│   ├── GeneralBFactThirdFurther/
│   ├── GeneralBFactThirdLast/
│   ├── GeneralBFactThirdMore/
│   ├── GeneralBFactThirdRest/
│   ├── GeneralBFactThirdSide/
│   ├── GeneralBFactThirdTail/
│   ├── GeneralBFactThirdTer/
│   ├── GeneralBFactThirdTerForm/
│   ├── GeneralBFactThirdVariant/
│   ├── GeneralBFactThirdVersion/
│   ├── GeneralBFactUpper/
│   ├── GeneralBFactUpperAltForm/
│   ├── GeneralBFactUpperBis/
│   ├── GeneralBFactUpperForm/
│   ├── GeneralBFactUpperTerForm/
│   ├── GeneralBFactUpperVariant/
│   ├── GeneralBFactUpperVersion/
│   ├── GeneralBFactVariant/
│   ├── GeneralBFactVersion/
│   ├── HermitianSesquilinear/
│   ├── HermitianVanishing/
│   ├── IdempotentTraceVanishing/
│   ├── IntegerMulIntegral/
│   ├── IterateZero/
│   ├── MiscLemmasA/
│   ├── MiscLemmasB/
│   ├── MiscLemmasC/
│   ├── MiscLemmasD/
│   ├── MiscLemmasE/
│   ├── MiscLemmasF/
│   ├── MiscLemmasH/
│   ├── MiscLemmasI/
│   ├── MiscLemmasJ/
│   ├── MiscLemmasK/
│   ├── MiscLemmasL/
│   ├── MiscLemmasM/
│   ├── MiscLemmasN/
│   ├── MiscLemmasO/
│   ├── MiscLemmasP/
│   ├── MiscLemmasQ/
│   ├── MiscLemmasR/
│   ├── MovedPointExistence/
│   ├── MultivariateIntegrals/
│   ├── NatMulIsIntegral/
│   ├── NearbyExistence/
│   ├── PaddedFamilies/
│   ├── PadicNatCastNorm/
│   ├── PartialDerivativeDegree/
│   ├── PeriodicFunctions/
│   ├── PlaneOverMembership/
│   ├── PosDefOfRealQuadratic/
│   ├── PowerApplication/
│   ├── PowerMembership/
│   ├── PowMulVecEigen/
│   ├── PowMulVecEigenvalue/
│   ├── ProductIdentities/
│   ├── RankOneOrbitForms/
│   ├── ScalarExtension/
│   ├── SecondBlockLemmaA/
│   ├── SimultaneousEigenvectors/
│   ├── SmulListSum/
│   └── TwistedIdempotents/
├── PositivityTheory/
│   ├── AutomorphicForms/
│   │   └── PublishedInputs/
│   │       ├── BorelInjectivity/
│   │       │   └── EquivariantProjections/
│   │       ├── CuspidalContinuity/
│   │       │   └── ArchimedeanCuspidal/
│   │       │       ├── AdelicGaussians/
│   │       │       ├── CyclicCharacterEigen/
│   │       │       ├── EulerProducts/
│   │       │       ├── GaugeTopology/
│   │       │       ├── KFiniteVectors/
│   │       │       │   ├── KFiniteAdelicGaussians/
│   │       │       │   ├── KFiniteGlobalStability/
│   │       │       │   ├── KFiniteThetaLifts/
│   │       │       │   │   └── PureThetaTransfer/
│   │       │       │   ├── LocallyConstantMajorants/
│   │       │       │   │   ├── GammaSplitting/
│   │       │       │   │   ├── SmoothMajorants/
│   │       │       │   │   └── TemperedDerivatives/
│   │       │       │   └── LocalWhittakerDuality/
│   │       │       │       └── WhittakerRealPlaces/
│   │       │       ├── MellinTransforms/
│   │       │       ├── RealLocalIntegrals/
│   │       │       │   ├── RealGammaLimits/
│   │       │       │   ├── RealSharpBounds/
│   │       │       │   └── RealTemperedBounds/
│   │       │       ├── SquareIntegrable/
│   │       │       ├── StripEstimates/
│   │       │       ├── SummableUnitBounds/
│   │       │       └── VerticalStrips/
│   │       ├── CyclicBaseChange/
│   │       ├── CyclicBaseChangeLifts/
│   │       ├── HilbertEisenstein/
│   │       ├── JacquetLanglands/
│   │       │   ├── RealArchimedeanBounds/
│   │       │   └── TorusKernels/
│   │       ├── NonzeroTypes/
│   │       └── RealGaloisRepresentations/
│   │           └── IwahoriSphericalTransfer/
│   ├── PublishedTheorems/
│   │   ├── TowerLemmas/
│   │   │   └── FormalTowerLemmas/
│   │   ├── UnitKilling/
│   │   │   └── UnitAnnihilation/
│   │   │       └── UnitAnnihilators/
│   │   └── WeilRepresentations/
│   │       └── ZariskiDensity/
│   └── Representations/
│       └── BoundaryCones/
│           └── ArchimedeanCones/
│               └── ConeOverlaps/
│                   └── OpenConeCriteria/
│                       └── OpenConeFormulation/
├── ReciprocityTheory/
│   ├── AdeleApproximation/
│   ├── AdicCompleteness/
│   ├── AnalyticForms/
│   │   ├── AnalyticCharts/
│   │   ├── LeviForms/
│   │   ├── PlurisubharmonicFunctions/
│   │   ├── PotentialTheory/
│   │   └── RegularLocalRings/
│   ├── Automorphisms/
│   ├── BasicDefinitions/
│   ├── BurnsideSurjectivity/
│   ├── Chebotarev/
│   ├── ClassFieldTheory/
│   │   ├── GlobalClassField/
│   │   │   └── SUnitGalois/
│   │   ├── LocalClassField/
│   │   └── PadicCompatibleSequences/
│   ├── CommutativeAlgebra/
│   │   ├── CohenMacaulay/
│   │   ├── MaximalIdealSquares/
│   │   ├── PolynomialHeights/
│   │   ├── PowerSeriesPresentations/
│   │   ├── SaturatedChains/
│   │   └── WeakRegularity/
│   ├── DualLattices/
│   ├── EigenFrames/
│   ├── GaloisValuations/
│   ├── GeneralLinearIntegers/
│   ├── GeometryOfNumbers/
│   │   ├── AsymptoticSequences/
│   │   ├── LatticeCovolumes/
│   │   ├── MatrixArithmetic/
│   │   ├── PluriharmonicAnalysis/
│   │   └── SphericalMonomials/
│   ├── GroupCohomology/
│   ├── Hypotheses/
│   ├── L2DbarEstimates/
│   │   ├── BasicIdentity/
│   │   ├── ChartDerivatives/
│   │   ├── HormanderEstimate/
│   │   ├── LeviForms/
│   │   ├── Localization/
│   │   ├── MinimalSolutions/
│   │   ├── Mollifiers/
│   │   ├── NormFibrations/
│   │   ├── PlurisubharmonicCharts/
│   │   ├── SkodaWeights/
│   │   ├── SymmetricSections/
│   │   └── WeakHolomorphy/
│   ├── NeutralLocalFields/
│   │   └── LocalFieldComparison/
│   │       └── LocalFieldAutomorphisms/
│   ├── ReducedBases/
│   ├── ReductiveGroups/
│   │   ├── ArithmeticGeometry/
│   │   │   ├── AdeleApproximation/
│   │   │   ├── ArakelovGeometry/
│   │   │   │   └── KleimanNefness/
│   │   │   ├── ArakelovVolumes/
│   │   │   │   ├── ArakelovInstances/
│   │   │   │   ├── IntegralModuleBases/
│   │   │   │   └── UpperBounds/
│   │   │   ├── ArithmeticIntersection/
│   │   │   │   ├── DiagonalDivisors/
│   │   │   │   ├── MixedFieldContraction/
│   │   │   │   ├── MultihomogeneousIdeals/
│   │   │   │   └── RationalSections/
│   │   │   ├── BirationalGeometry/
│   │   │   │   ├── BlowupProjections/
│   │   │   │   └── ToroidalCompactification/
│   │   │   ├── DiscreteValuationRings/
│   │   │   ├── ExtensionDescent/
│   │   │   │   └── ChartPullbacks/
│   │   │   │       ├── BaseChangeKernels/
│   │   │   │       ├── CubePullbacks/
│   │   │   │       ├── GeneratorPullback/
│   │   │   │       ├── LinearRestriction/
│   │   │   │       ├── TangentLinearity/
│   │   │   │       ├── UniformBaseChange/
│   │   │   │       │   └── PullbackDegree/
│   │   │   │       ├── UniversalCharts/
│   │   │   │       └── WeightedChartPullback/
│   │   │   ├── FirstCohomology/
│   │   │   ├── FundamentalDomains/
│   │   │   │   └── FundamentalDomainExtension/
│   │   │   │       ├── NearSupremumBounds/
│   │   │   │       ├── PointAssembly/
│   │   │   │       └── UnipotentMoves/
│   │   │   ├── HeightTheory/
│   │   │   │   └── GaussHeights/
│   │   │   │       ├── GaussGenericHeight/
│   │   │   │       │   └── GaussGenericStatements/
│   │   │   │       │       ├── GaussGenericLemmas/
│   │   │   │       │       │   └── TranslationDomainMaps/
│   │   │   │       │       └── GaussGenericTheorem/
│   │   │   │       ├── GaussUniqueness/
│   │   │   │       │   └── GaussUniquenessStatements/
│   │   │   │       │       ├── GaussUniquenessLemmas/
│   │   │   │       │       │   └── KernelLineArguments/
│   │   │   │       │       └── GaussUniquenessTheorem/
│   │   │   │       ├── GenericPointHeight/
│   │   │   │       │   └── GenericPointStatements/
│   │   │   │       │       ├── GenericPointLemmas/
│   │   │   │       │       │   └── GenericPointWeights/
│   │   │   │       │       └── GenericPointTheorem/
│   │   │   │       └── PlaceSumHeights/
│   │   │   │           └── PlaceSumStatements/
│   │   │   │               ├── PlaceSumLemmas/
│   │   │   │               │   └── GaussValuationSums/
│   │   │   │               └── PlaceSumTheorem/
│   │   │   ├── PlaceDivisors/
│   │   │   │   ├── ChartPointCongruence/
│   │   │   │   ├── FiniteLocalLifts/
│   │   │   │   ├── LinearFormDegree/
│   │   │   │   ├── SiegelPullbackTransfer/
│   │   │   │   └── TopLimitModules/
│   │   │   ├── PullbackSections/
│   │   │   │   └── HolomorphicFamilies/
│   │   │   ├── Rationality/
│   │   │   ├── SemiabelianSchemes/
│   │   │   │   ├── AbelianSchemeQuotients/
│   │   │   │   ├── Biextensions/
│   │   │   │   ├── CubicalStructures/
│   │   │   │   ├── GenericFiberGluing/
│   │   │   │   ├── PrecompleteBases/
│   │   │   │   └── SplitTori/
│   │   │   ├── SquareIntegrability/
│   │   │   │   ├── FourierProjections/
│   │   │   │   └── TiledBoundaries/
│   │   │   ├── StrongApproximation/
│   │   │   ├── SymplecticGenerators/
│   │   │   │   └── SymplecticCharacters/
│   │   │   ├── TaylorDiscriminants/
│   │   │   │   ├── DiscriminantEstimates/
│   │   │   │   │   ├── DiscriminantLemmas/
│   │   │   │   │   │   ├── DividedPowerIntegrals/
│   │   │   │   │   │   ├── IdempotentEvaluation/
│   │   │   │   │   │   ├── PerpendicularDeterminants/
│   │   │   │   │   │   ├── SchwarzBallNumerics/
│   │   │   │   │   │   ├── UniformDiscreteness/
│   │   │   │   │   │   └── WickFormula/
│   │   │   │   │   └── DiscriminantTheorems/
│   │   │   │   └── WickVanishing/
│   │   │   ├── ValuationLifting/
│   │   │   │   └── ValuationApproximation/
│   │   │   └── WeightedSumBounds/
│   │   ├── DiscreteSeries/
│   │   │   ├── AnalyticVectors/
│   │   │   ├── BochnerInequality/
│   │   │   ├── CasimirAlgebra/
│   │   │   ├── CasimirCoefficients/
│   │   │   ├── DiscreteSeriesExistence/
│   │   │   ├── ExceptionalGroupG2/
│   │   │   │   ├── BochnerG2/
│   │   │   │   ├── ExistenceG2/
│   │   │   │   ├── FormalDegreeG2/
│   │   │   │   ├── RigidityG2/
│   │   │   │   └── TensorProductsG2/
│   │   │   ├── FormalDegree/
│   │   │   │   └── HaarVolumes/
│   │   │   ├── HighestWeights/
│   │   │   │   ├── ContinuousRepresentations/
│   │   │   │   ├── PieriRules/
│   │   │   │   └── PRVComponents/
│   │   │   ├── InfinitesimalDecay/
│   │   │   ├── LaplaceOperators/
│   │   │   │   ├── BesselVectors/
│   │   │   │   ├── CapelliIdentity/
│   │   │   │   ├── DifferentialAction/
│   │   │   │   │   └── DifferentialActionLemma/
│   │   │   │   ├── InterlacingWalks/
│   │   │   │   ├── KTypeLemma/
│   │   │   │   ├── LaplaceEstimates/
│   │   │   │   │   └── SmoothMatrixMaps/
│   │   │   │   ├── LaplaceFoundations/
│   │   │   │   │   └── OneParameterSubgroups/
│   │   │   │   ├── ReproducingKernels/
│   │   │   │   └── SpectralGap/
│   │   │   ├── MultiplicityOne/
│   │   │   │   ├── HermitianMeasures/
│   │   │   │   └── MultiplicityDescent/
│   │   │   ├── RigidityTheorems/
│   │   │   ├── TailIntegrals/
│   │   │   ├── TensorRepresentations/
│   │   │   └── TraceGap/
│   │   ├── ExtensionEmbeddings/
│   │   ├── LatticeEmbeddings/
│   │   ├── Lattices/
│   │   ├── LocalHeights/
│   │   ├── Models/
│   │   │   └── FiniteGeneration/
│   │   │       └── FiniteGenerationProofs/
│   │   ├── PlaceCounting/
│   │   ├── SymplecticTraces/
│   │   │   └── WeylCharacters/
│   │   ├── TraceFormulas/
│   │   └── UnramifiedIntegrals/
│   ├── ResidueCardinality/
│   ├── SemistableReduction/
│   ├── ThetaQuasiPeriods/
│   └── ThetaSummability/
│       ├── RealCoinvariants/
│       └── TailSumEstimates/
└── Supplements/
    └── Kernels/
```

</details>

Every `.lean` chapter/module is present in its listed folder. For the main RH claim route, start at [`src/Main.lean`](src/Main.lean), follow `rhOfAll` to [`src/Supplements/Kernels/MainTheorems.lean`](src/Supplements/Kernels/MainTheorems.lean), then follow the `Formalism.VW.rh_of_every` and `allChi` imports through `src/Formalism/` and `src/Development/`. The 175,187 individual Lean files are not repeated as a flat list here; their directory placement is shown above.

## Lean version and dependencies

The included `lean-toolchain` requests Lean `v4.33.1`. `lakefile.toml` declares Mathlib and the library targets. Dependencies are not vendored in this repository.

The source has not been built or checked in this preparation. Treat it as untrusted downloaded source; review it before running Lean or Lake commands.

## Provenance and licensing

The files were downloaded from the archive parts linked above and assembled for this repository. The archive does not include a license file, so no reuse license is implied here. Refer to the original [remark PDF](https://alpo.ge/remark.pdf) for its accompanying claims and context.
