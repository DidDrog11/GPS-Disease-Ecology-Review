# Proposed Synthesis Projects: GPS and Disease Ecology

Background: Following the systematic review we recently completed in the addiction literature, there is a clear opportunity to apply a similar structural audit to our own field. Disease ecology increasingly pairs individual-level movement tracking (GPS, VHF) with pathogen/serological sampling. However, the methodological pipelines used to process this data wildly, and the ecological outcomes (e.g., does infection probability alter with increased mobility?) are heavily context-dependent.

I propose leveraging a single systematic literature search into two distinct projects.

## Project 1: Methodological and Analytic Choices in Disease Ecology

A systematic audit of study design, feature extraction, and reporting standards.

The Concept:
Before we can trust the biological signals linking movement to disease, we need to understand the noise. This project will systematically review studies that explicitly pair terrestrial animal movement tracking with individual- or group-level disease/pathogen sampling. We will extract exactly how the field collects, processes, and analyses this data.

Key Extraction Targets:

    Device & Sampling: Device type, fix frequency, battery life vs. tracking duration trade-offs.

    Missing Data Handling: How are missing fixes handled? (do authors account for the fact that a missing fix might be biologically informative—e.g., febrile lethargy, sheltering, or mortality—rather than just technical failure?)

    Movement Metrics: Which specific spatial features are extracted (e.g., home range estimators like KDE vs. LoCoH, roaming entropy, daily travel distance, contact network parameters)?

    Reporting Quality: Are authors reporting sample size justifications, device failure rates, and sensitivity analyses for spatial scaling?

Barriers & Limitations:

    Synthesising disparate methodologies into a cohesive narrative will be structurally difficult.

    The definition of terms like "contact," "interaction," or "activity space" will vary between papers. We will have to build a standard dictionary to group these features.

    While hopefully useful for the field it will be heavily descriptive.

## Project 2: Bayesian Meta-Analysis of Movement Metrics and Disease Status

A quantitative synthesis of the direction and magnitude of spatial-epidemiological associations.

The Concept:
Using the same literature identified in Project 1, we will extract the statistical associations between infection status and spatial mobility. Because a frequentist meta-analysis would force incomparable ecological systems into a single metric, we will use a Bayesian hierarchical framework (e.g., brms/Stan). This allows us to model the variance rather than ignoring it.

Key Extraction Targets:

    Effect Directions & Sizes: Does infection increase or decrease the specified movement metric?

    Statistical Outputs: Exact means, SDs, sample sizes, and raw test statistics (t, F, χ2, precise p-values) to calculate standardisable effect sizes (e.g., Hedges' g).

    Biological Covariates: Host taxonomy, pathogen functional guild (e.g., micro vs. macroparasite, transmission mode), and infection phase (acute vs. chronic) to use as population-level effects and priors.

Barriers & Limitations:

    Field ecology is not great at reporting the residual variance or marginal means required to calculate effect sizes. We might start with 150 papers in Project 1 and find that only 30 report enough raw statistical data to be included in Project 2.

    We cannot treat a behavioural change in a fox as statistically independent from a wolf. We will need to construct and incorporate a phylogenetic variance-covariance matrix into the Bayesian model.

    Null results are almost certainly underrepresented in the bio-logging literature. Our models will need to explicitly account for this bias.

Next Steps for the Group:
If we want to pursue this, the immediate next step is drafting the protocol, running the search and designing the data extraction sheet. We have to design the extraction sheet to capture the data for both projects simultaneously, so we only have to read these papers once.
