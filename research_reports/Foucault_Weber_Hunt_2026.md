# HRP Lab Research Briefing  
## Trident-G Research Notes: New Findings in Adaptive Cognition

# **The same error means different things in different environments: what adaptive learning reveals about agent–niche synergy**

### Standfirst

A new behavioural and computational study by Foucault, Weber and Hunt compares how people learn when environmental change occurs through abrupt change points versus continuous random walks. Participants adapted both their belief updating and uncertainty-sensitive actions to the stated dynamics of each environment. This briefing evaluates the evidence and asks whether the results provide support for the Trident-G proposal that adaptive intelligence depends partly on the quality of coupling between an agent’s internal models and the structure of its niche.

---

## Study reviewed

| | |
|---|---|
| **Authors** | Cedric Foucault, Lilian A. Weber and Laurence Hunt |
| **Title** | *Environmental dynamics shape human learning: change points versus random walks* |
| **Journal/status** | *eLife*, reviewed preprint, version 1 |
| **Year** | 2026 |
| **DOI** | 10.7554/eLife.110137.1 |
| **Study type** | Behavioural predictive-inference experiments with Bayesian modelling |
| **Sample** | 60 adults: 30 in each of two experiments |
| **Population** | English-speaking adults recruited through Prolific |
| **Primary methods** | Trial-wise prediction, uncertainty-sensitive action, apparent learning-rate analysis and ideal-observer modelling |
| **Open data/code** | Early-access code and data repository reported |
| **Preregistration** | Not reported in the reviewed preprint |

The article follows the critical research-briefing structure specified for the technical ResearchGate series. fileciteturn0file0 The study details and reviewer assessments below are drawn from the attached reviewed preprint. fileciteturn0file1

---

## 1. The scientific problem

Learning in a changing environment requires more than reacting strongly whenever an outcome is surprising. The learner must infer **why** the prediction failed.

A large error could indicate that the environment has shifted abruptly. Alternatively, it could be an unusually noisy observation within a continuously drifting process. These possibilities call for different responses. Under change-point dynamics, a sufficiently large error can justify rapidly discarding an old estimate. Under random-walk dynamics, continuous smaller adjustments may be more appropriate because the latent state is expected to move on every trial.

These two classes of environment have usually been studied in separate experimental traditions and with different computational models. It has therefore remained unclear whether observed differences reflect genuinely structure-sensitive learning or merely differences among tasks, modelling conventions and participant samples.

A second problem concerns the source of uncertainty. Learners must distinguish changes in a latent mean from changes in variance or stochasticity. Both can produce dispersed observations and large prediction errors, but they have different implications for prediction and action.

Foucault and colleagues addressed both problems using a common task and a unified family of Bayesian models.

---

## 2. What the researchers did

Participants completed a “capture-the-beams” prediction task. On each trial, they positioned a paddle around a circular ring to predict where the next beam would appear. They also selected either a narrow or wide paddle.

The narrow paddle offered a larger reward when successful but a greater risk of missing. The wide paddle offered lower reward but provided more coverage. Paddle position therefore indicated the participant’s current estimate of the latent mean, while paddle width provided an action-based report of estimated variance.

The task contained two independently changing latent properties:

- the average beam direction;
- the variance of beam locations.

In Experiment 1, the mean remained stable for periods and then changed abruptly at unpredictable change points. In Experiment 2, the mean moved gradually according to a random walk. Variance alternated probabilistically between low and high states in both experiments.

Participants were explicitly told whether the mean would change abruptly or gradually. They were not told the precise change frequency, variance values or future observations. Each participant completed 1,500 trials, providing dense within-person behavioural data.

The researchers compared human behaviour with models that crossed two assumptions:

1. change-point versus random-walk dynamics;
2. fixed versus inferred variance.

An apparent learning rate was calculated from the size of each paddle-location update relative to the preceding prediction error.

> **The decisive test was whether the same prediction error produced different updating patterns under the two environmental structures, and whether each pattern resembled the model matched to that environment.**

---

## 3. What they found

### Direct behavioural observations

Participants altered their learning behaviour according to the stated environmental dynamics.

