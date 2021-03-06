---
layout: content
title: Artifact Evaluation
---

# Artifact Evaluation

# Call for Artifacts

Authors of accepted {{ site.conference.short_title }} {{ site.conference.year }} papers are invited to formally submit their supporting materials to the Artifact Evaluation (AE) process.
The [artifact evaluation committee]({{ '/organization/#artifact-evaluation-committee' | relative_url }}) attempts to reproduce (at least the main) experiments and assesses if submitted artifacts support the claims made in the paper.
The submission is voluntary and does not influence the final decision regarding the paper acceptance.

We invite every author of an accepted {{ site.conference.short_title }} paper to consider submitting an artifact.
At {{ site.conference.short_title }} we follow [ACM's artifact reviewing and badging policy](https://www.acm.org/publications/policies/artifact-review-badging).
ACM describes a research artifact as follows:

  > By “artifact” we mean a digital object that was either created by the authors to be used as part of the study or generated by the experiment itself. For example, artifacts can be software systems, scripts used to run experiments, input datasets, raw data collected in the experiment, or scripts used to analyse results.

### Artifact Evaluation Chairs
- [Bastian Hagedorn](https://bastianhagedorn.github.io/), University of Münster
- [Michel Steuwer](https://michel.steuwer.info/), University of Glasgow
- [Michael Laurenzano](http://www.gozano.com/), University of Michigan/Clinc

## Deadlines

--- | ---
**15 November 2019**       | Artifact Submission
**25 November -- 6 December 2019** | Artifact Evaluation Technical Clarification Period
**13 December 2019**       | Artifact Evaluation Notification


## Submission
Submissions are made via the artifact evaluation submission website: [https://cgo20ae.hotcrp.com/](https://cgo20ae.hotcrp.com/)

Authors submit:
 - the paper that has been accepted at {{ site.conference.short_title }}, extended with
 - an appendix providing a link to and describing the artifact.<br/> We recommend to use [this AE appendix template](http://ctuning.org/ae/templates/ae-20190108.tex) from ctuning.org where you can also find a [detailed description what information to provide](http://ctuning.org/ae/submission_extra.html).

For the artifact itself, we encourage the use of container or VM technologies like [Docker](https://www.docker.com/), [Singularity](https://sylabs.io/docs/), [Virtual Box](https://www.virtualbox.org/) or [Vagrant](https://www.vagrantup.com/) to package the artifact in one stand-alone container or VM which provides all required dependencies.
Giving AE reviewers remote access to your machines with preinstalled (proprietary) software is also possible.

**If you have an unusual experimental setup which requires specific hardware (i.e., custom hardware, oscilloscopes for measurements ...) or proprietary software please contact the [artifact evaluation chairs](#artifact-evaluation-chairs) before the submission.**

There are more tips preparing a submission available on the [ctuning website](http://ctuning.org/ae/submission-20190108.html).

# Evaluation Process
Each submitted artifact is evaluated by at least two members of the artifact evaluation committee.

During the process authors and evaluators are allowed to anonymously communicate with each other to overcome technical difficulties.<br/>
**Ideally, we hope to see all submitted artifacts to successfully pass artifact evaluation.**

The evaluators are asked to evaluate the artifact based on the following criteria, that are defined by [ACM](https://www.acm.org/publications/policies/artifact-review-badging).

### Is the artifact functional?
- Package complete?
    All components relevant to evaluation are included in the package?
- Well documented?
    Enough to understand, install and evaluate artifact?
- Exercisable?
    Includes scripts and/or software to perform appropriate experiments and generate results?
- Consistent?
    Artifacts are relevant to the associated paper and contribute in some inherent way to the generation of its main results?

The artifacts associated with the paper will receive an "Artifacts Evaluated - Functional" badge only if they are found to be documented, consistent, complete, exercisable, and include appropriate evidence of verification and validation.

### Is the artifact customizable and reusable?
- Can this artifact and experimental workflow be easily reused and customized?<br/>
    For example, can it be used on a different platform, with different benchmarks, data sets, compilers, tools, under different conditions and parameters, etc.?
    
The artifacts associated with the paper will receive an "Artifact Evaluated - Reusable" badge only if they are of a quality that significantly exceeds minimal functionality.
That is, they have all the qualities of the Artifacts Evaluated - Functional level, but, in addition, they are very carefully documented and well-structured to the extent that reuse and repurposing are facilitated.
In particular, norms and standards of the research community for artifacts of this type are strictly adhered to.


### Have the results been validated?
- Can all main results from the paper be validated using provided artifacts?<br/>
  Evaluators are asked to report any unexpected artifact behavior (depends on the type of artifact such as unexpected output, scalability issues, crashes, performance variation, etc).

The artifacts associated with the paper will receive a "Results replicated" badge only if the main results of the paper have been obtained in a subsequent study by a person or team other than the authors, using, in part, artifacts provided by the author.
Note that variation of empirical and numerical results is tolerated.
In fact it is often unavoidable in computer systems research - see ["how to report and compare empirical results?" in AE FAQ on ctuning.org](http://ctuning.org/ae/faq.html)!

Based on the results the following badges are awarded.

# Badges

ACM recommends awarding three different type of badges to communicate how the artifact has been evaluated.<br/>
A single paper can receive up to three badges — one badge of each type.

:---: | :---: | :---:
![Artifact Available badge](/img/ae-badges/artifacts_available_dl.jpg) || The green _Artifacts Available badge_ indicates that an artifact is publicly accessible in an archival repository. For this badge to be awarded the paper does not have to be independently evaluated. ACM requires that a qualified archival repository is used, for example Zenodo, figshare, Dryad. Personal webpages, GitHub repositories or alike are not sufficient as it can be changed after the submission deadline! 

![Artifacts Evaluated badges](/img/ae-badges/artifacts_evaluated_functional_dl.jpg) | ![Artifacts Evaluated badges](/img/ae-badges/artifacts_evaluated_reusable_dl.jpg) | The red _Artifacts Evaluated badges_ indicate that a research artifact has been successfully completed an independent audit. A reviewer has verified that the artifact is documented, complete, consistent, and exercisable.
| | The lighter red _Artifacts Evaluated — Functional_ badge indicates a basic level of functionality. The darker red _Artifacts Evaluated — Reusable_ badge indicates a higher quality artifact which significantly exceeds minimal functionality so that reuse and repurposing is facilitated.

 ![Artifacts Evaluated badges](/img/ae-badges/results_replicated_dl.jpg) | ![Artifacts Evaluated badges](/img/ae-badges/results_reproduced_dl.jpg) | The blue _Results Validated badges_ indicate that the main results of the paper have been successfully obtained by an independent reviewer.
 | | The lighter blue _Results Replicated_ badge indicates that the main results of the paper have been successfully obtained using the provided artifact. The darker blue _Results Reproduced_ badge indicates that the main results of the paper have been independently obtained without using the author-provided research artifact.

At {{ site.conference.short_title }} the artifact evaluation committee awards for each successfully evaluated paper one of the two red _Artifacts Evaluated badges_ as well as the lighter blue _Results Replicated_ badge.
We _do not award_ the darker blue _Results Reproduced_ badge in this artifact evaluation process.
The green _Artifact Available badge_ does not require the formal audit and, therefore, is awarded directly by the publisher — if the authors provide a link to the deposited artifact.