In the change-point environment, large prediction errors produced sharply increased paddle-location updates. This is sensible when a large discrepancy suggests that the previous latent mean may no longer be relevant.

In the random-walk environment, updating was more evenly distributed across error magnitudes. Even modest errors were informative because the latent mean was expected to drift continually rather than remain fixed between occasional jumps.

Participants also adapted paddle width to environmental stochasticity. In the change-point experiment, they selected the wide paddle on approximately 49% of high-variance trials but only 18% of low-variance trials. A similar pattern occurred in the random-walk experiment.

Crucially, participants did not respond identically to changes in mean and variance. Mean change points produced a brief increase in wide-paddle use, consistent with temporary uncertainty about location. Variance increases produced a sustained switch towards the wide paddle. The estimated adjustment lasted approximately 9.6 observations following variance changes, compared with 2.3 observations following mean changes.

### Model-dependent results

Human apparent learning rates correlated more strongly with the model whose assumed dynamics matched the task.

All participants in the change-point experiment were better matched by the change-point model. In the random-walk experiment, only 10% were better matched by the change-point model, implying that the large majority were closer to the random-walk model.

The models also clarified an initially counterintuitive result. Higher stochasticity does not have one simple effect on average learning rate. Holding error magnitude constant, greater stochasticity makes each observation less informative and reduces updating. Yet greater stochasticity also produces more large errors, which can increase average updating—especially when those errors are interpreted as possible change points.

### Authors’ interpretation

The authors interpret these findings as evidence that people deploy an internal generative model appropriate to the environment and use that model to determine how prediction errors should alter beliefs and actions.

That interpretation is plausible because the critical behavioural signatures differed in the directions predicted by the matched models. It is nevertheless stronger than the direct observation. The study establishes structure-sensitive behaviour that resembles model predictions; it does not yet definitively identify the process by which each participant generated that behaviour.

---

## Figure 1. The study at a glance

 <img width="616" height="441" alt="image" src="https://github.com/user-attachments/assets/d54b7f78-1647-4621-8369-8f75c91d6126" />

  *Simplified reconstruction of the experimental logic and principal behavioural result in Foucault et al. (2026).*

---

## 4. Critical appraisal

### What is unusually strong?

The strongest feature is the use of a common task and modelling framework to compare two generative structures that have often been investigated separately. Most task parameters were held constant while mean dynamics differed, reducing the risk that qualitatively different results arose from unrelated task designs.

The simultaneous manipulation of mean and variance is also valuable. It allowed the researchers to ask whether participants could distinguish a change in the expected location from a change in observational reliability.

The study produced converging behavioural readouts. Paddle location, movement probability, update magnitude and paddle width all pointed towards environment-sensitive adaptation. The large number of trials per participant permitted detailed event-related analyses, including the different temporal responses to mean and variance changes.

Finally, the full task code and supporting data were made available for inspection and reuse.

### What remains uncertain?

The experiments used two independent groups rather than exposing the same participants to both structures. A within-person crossover would provide a stronger test of whether individuals switch models when environmental dynamics change.

Participants were explicitly informed about the relevant generative structure. The study therefore tests the ability to **apply** an instructed model, not the ability to discover whether the environment is governed by change points, random walks or some hybrid process.

The sample size was modest at the person level, despite the dense trial-level data. The models were not initially fitted directly to each participant, and model comparison relied substantially on their ability to reproduce aggregated behavioural signatures.

The study also remains a version-one reviewed preprint. The eLife assessment judged most conclusions to have solid support but considered some claims incompletely supported.

### The strongest alternative explanation

A serious alternative is that part of the apparent learning-rate pattern reflects the response mechanism rather than Bayesian belief updating itself.

Participants frequently left the paddle stationary when the required change was small. The models reproduced this through a response-probability mechanism resembling motor inertia or satisficing. Because no-movement trials have an apparent learning rate of zero, averaging them with active updates can alter the shape of the learning-rate curve.

A simpler learning rule combined with the same response mechanism might therefore reproduce part of the reported signature. The reviewers specifically requested comparisons with Rescorla–Wagner models, clearer separation of normative inference from response-level perseveration, individual model fitting and examination of hybrid strategies. The authors agreed to undertake these analyses.

### What the study does not show

It does not establish that people spontaneously infer environmental dynamics without instruction. It does not show that the mechanism transfers across task wrappers or real-world domains. It contains no neural or physiological measure of prediction error, precision or criticality. Nor does it directly measure general intelligence, Trident-G niche coupling or the near-critical Ψ-band.

**Evidence status:** strong within-task evidence for structure-sensitive learning; moderate support for the proposed Bayesian process; preliminary relevance to broader adaptive intelligence.

---

## 5. Predictive-processing interpretation

In predictive-processing terms, the study shows why prediction error should not be treated as a context-free teaching signal.

A prediction error acquires its meaning from a generative model. Under change-point assumptions, a large error raises the probability that the latent state has been replaced, making substantial updating appropriate. Under random-walk assumptions, error is interpreted within a process of continuing drift, favouring steadier integration.

Variance inference provides a second level of calibration. When variance is high, any one observation provides weaker evidence about the latent mean. Participants’ paddle-width choices and error-conditioned learning rates indicate that they were sensitive to this distinction.

The study therefore supports a central predictive-processing principle:

> **Adaptive learning depends not only on the magnitude of prediction error, but on the inferred cause, reliability and temporal structure of that error.**

However, this is behavioural and computational evidence. The study did not directly measure neural precision weighting, hierarchical prediction-error signals or the implementation of Bayesian inference in the brain.

---

## 6. Trident-G alignment: from environmental fit to niche synergy

Trident-G treats general adaptive intelligence as a property of the coupled brain–body–niche system rather than as an isolated capacity inside the individual. Its niche-coupling parameter, **λ**, describes the quality of the link between internal adaptive dynamics and environmental structure. When coupling is poor, internal search and updating may be coherent yet misaligned with the demands of the niche. When coupling is strong, environmental regularities shape prediction, inference and action in ways that preserve useful adaptation. fileciteturn0file2

Foucault and colleagues provide a clean task-level illustration of this idea. Participants did not merely generate accurate predictions. They adjusted the **form of learning itself** to fit the environment:

```text
environmental dynamics
→ appropriate generative assumptions
→ calibrated interpretation of error
→ uncertainty-sensitive action
→ improved environmental fit
```

The strongest Trident-G implication is that niche synergy should not be identified with raw performance alone. It involves at least four linked forms of alignment:

| Form of alignment | Expression in the study |
|---|---|
| **Structural alignment** | Change-point or random-walk assumptions match the environment |
| **Error-attribution alignment** | Surprise is attributed to mean change, gradual drift or stochasticity |
| **Precision alignment** | Evidence is weighted according to inferred variance |
| **Policy alignment** | Paddle location and width are adapted to expected outcomes and risk |

This suggests a possible behavioural operationalisation of λ at the local task level: not simply how accurately an agent predicts, but how well its model class, uncertainty estimates, updating policy and actions remain aligned with the environment’s generative organisation.

The findings also fit the G-loop principle that mismatch should produce different kinds of updating depending on what has changed. A large discrepancy need not reopen the entire system. It should propagate only when it indicates that the active relational map, context or policy is no longer appropriate.

There are nevertheless important boundaries. Participants were told which structural model applied, so environmental coupling was partly scaffolded through explicit instruction. The study did not test autonomous niche-model discovery, cross-context transfer, allostatic regulation or near-critical dynamics.

### Alignment classification

> **Convergent evidence with a useful extension.**

The study independently supports the Trident-G claim that adaptive cognition depends on model–environment coupling. It also suggests more precise behavioural components through which niche coupling might be measured. It is not direct support for the full theory because λ, Ψ-band occupancy and general adaptive intelligence were not measured.

---

## Evidence-to-theory map

```text
WHAT WAS OBSERVED
The same-sized errors produced different updates
in abrupt and gradual environments.
               ↓
WHAT THE AUTHORS INFER
Learners used environment-appropriate
generative models.
               ↓
PREDICTIVE-PROCESSING READING
Prediction error is weighted by beliefs about
latent dynamics and stochasticity.
               ↓
TRIDENT-G IMPLICATION
Adaptive intelligence depends partly on the fit
between internal models, action policies and
the structure of the niche.
```
---

## 7. Follow-up tests

### Test 1: Uninstructed structure discovery

Participants should encounter environments whose dynamics are initially undisclosed and occasionally switch between change-point and random-walk regimes.

A structure-learning account predicts that behaviour should gradually acquire the appropriate error-weighting signature and later switch when the regime changes. A purely instruction-driven strategy would not generalise.

### Test 2: Direct comparison with simpler and hybrid models

Bayesian, Rescorla–Wagner, satisficing and hybrid models should be fitted to individual trial sequences and evaluated out of sample.

The critical question is whether explicit inference over environmental structure explains behaviour beyond a simpler fixed learning rule plus perseveration.

### Test 3: Transfer of the inferred structure

After learning abrupt or gradual dynamics in the beam task, participants should encounter a changed sensory wrapper—or a conceptually different forecasting task—with the same latent dynamics.

If an abstract generative model has been learned, the appropriate update policy should recover more rapidly in the new wrapper. This would connect model–environment alignment with Trident-G horizontal transfer rather than task-specific fluency.

### Test 4: Manipulating niche coupling

Feedback controllability, reliability and action efficacy could be manipulated independently. This would test whether stronger agent–environment coupling improves structural inference, calibration and recovery after environmental change.

The Trident-G interpretation would be weakened if model–environment alignment failed to predict adaptation, transfer or action quality once response perseveration and task instructions were controlled.

---

## 8. Summary

Foucault and colleagues provide strong behavioural evidence that people do not assign a fixed meaning to prediction error: they alter learning and uncertainty-sensitive action according to whether their environment changes abruptly or gradually.

The results offer **convergent evidence** for the Trident-G niche-synergy principle, because adaptive performance emerged from alignment between environmental dynamics, internal generative assumptions, evidence weighting and action—but they do not directly test the wider Trident-G architecture.

The decisive next step is to determine whether people can discover, transfer and revise these structural models without instruction when the niche itself changes.

---

## References

Adams, R. P., & MacKay, D. J. C. (2007). Bayesian online changepoint detection. *arXiv*.  

Bruckner, R., Heekeren, H. R., & Nassar, M. R. (2025). Understanding learning through uncertainty and bias. *Communications Psychology, 3*, 24.

Foucault, C., Weber, L. A., & Hunt, L. (2026). Environmental dynamics shape human learning: Change points versus random walks. *eLife, 15*, RP110137. https://doi.org/10.7554/eLife.110137.1

Friston, K. (2010). The free-energy principle: A unified brain theory? *Nature Reviews Neuroscience, 11*, 127–138.

Gershman, S. J., & Niv, Y. (2010). Learning latent structure: Carving nature at its joints. *Current Opinion in Neurobiology, 20*, 251–256.

Marković, D., & Kiebel, S. J. (2016). Comparative analysis of behavioural models for adaptive learning in changing environments. *Frontiers in Computational Neuroscience, 10*, 33.

Mathys, C., Daunizeau, J., Friston, K. J., & Stephan, K. E. (2011). A Bayesian foundation for individual learning under uncertainty. *Frontiers in Human Neuroscience, 5*, 39.

Nassar, M. R., Wilson, R. C., Heasly, B., & Gold, J. I. (2010). An approximately Bayesian delta-rule model explains the dynamics of belief updating in a changing environment. *Journal of Neuroscience, 30*, 12366–12378.

Piray, P., & Daw, N. D. (2021). A model for learning based on the joint estimation of stochasticity and volatility. *Nature Communications, 12*, 6587.

Piray, P., & Daw, N. D. (2024). Computational processes of simultaneous learning of stochasticity and volatility in humans. *Nature Communications, 15*, 9073.

Pulcu, E., & Browning, M. (2025). Humans adapt rationally to approximate estimates of uncertainty. *eLife, 14*, RP103734.

Smith, M. A. (2026). *Trident G theory of general adaptive intelligence: A dynamical characterisation of intelligence as Griffiths Phase bifurcating dynamics*. Working theory document.
