---
title: "Read-based isoLASER: comparison with GTEx brain sQTLs (FDR < 0.10, cis set on heterozygous donors)"
author: "XSun"
date: "2026-10-28"
output:
  workflowr::wflow_html:
    toc: true
    toc_float: true
---

<p>
<button type="button" class="btn btn-default btn-workflowr btn-workflowr-report"
  data-toggle="collapse" data-target="#workflowr-report">
  <span class="glyphicon glyphicon-list" aria-hidden="true"></span>
  workflowr
  <span class="glyphicon glyphicon-exclamation-sign text-danger" aria-hidden="true"></span>
</button>
</p>

<div id="workflowr-report" class="collapse">
<ul class="nav nav-tabs">
  <li class="active"><a data-toggle="tab" href="#summary">Summary</a></li>
  <li><a data-toggle="tab" href="#checks">
  Checks <span class="glyphicon glyphicon-exclamation-sign text-danger" aria-hidden="true"></span>
  </a></li>
  <li><a data-toggle="tab" href="#versions">Past versions</a></li>
</ul>

<div class="tab-content">
<div id="summary" class="tab-pane fade in active">
  <p><strong>Last updated:</strong> 2026-10-28</p>
  <p><strong>Checks:</strong>
  <span class="glyphicon glyphicon-ok text-success" aria-hidden="true"></span>
  6
  <span class="glyphicon glyphicon-exclamation-sign text-danger" aria-hidden="true"></span>
  1
  </p>
  <p><strong>Knit directory:</strong>
  <code>long_read_rna/</code>
  <span class="glyphicon glyphicon-question-sign" aria-hidden="true"
  title="This is the local directory in which the code in this file was executed.">
  </span>
  </p>
  <p>
  This reproducible <a href="https://rmarkdown.rstudio.com">R Markdown</a>
  analysis was created with <a
  href="https://github.com/workflowr/workflowr">workflowr</a> (version
  1.7.0). The <em>Checks</em> tab describes the
  reproducibility checks that were applied when the results were created.
  The <em>Past versions</em> tab lists the development history.
  </p>
<hr>
</div>
<div id="checks" class="tab-pane fade">
  <div class="panel-group" id="workflowr-checks">
  <div class="panel panel-default">
<div class="panel-heading">
<p class="panel-title">
<a data-toggle="collapse" data-parent="#workflowr-checks" href="#strongRMarkdownfilestronguncommittedchanges">
  <span class="glyphicon glyphicon-exclamation-sign text-danger" aria-hidden="true"></span>
  <strong>R Markdown file:</strong> uncommitted changes
</a>
</p>
</div>
<div id="strongRMarkdownfilestronguncommittedchanges" class="panel-collapse collapse">
<div class="panel-body">
  The R Markdown file has unstaged changes. 
To know which version of the R Markdown file created these
results, you'll want to first commit it to the Git repo. If
you're still working on the analysis, you can ignore this
warning. When you're finished, you can run
<code>wflow_publish</code> to commit the R Markdown file and
build the HTML.

</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<p class="panel-title">
<a data-toggle="collapse" data-parent="#workflowr-checks" href="#strongEnvironmentstrongempty">
  <span class="glyphicon glyphicon-ok text-success" aria-hidden="true"></span>
  <strong>Environment:</strong> empty
</a>
</p>
</div>
<div id="strongEnvironmentstrongempty" class="panel-collapse collapse">
<div class="panel-body">
  
Great job! The global environment was empty. Objects defined in the global
environment can affect the analysis in your R Markdown file in unknown ways.
For reproduciblity it's best to always run the code in an empty environment.

</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<p class="panel-title">
<a data-toggle="collapse" data-parent="#workflowr-checks" href="#strongSeedstrongcodesetseed20260908code">
  <span class="glyphicon glyphicon-ok text-success" aria-hidden="true"></span>
  <strong>Seed:</strong> <code>set.seed(20260908)</code>
</a>
</p>
</div>
<div id="strongSeedstrongcodesetseed20260908code" class="panel-collapse collapse">
<div class="panel-body">
  
The command <code>set.seed(20260908)</code> was run prior to running the code in the R Markdown file.
Setting a seed ensures that any results that rely on randomness, e.g.
subsampling or permutations, are reproducible.

</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<p class="panel-title">
<a data-toggle="collapse" data-parent="#workflowr-checks" href="#strongSessioninformationstrongrecorded">
  <span class="glyphicon glyphicon-ok text-success" aria-hidden="true"></span>
  <strong>Session information:</strong> recorded
</a>
</p>
</div>
<div id="strongSessioninformationstrongrecorded" class="panel-collapse collapse">
<div class="panel-body">
  
Great job! Recording the operating system, R version, and package versions is
critical for reproducibility.

</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<p class="panel-title">
<a data-toggle="collapse" data-parent="#workflowr-checks" href="#strongCachestrongnone">
  <span class="glyphicon glyphicon-ok text-success" aria-hidden="true"></span>
  <strong>Cache:</strong> none
</a>
</p>
</div>
<div id="strongCachestrongnone" class="panel-collapse collapse">
<div class="panel-body">
  
Nice! There were no cached chunks for this analysis, so you can be confident
that you successfully produced the results during this run.

</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<p class="panel-title">
<a data-toggle="collapse" data-parent="#workflowr-checks" href="#strongFilepathsstrongrelative">
  <span class="glyphicon glyphicon-ok text-success" aria-hidden="true"></span>
  <strong>File paths:</strong> relative
</a>
</p>
</div>
<div id="strongFilepathsstrongrelative" class="panel-collapse collapse">
<div class="panel-body">
  
Great job! Using relative paths to the files within your workflowr project
makes it easier to run your code on other machines.

</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<p class="panel-title">
<a data-toggle="collapse" data-parent="#workflowr-checks" href="#strongRepositoryversionstrongahrefhttpsgithubcomxsun1229longreadrnatreea43035e3a37a3c2658a8b1528f4dd9849c68581atargetblanka43035ea">
  <span class="glyphicon glyphicon-ok text-success" aria-hidden="true"></span>
  <strong>Repository version:</strong> <a href="https://github.com/xsun1229/long_read_rna/tree/a43035e3a37a3c2658a8b1528f4dd9849c68581a" target="_blank">a43035e</a>
</a>
</p>
</div>
<div id="strongRepositoryversionstrongahrefhttpsgithubcomxsun1229longreadrnatreea43035e3a37a3c2658a8b1528f4dd9849c68581atargetblanka43035ea" class="panel-collapse collapse">
<div class="panel-body">
  
<p>
Great! You are using Git for version control. Tracking code development and
connecting the code version to the results is critical for reproducibility.
</p>

<p>
The results in this page were generated with repository version <a href="https://github.com/xsun1229/long_read_rna/tree/a43035e3a37a3c2658a8b1528f4dd9849c68581a" target="_blank">a43035e</a>.
See the <em>Past versions</em> tab to see a history of the changes made to the
R Markdown and HTML files.
</p>

<p>
Note that you need to be careful to ensure that all relevant files for the
analysis have been committed to Git prior to generating the results (you can
use <code>wflow_publish</code> or <code>wflow_git_commit</code>). workflowr only
checks the R Markdown file, but you know if there are other scripts or data
files that it depends on. Below is the status of the Git repository when the
results were generated:
</p>

<pre><code>
Untracked files:
	Untracked:  analysis/isolaser_fdr_panel10nc_q010_hetcis.Rmd
	Untracked:  analysis/isolaser_fdr_reads10nc_q010_hetcis.Rmd

Unstaged changes:
	Modified:   analysis/index.Rmd
	Modified:   analysis/isolaser_gtex_comparison_panel10nc_q010_hetcis.Rmd
	Modified:   analysis/isolaser_gtex_comparison_reads10nc_q010_hetcis.Rmd

</code></pre>

<p>
Note that any generated files, e.g. HTML, png, CSS, etc., are not included in
this status report because it is ok for generated content to have uncommitted
changes.
</p>

</div>
</div>
</div>
</div>
<hr>
</div>
<div id="versions" class="tab-pane fade">
  
<p>
These are the previous versions of the repository in which changes were made
to the R Markdown (<code>analysis/isolaser_gtex_comparison_reads10nc_q010_hetcis.Rmd</code>) and HTML (<code>docs/isolaser_gtex_comparison_reads10nc_q010_hetcis.html</code>)
files. If you've configured a remote Git repository (see
<code>?wflow_git_remote</code>), click on the hyperlinks in the table below to
view the files as they were in that past version.
</p>
<div class="table-responsive">
<table class="table table-condensed table-hover">
<thead>
<tr>
<th>File</th>
<th>Version</th>
<th>Author</th>
<th>Date</th>
<th>Message</th>
</tr>
</thead>
<tbody>
<tr>
<td>Rmd</td>
<td><a href="https://github.com/xsun1229/long_read_rna/blob/a43035e3a37a3c2658a8b1528f4dd9849c68581a/analysis/isolaser_gtex_comparison_reads10nc_q010_hetcis.Rmd" target="_blank">a43035e</a></td>
<td>XSun</td>
<td>2026-10-28</td>
<td>update</td>
</tr>
</tbody>
</table>
</div>

<hr>
</div>
</div>
</div>








This page compares **read-based isoLASER** without the clustering filter
([FDR page](isolaser_fdr_reads10nc_q010.html)) with GTEx v8 sQTLs in the nine brain
tissues that have full summary statistics. As in the right panel of
[Fig. 3e of the isoLASER paper](https://www.nature.com/articles/s41467-025-64605-6),
we compare our allelic splicing effects (isoLASER ΔPSI) with GTEx sQTL effects
(beta), using each event's **skipping junction**. Its usage falls when the exonic
part is included, so a **negative correlation** is expected.

# How pairs were matched

- **Variant and gene:** the same SNV (position, REF and ALT; isoLASER's 0-based
  position + 1 = GTEx's), tested for the same Ensembl gene in GTEx.
- **GTEx data:** the full summary statistics, every tested association at any
  p-value. Nine of GTEx's 13 brain tissues have them on the cluster. The other four
  (Amygdala, Anterior cingulate cortex BA24, Spinal cord cervical c-1 and
  Substantia nigra) have only GTEx's significant pairs and are left out. This
  differs from the paper, whose Methods describe an overlap with GTEx's
  significant pairs: here pairs that GTEx does not call significant (the grey
  points) are included.
- **Event:** the exonic part must form an annotated exon-skipping or
  alternative-splice-site event, and the GTEx junction must be exactly that
  event's skipping junction.
- **Points:** each point is one **pair**: an isoLASER association (variant ×
  exonic part) and its matched GTEx skipping junction, at one timepoint.

Our associations come in three sets:

- **isoLASER cis, heterozygous donors** (our definition): isoLASER's own `cis`
  cutoff, computed in this run from the panel-heterozygous donors only (≥ 10
  reads each, ≥ 20 over those donors, part ≥ 10 bp), with no ΔPSI or q cutoff.
  It replaces the paper's cutoff of the [earlier version](isolaser_gtex_comparison_reads10nc_q010.html),
  isoLASER's joint output. That set also used variants absent from the donors'
  genotype panel, and pooled homozygous donors.
- **Before FDR:** the same plus \|ΔPSI\| ≥ 0.05: this run's screen. There is
  no clustering filter.
- **After FDR:** the same plus permutation BH q < 0.10 within each timepoint, as
  on [this run's FDR page](isolaser_fdr_reads10nc_q010.html).

The cutoffs are those of this run's [FDR page](isolaser_fdr_reads10nc_q010.html):
\|ΔPSI\| ≥ 0.05 and BH q < 0.10. The BH q-values were calculated over the full
eligible family of tested associations in each timepoint, before the `cis` and
\|ΔPSI\| display filters are applied, so the effect-size screen changes no
q-value. Earlier versions used q < 0.05 ([page](isolaser_gtex_comparison_reads10nc.html)) and the
paper's cutoff as the first set ([page](isolaser_gtex_comparison_reads10nc_q010.html)).

**Example, HNRNPK.** The C>T variant (chr9:83980154, 0-based) and the 34-base
exonic part (gold) form an alternative splice site. GTEx measures the
skipping junction (blue), which jumps over the part. At 6 hours, ALT changes
part inclusion by -26.5 percentage points in this
run. GTEx Cerebellum's beta for the skipping junction is
+0.97: opposite signs, as expected.

![](assets/isolaser_gtex_reads10nc_q010_hetcis/comparable_event_example_skipping.png)

# Scatter plots {.tabset}

One tab per tissue. Rows are the three sets and columns the timepoints; each
panel title gives the pairs, genes, Pearson R and p. Blue: GTEx nominal
p < 0.05; grey: p ≥ 0.05. The line is a least-squares fit, drawn when a panel
has 3 or more pairs.

## Cerebellum

![](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Cerebellum.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Cerebellum.pdf)

## Cerebellar Hemisphere

![](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Cerebellar_Hemisphere.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Cerebellar_Hemisphere.pdf)

## Caudate basal ganglia

![](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Caudate_basal_ganglia.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Caudate_basal_ganglia.pdf)

## Cortex

![](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Cortex.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Cortex.pdf)

## Frontal Cortex BA9

![](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Frontal_Cortex_BA9.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Frontal_Cortex_BA9.pdf)

## Hippocampus

![](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Hippocampus.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Hippocampus.pdf)

## Hypothalamus

![](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Hypothalamus.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Hypothalamus.pdf)

## Nucleus accumbens basal ganglia

![](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Nucleus_accumbens_basal_ganglia.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Nucleus_accumbens_basal_ganglia.pdf)

## Putamen basal ganglia

![](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Putamen_basal_ganglia.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_Brain_Putamen_basal_ganglia.pdf)

# Testing

## How the testing works

Two tests, both on the skipping-junction pairs, for each set and tissue:

- **Correlation** (as in the paper): the Pearson correlation of our ΔPSI with
  GTEx's beta, for each timepoint. A negative R is expected. **Expected sign**
  counts the pairs where the two have opposite signs. **GTEx p < 1e-5** repeats
  the count for pairs where GTEx itself has strong evidence.
- **Sign consistency** (our definition; the paper reports only the
  correlation):
  - we take the pairs where GTEx is significant (nominal p < 0.05, the blue
    points) and our ΔPSI is not 0;
  - a pair is **consistent** when our ΔPSI and GTEx's beta have opposite signs;
  - a binomial test asks whether the share of consistent pairs differs from 50%
    (two-sided) or is above it, the expected direction (one-sided).

  We count this per timepoint, and over all timepoints with **each pair
  once**: each pair's mean ΔPSI over the timepoints where it is called, so an
  association reported at several timepoints counts once.

**The binomial p-values are exploratory.** The test assumes independent pairs,
and they are not:

- pairs can come from the same gene or exonic part, so related variants count
  separately;
- the same associations recur in every tissue;
- nothing corrects for the many sets, timepoints and tissues tested.

For example, after FDR the pairs with GTEx p < 0.05 are 6 pairs at
5 exonic parts in 5
genes (ATP5MJ, DGCR6L, HNRNPK, PPA2, SNHG5), over all nine tissues. Their agreement
is useful descriptive evidence, but the binomial p treats them as 6
independent trials. A formal test would have to account for dependence within
genes and loci, and for multiple comparisons.

## Results {.tabset}

In each tab:

- **Pairs matched**: per set and timepoint, our associations (variant × exonic
  part, single-base variants), those whose variant GTEx tests for the same gene in
  that tissue, the plotted pairs and their genes.
- **Correlation** and **Sign consistency**, as defined above.

Most of the cis set's associations are tested in GTEx for the same variant and
gene: 78.7&ndash;88.2% across tissues and timepoints (Cerebellum at 0 hr:
282 of 355,
79.4%,
with 39 plotted pairs). Fewer form an annotated event with a
matching skipping junction. For the paper's cutoff on the
[earlier version](isolaser_gtex_comparison_reads10nc_q010.html), only a minority were
tested, because many of its variants are not in the donors' genotype panel.

### Cerebellum

**Pairs matched**

|Set                      |Timepoint | Our associations (SNVs)| Same variant and gene tested in GTEx| Plotted pairs| Genes|
|:------------------------|:---------|-----------------------:|------------------------------------:|-------------:|-----:|
|isoLASER cis, het donors |0 hr      |                     355|                                  282|            39|    25|
|isoLASER cis, het donors |1 hr      |                     656|                                  516|            83|    56|
|isoLASER cis, het donors |6 hr      |                     716|                                  568|            65|    44|
|Before FDR               |0 hr      |                     194|                                  170|            26|    18|
|Before FDR               |1 hr      |                     359|                                  331|            57|    40|
|Before FDR               |6 hr      |                     403|                                  362|            40|    30|
|After FDR                |0 hr      |                      21|                                   20|             5|     4|
|After FDR                |1 hr      |                      27|                                   26|             4|     3|
|After FDR                |6 hr      |                      39|                                   27|             5|     4|

**Correlation**

|Set                      |Timepoint | Pairs|    All: R (p)| All: expected sign| GTEx p < 1e-5: expected sign|
|:------------------------|:---------|-----:|-------------:|------------------:|----------------------------:|
|isoLASER cis, het donors |0 hr      |    39|  -0.26 (0.11)|              28/39|                        10/11|
|isoLASER cis, het donors |1 hr      |    83|  -0.16 (0.15)|              48/83|                        19/25|
|isoLASER cis, het donors |6 hr      |    65| -0.25 (0.042)|              40/65|                        15/17|
|Before FDR               |0 hr      |    26| -0.42 (0.034)|              20/26|                          8/8|
|Before FDR               |1 hr      |    57|  -0.21 (0.11)|              35/57|                        14/17|
|Before FDR               |6 hr      |    40| -0.32 (0.043)|              27/40|                        12/12|
|After FDR                |0 hr      |     5|  -0.47 (0.42)|                5/5|                          3/3|
|After FDR                |1 hr      |     4|  -0.83 (0.17)|                4/4|                          4/4|
|After FDR                |6 hr      |     5| -0.83 (0.079)|                5/5|                          4/4|

**Sign consistency** (pairs with GTEx p < 0.05; the binomial p-values are exploratory)

|Set                      |Timepoint                      | Pairs| Consistent| Consistent (%)| Binomial p, two-sided| Binomial p, one-sided|
|:------------------------|:------------------------------|-----:|----------:|--------------:|---------------------:|---------------------:|
|isoLASER cis, het donors |0 hr                           |    18|         16|             89|                0.0013|               0.00066|
|isoLASER cis, het donors |1 hr                           |    40|         24|             60|                  0.27|                  0.13|
|isoLASER cis, het donors |6 hr                           |    25|         18|             72|                 0.043|                 0.022|
|isoLASER cis, het donors |All timepoints, each pair once |    61|         38|             62|                 0.072|                 0.036|
|Before FDR               |0 hr                           |    13|         12|             92|                0.0034|                0.0017|
|Before FDR               |1 hr                           |    27|         17|             63|                  0.25|                  0.12|
|Before FDR               |6 hr                           |    16|         14|             88|                0.0042|                0.0021|
|Before FDR               |All timepoints, each pair once |    44|         31|             70|                0.0096|                0.0048|
|After FDR                |0 hr                           |     3|          3|            100|                  0.25|                  0.12|
|After FDR                |1 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |6 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |All timepoints, each pair once |     5|          5|            100|                 0.062|                 0.031|

### Cerebellar Hemisphere

**Pairs matched**

|Set                      |Timepoint | Our associations (SNVs)| Same variant and gene tested in GTEx| Plotted pairs| Genes|
|:------------------------|:---------|-----------------------:|------------------------------------:|-------------:|-----:|
|isoLASER cis, het donors |0 hr      |                     355|                                  286|            42|    28|
|isoLASER cis, het donors |1 hr      |                     656|                                  517|            82|    55|
|isoLASER cis, het donors |6 hr      |                     716|                                  565|            69|    48|
|Before FDR               |0 hr      |                     194|                                  173|            28|    20|
|Before FDR               |1 hr      |                     359|                                  331|            57|    40|
|Before FDR               |6 hr      |                     403|                                  364|            42|    31|
|After FDR                |0 hr      |                      21|                                   20|             5|     4|
|After FDR                |1 hr      |                      27|                                   26|             4|     3|
|After FDR                |6 hr      |                      39|                                   27|             5|     4|

**Correlation**

|Set                      |Timepoint | Pairs|    All: R (p)| All: expected sign| GTEx p < 1e-5: expected sign|
|:------------------------|:---------|-----:|-------------:|------------------:|----------------------------:|
|isoLASER cis, het donors |0 hr      |    42| -0.37 (0.015)|              28/42|                          7/7|
|isoLASER cis, het donors |1 hr      |    82| -0.19 (0.089)|              44/82|                        14/17|
|isoLASER cis, het donors |6 hr      |    69| -0.28 (0.019)|              36/69|                        14/14|
|Before FDR               |0 hr      |    28| -0.45 (0.017)|              23/28|                          7/7|
|Before FDR               |1 hr      |    57|  -0.22 (0.11)|              31/57|                        13/14|
|Before FDR               |6 hr      |    42| -0.32 (0.041)|              25/42|                        13/13|
|After FDR                |0 hr      |     5|  -0.51 (0.38)|                5/5|                          3/3|
|After FDR                |1 hr      |     4|  -0.83 (0.17)|                4/4|                          4/4|
|After FDR                |6 hr      |     5| -0.84 (0.073)|                4/5|                          4/4|

**Sign consistency** (pairs with GTEx p < 0.05; the binomial p-values are exploratory)

|Set                      |Timepoint                      | Pairs| Consistent| Consistent (%)| Binomial p, two-sided| Binomial p, one-sided|
|:------------------------|:------------------------------|-----:|----------:|--------------:|---------------------:|---------------------:|
|isoLASER cis, het donors |0 hr                           |    16|         15|             94|               0.00052|               0.00026|
|isoLASER cis, het donors |1 hr                           |    34|         23|             68|                 0.058|                 0.029|
|isoLASER cis, het donors |6 hr                           |    28|         21|             75|                 0.013|                0.0063|
|isoLASER cis, het donors |All timepoints, each pair once |    57|         39|             68|                0.0075|                0.0038|
|Before FDR               |0 hr                           |    13|         12|             92|                0.0034|                0.0017|
|Before FDR               |1 hr                           |    21|         16|             76|                 0.027|                 0.013|
|Before FDR               |6 hr                           |    19|         16|             84|                0.0044|                0.0022|
|Before FDR               |All timepoints, each pair once |    40|         31|             78|               0.00068|               0.00034|
|After FDR                |0 hr                           |     3|          3|            100|                  0.25|                  0.12|
|After FDR                |1 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |6 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |All timepoints, each pair once |     5|          5|            100|                 0.062|                 0.031|

### Caudate basal ganglia

**Pairs matched**

|Set                      |Timepoint | Our associations (SNVs)| Same variant and gene tested in GTEx| Plotted pairs| Genes|
|:------------------------|:---------|-----------------------:|------------------------------------:|-------------:|-----:|
|isoLASER cis, het donors |0 hr      |                     355|                                  303|            38|    26|
|isoLASER cis, het donors |1 hr      |                     656|                                  545|            85|    57|
|isoLASER cis, het donors |6 hr      |                     716|                                  598|            61|    40|
|Before FDR               |0 hr      |                     194|                                  168|            24|    18|
|Before FDR               |1 hr      |                     359|                                  336|            59|    41|
|Before FDR               |6 hr      |                     403|                                  369|            36|    26|
|After FDR                |0 hr      |                      21|                                   20|             5|     4|
|After FDR                |1 hr      |                      27|                                   26|             4|     3|
|After FDR                |6 hr      |                      39|                                   33|             5|     4|

**Correlation**

|Set                      |Timepoint | Pairs|     All: R (p)| All: expected sign| GTEx p < 1e-5: expected sign|
|:------------------------|:---------|-----:|--------------:|------------------:|----------------------------:|
|isoLASER cis, het donors |0 hr      |    38|   -0.25 (0.12)|              29/38|                          6/7|
|isoLASER cis, het donors |1 hr      |    85|  -0.25 (0.023)|              43/85|                        18/20|
|isoLASER cis, het donors |6 hr      |    61|  -0.25 (0.053)|              32/61|                        12/13|
|Before FDR               |0 hr      |    24|  -0.49 (0.016)|              21/24|                          4/4|
|Before FDR               |1 hr      |    59| -0.34 (0.0076)|              31/59|                        14/14|
|Before FDR               |6 hr      |    36|  -0.32 (0.056)|              23/36|                        10/10|
|After FDR                |0 hr      |     5|   -0.57 (0.31)|                5/5|                          2/2|
|After FDR                |1 hr      |     4|   -0.86 (0.14)|                4/4|                          3/3|
|After FDR                |6 hr      |     5|  -0.94 (0.017)|                5/5|                          3/3|

**Sign consistency** (pairs with GTEx p < 0.05; the binomial p-values are exploratory)

|Set                      |Timepoint                      | Pairs| Consistent| Consistent (%)| Binomial p, two-sided| Binomial p, one-sided|
|:------------------------|:------------------------------|-----:|----------:|--------------:|---------------------:|---------------------:|
|isoLASER cis, het donors |0 hr                           |    16|         14|             88|                0.0042|                0.0021|
|isoLASER cis, het donors |1 hr                           |    34|         26|             76|                0.0029|                0.0015|
|isoLASER cis, het donors |6 hr                           |    22|         16|             73|                 0.052|                 0.026|
|isoLASER cis, het donors |All timepoints, each pair once |    52|         37|             71|                0.0032|                0.0016|
|Before FDR               |0 hr                           |    11|         11|            100|               0.00098|               0.00049|
|Before FDR               |1 hr                           |    23|         19|             83|                0.0026|                0.0013|
|Before FDR               |6 hr                           |    14|         13|             93|                0.0018|               0.00092|
|Before FDR               |All timepoints, each pair once |    36|         31|             86|               1.3e-05|               6.5e-06|
|After FDR                |0 hr                           |     3|          3|            100|                  0.25|                  0.12|
|After FDR                |1 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |6 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |All timepoints, each pair once |     5|          5|            100|                 0.062|                 0.031|

### Cortex

**Pairs matched**

|Set                      |Timepoint | Our associations (SNVs)| Same variant and gene tested in GTEx| Plotted pairs| Genes|
|:------------------------|:---------|-----------------------:|------------------------------------:|-------------:|-----:|
|isoLASER cis, het donors |0 hr      |                     355|                                  291|            41|    27|
|isoLASER cis, het donors |1 hr      |                     656|                                  519|            80|    53|
|isoLASER cis, het donors |6 hr      |                     716|                                  571|            62|    40|
|Before FDR               |0 hr      |                     194|                                  177|            28|    20|
|Before FDR               |1 hr      |                     359|                                  338|            57|    39|
|Before FDR               |6 hr      |                     403|                                  367|            38|    27|
|After FDR                |0 hr      |                      21|                                   20|             6|     5|
|After FDR                |1 hr      |                      27|                                   26|             4|     3|
|After FDR                |6 hr      |                      39|                                   33|             5|     4|

**Correlation**

|Set                      |Timepoint | Pairs|     All: R (p)| All: expected sign| GTEx p < 1e-5: expected sign|
|:------------------------|:---------|-----:|--------------:|------------------:|----------------------------:|
|isoLASER cis, het donors |0 hr      |    41|  -0.27 (0.086)|              29/41|                          8/9|
|isoLASER cis, het donors |1 hr      |    80|  -0.27 (0.015)|              47/80|                        15/18|
|isoLASER cis, het donors |6 hr      |    62|  -0.29 (0.024)|              33/62|                        15/17|
|Before FDR               |0 hr      |    28|  -0.45 (0.015)|              23/28|                          6/6|
|Before FDR               |1 hr      |    57| -0.38 (0.0037)|              35/57|                        12/12|
|Before FDR               |6 hr      |    38|  -0.37 (0.024)|              26/38|                        13/13|
|After FDR                |0 hr      |     6|   -0.39 (0.45)|                5/6|                          3/3|
|After FDR                |1 hr      |     4|    -0.80 (0.2)|                4/4|                          4/4|
|After FDR                |6 hr      |     5|  -0.90 (0.036)|                5/5|                          4/4|

**Sign consistency** (pairs with GTEx p < 0.05; the binomial p-values are exploratory)

|Set                      |Timepoint                      | Pairs| Consistent| Consistent (%)| Binomial p, two-sided| Binomial p, one-sided|
|:------------------------|:------------------------------|-----:|----------:|--------------:|---------------------:|---------------------:|
|isoLASER cis, het donors |0 hr                           |    19|         18|             95|               7.6e-05|               3.8e-05|
|isoLASER cis, het donors |1 hr                           |    32|         25|             78|                0.0021|                0.0011|
|isoLASER cis, het donors |6 hr                           |    24|         18|             75|                 0.023|                 0.011|
|isoLASER cis, het donors |All timepoints, each pair once |    54|         42|             78|               5.2e-05|               2.6e-05|
|Before FDR               |0 hr                           |    15|         15|            100|               6.1e-05|               3.1e-05|
|Before FDR               |1 hr                           |    24|         20|             83|                0.0015|               0.00077|
|Before FDR               |6 hr                           |    17|         15|             88|                0.0023|                0.0012|
|Before FDR               |All timepoints, each pair once |    42|         37|             88|               4.4e-07|               2.2e-07|
|After FDR                |0 hr                           |     3|          3|            100|                  0.25|                  0.12|
|After FDR                |1 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |6 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |All timepoints, each pair once |     5|          5|            100|                 0.062|                 0.031|

### Frontal Cortex BA9

**Pairs matched**

|Set                      |Timepoint | Our associations (SNVs)| Same variant and gene tested in GTEx| Plotted pairs| Genes|
|:------------------------|:---------|-----------------------:|------------------------------------:|-------------:|-----:|
|isoLASER cis, het donors |0 hr      |                     355|                                  292|            41|    27|
|isoLASER cis, het donors |1 hr      |                     656|                                  516|            83|    55|
|isoLASER cis, het donors |6 hr      |                     716|                                  568|            64|    42|
|Before FDR               |0 hr      |                     194|                                  178|            27|    19|
|Before FDR               |1 hr      |                     359|                                  335|            58|    40|
|Before FDR               |6 hr      |                     403|                                  365|            40|    29|
|After FDR                |0 hr      |                      21|                                   20|             5|     4|
|After FDR                |1 hr      |                      27|                                   26|             4|     3|
|After FDR                |6 hr      |                      39|                                   33|             5|     4|

**Correlation**

|Set                      |Timepoint | Pairs|    All: R (p)| All: expected sign| GTEx p < 1e-5: expected sign|
|:------------------------|:---------|-----:|-------------:|------------------:|----------------------------:|
|isoLASER cis, het donors |0 hr      |    41|  -0.20 (0.22)|              26/41|                         9/10|
|isoLASER cis, het donors |1 hr      |    83|  -0.23 (0.04)|              47/83|                        15/18|
|isoLASER cis, het donors |6 hr      |    64| -0.28 (0.026)|              35/64|                        15/16|
|Before FDR               |0 hr      |    27| -0.37 (0.055)|              18/27|                          7/7|
|Before FDR               |1 hr      |    58| -0.32 (0.014)|              35/58|                        12/13|
|Before FDR               |6 hr      |    40| -0.37 (0.018)|              28/40|                        13/13|
|After FDR                |0 hr      |     5|  -0.48 (0.41)|                4/5|                          3/3|
|After FDR                |1 hr      |     4|  -0.87 (0.13)|                4/4|                          4/4|
|After FDR                |6 hr      |     5| -0.94 (0.019)|                5/5|                          4/4|

**Sign consistency** (pairs with GTEx p < 0.05; the binomial p-values are exploratory)

|Set                      |Timepoint                      | Pairs| Consistent| Consistent (%)| Binomial p, two-sided| Binomial p, one-sided|
|:------------------------|:------------------------------|-----:|----------:|--------------:|---------------------:|---------------------:|
|isoLASER cis, het donors |0 hr                           |    15|         14|             93|               0.00098|               0.00049|
|isoLASER cis, het donors |1 hr                           |    34|         23|             68|                 0.058|                 0.029|
|isoLASER cis, het donors |6 hr                           |    25|         18|             72|                 0.043|                 0.022|
|isoLASER cis, het donors |All timepoints, each pair once |    54|         36|             67|                  0.02|                0.0099|
|Before FDR               |0 hr                           |    11|         11|            100|               0.00098|               0.00049|
|Before FDR               |1 hr                           |    24|         18|             75|                 0.023|                 0.011|
|Before FDR               |6 hr                           |    17|         15|             88|                0.0023|                0.0012|
|Before FDR               |All timepoints, each pair once |    39|         31|             79|               0.00029|               0.00015|
|After FDR                |0 hr                           |     3|          3|            100|                  0.25|                  0.12|
|After FDR                |1 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |6 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |All timepoints, each pair once |     5|          5|            100|                 0.062|                 0.031|

### Hippocampus

**Pairs matched**

|Set                      |Timepoint | Our associations (SNVs)| Same variant and gene tested in GTEx| Plotted pairs| Genes|
|:------------------------|:---------|-----------------------:|------------------------------------:|-------------:|-----:|
|isoLASER cis, het donors |0 hr      |                     355|                                  308|            42|    28|
|isoLASER cis, het donors |1 hr      |                     656|                                  543|            84|    56|
|isoLASER cis, het donors |6 hr      |                     716|                                  596|            66|    43|
|Before FDR               |0 hr      |                     194|                                  174|            27|    19|
|Before FDR               |1 hr      |                     359|                                  334|            58|    40|
|Before FDR               |6 hr      |                     403|                                  368|            39|    28|
|After FDR                |0 hr      |                      21|                                   20|             5|     4|
|After FDR                |1 hr      |                      27|                                   26|             4|     3|
|After FDR                |6 hr      |                      39|                                   33|             5|     4|

**Correlation**

|Set                      |Timepoint | Pairs|     All: R (p)| All: expected sign| GTEx p < 1e-5: expected sign|
|:------------------------|:---------|-----:|--------------:|------------------:|----------------------------:|
|isoLASER cis, het donors |0 hr      |    42|  -0.30 (0.053)|              32/42|                          5/6|
|isoLASER cis, het donors |1 hr      |    84|   -0.24 (0.03)|              52/84|                        13/16|
|isoLASER cis, het donors |6 hr      |    66| -0.33 (0.0064)|              38/66|                        11/14|
|Before FDR               |0 hr      |    27|  -0.46 (0.015)|              22/27|                          3/3|
|Before FDR               |1 hr      |    58|  -0.31 (0.017)|              37/58|                        10/11|
|Before FDR               |6 hr      |    39| -0.43 (0.0065)|              27/39|                          9/9|
|After FDR                |0 hr      |     5|   -0.42 (0.48)|                3/5|                         none|
|After FDR                |1 hr      |     4|   -0.86 (0.14)|                4/4|                          1/1|
|After FDR                |6 hr      |     5| -0.96 (0.0084)|                5/5|                          1/1|

**Sign consistency** (pairs with GTEx p < 0.05; the binomial p-values are exploratory)

|Set                      |Timepoint                      | Pairs| Consistent| Consistent (%)| Binomial p, two-sided| Binomial p, one-sided|
|:------------------------|:------------------------------|-----:|----------:|--------------:|---------------------:|---------------------:|
|isoLASER cis, het donors |0 hr                           |    17|         15|             88|                0.0023|                0.0012|
|isoLASER cis, het donors |1 hr                           |    33|         23|             70|                 0.035|                 0.018|
|isoLASER cis, het donors |6 hr                           |    25|         20|             80|                0.0041|                 0.002|
|isoLASER cis, het donors |All timepoints, each pair once |    54|         38|             70|                0.0038|                0.0019|
|Before FDR               |0 hr                           |    12|         10|             83|                 0.039|                 0.019|
|Before FDR               |1 hr                           |    23|         17|             74|                 0.035|                 0.017|
|Before FDR               |6 hr                           |    18|         18|            100|               7.6e-06|               3.8e-06|
|Before FDR               |All timepoints, each pair once |    40|         32|             80|               0.00018|               9.1e-05|
|After FDR                |0 hr                           |     4|          3|             75|                  0.62|                  0.31|
|After FDR                |1 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |6 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |All timepoints, each pair once |     6|          5|             83|                  0.22|                  0.11|

### Hypothalamus

**Pairs matched**

|Set                      |Timepoint | Our associations (SNVs)| Same variant and gene tested in GTEx| Plotted pairs| Genes|
|:------------------------|:---------|-----------------------:|------------------------------------:|-------------:|-----:|
|isoLASER cis, het donors |0 hr      |                     355|                                  313|            39|    26|
|isoLASER cis, het donors |1 hr      |                     656|                                  535|            81|    54|
|isoLASER cis, het donors |6 hr      |                     716|                                  591|            63|    43|
|Before FDR               |0 hr      |                     194|                                  179|            26|    19|
|Before FDR               |1 hr      |                     359|                                  335|            59|    41|
|Before FDR               |6 hr      |                     403|                                  368|            38|    28|
|After FDR                |0 hr      |                      21|                                   20|             6|     5|
|After FDR                |1 hr      |                      27|                                   26|             4|     3|
|After FDR                |6 hr      |                      39|                                   33|             5|     4|

**Correlation**

|Set                      |Timepoint | Pairs|     All: R (p)| All: expected sign| GTEx p < 1e-5: expected sign|
|:------------------------|:---------|-----:|--------------:|------------------:|----------------------------:|
|isoLASER cis, het donors |0 hr      |    39|  -0.33 (0.039)|              24/39|                          6/7|
|isoLASER cis, het donors |1 hr      |    81|  -0.21 (0.059)|              41/81|                        16/17|
|isoLASER cis, het donors |6 hr      |    63|  -0.30 (0.018)|              38/63|                        12/13|
|Before FDR               |0 hr      |    26| -0.52 (0.0066)|              20/26|                          4/4|
|Before FDR               |1 hr      |    59|   -0.27 (0.04)|              31/59|                        12/12|
|Before FDR               |6 hr      |    38|  -0.39 (0.015)|              29/38|                        10/10|
|After FDR                |0 hr      |     6|   -0.48 (0.34)|                6/6|                          2/2|
|After FDR                |1 hr      |     4|  -0.93 (0.069)|                4/4|                          3/3|
|After FDR                |6 hr      |     5|  -0.97 (0.005)|                5/5|                          3/3|

**Sign consistency** (pairs with GTEx p < 0.05; the binomial p-values are exploratory)

|Set                      |Timepoint                      | Pairs| Consistent| Consistent (%)| Binomial p, two-sided| Binomial p, one-sided|
|:------------------------|:------------------------------|-----:|----------:|--------------:|---------------------:|---------------------:|
|isoLASER cis, het donors |0 hr                           |    15|         14|             93|               0.00098|               0.00049|
|isoLASER cis, het donors |1 hr                           |    30|         22|             73|                 0.016|                0.0081|
|isoLASER cis, het donors |6 hr                           |    21|         16|             76|                 0.027|                 0.013|
|isoLASER cis, het donors |All timepoints, each pair once |    47|         34|             72|                0.0031|                0.0015|
|Before FDR               |0 hr                           |    12|         12|            100|               0.00049|               0.00024|
|Before FDR               |1 hr                           |    22|         17|             77|                 0.017|                0.0085|
|Before FDR               |6 hr                           |    14|         13|             93|                0.0018|               0.00092|
|Before FDR               |All timepoints, each pair once |    36|         30|             83|                 7e-05|               3.5e-05|
|After FDR                |0 hr                           |     3|          3|            100|                  0.25|                  0.12|
|After FDR                |1 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |6 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |All timepoints, each pair once |     5|          5|            100|                 0.062|                 0.031|

### Nucleus accumbens basal ganglia

**Pairs matched**

|Set                      |Timepoint | Our associations (SNVs)| Same variant and gene tested in GTEx| Plotted pairs| Genes|
|:------------------------|:---------|-----------------------:|------------------------------------:|-------------:|-----:|
|isoLASER cis, het donors |0 hr      |                     355|                                  291|            42|    28|
|isoLASER cis, het donors |1 hr      |                     656|                                  516|            86|    58|
|isoLASER cis, het donors |6 hr      |                     716|                                  569|            63|    41|
|Before FDR               |0 hr      |                     194|                                  176|            28|    20|
|Before FDR               |1 hr      |                     359|                                  336|            60|    42|
|Before FDR               |6 hr      |                     403|                                  366|            39|    28|
|After FDR                |0 hr      |                      21|                                   20|             5|     4|
|After FDR                |1 hr      |                      27|                                   26|             4|     3|
|After FDR                |6 hr      |                      39|                                   33|             5|     4|

**Correlation**

|Set                      |Timepoint | Pairs|    All: R (p)| All: expected sign| GTEx p < 1e-5: expected sign|
|:------------------------|:---------|-----:|-------------:|------------------:|----------------------------:|
|isoLASER cis, het donors |0 hr      |    42| -0.33 (0.035)|              27/42|                        10/11|
|isoLASER cis, het donors |1 hr      |    86|  -0.23 (0.03)|              46/86|                        16/17|
|isoLASER cis, het donors |6 hr      |    63|  -0.29 (0.02)|              39/63|                        14/16|
|Before FDR               |0 hr      |    28|  -0.48 (0.01)|              20/28|                          8/8|
|Before FDR               |1 hr      |    60| -0.31 (0.015)|              31/60|                        13/13|
|Before FDR               |6 hr      |    39| -0.37 (0.021)|              29/39|                        12/12|
|After FDR                |0 hr      |     5|  -0.47 (0.43)|                4/5|                          3/3|
|After FDR                |1 hr      |     4|  -0.83 (0.17)|                4/4|                          4/4|
|After FDR                |6 hr      |     5|  -0.93 (0.02)|                5/5|                          4/4|

**Sign consistency** (pairs with GTEx p < 0.05; the binomial p-values are exploratory)

|Set                      |Timepoint                      | Pairs| Consistent| Consistent (%)| Binomial p, two-sided| Binomial p, one-sided|
|:------------------------|:------------------------------|-----:|----------:|--------------:|---------------------:|---------------------:|
|isoLASER cis, het donors |0 hr                           |    14|         14|            100|               0.00012|               6.1e-05|
|isoLASER cis, het donors |1 hr                           |    31|         21|             68|                 0.071|                 0.035|
|isoLASER cis, het donors |6 hr                           |    28|         21|             75|                 0.013|                0.0063|
|isoLASER cis, het donors |All timepoints, each pair once |    51|         35|             69|                 0.011|                0.0055|
|Before FDR               |0 hr                           |    11|         11|            100|               0.00098|               0.00049|
|Before FDR               |1 hr                           |    20|         15|             75|                 0.041|                 0.021|
|Before FDR               |6 hr                           |    21|         18|             86|                0.0015|               0.00074|
|Before FDR               |All timepoints, each pair once |    38|         30|             79|               0.00047|               0.00024|
|After FDR                |0 hr                           |     3|          3|            100|                  0.25|                  0.12|
|After FDR                |1 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |6 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |All timepoints, each pair once |     5|          5|            100|                 0.062|                 0.031|

### Putamen basal ganglia

**Pairs matched**

|Set                      |Timepoint | Our associations (SNVs)| Same variant and gene tested in GTEx| Plotted pairs| Genes|
|:------------------------|:---------|-----------------------:|------------------------------------:|-------------:|-----:|
|isoLASER cis, het donors |0 hr      |                     355|                                  306|            38|    26|
|isoLASER cis, het donors |1 hr      |                     656|                                  542|            83|    55|
|isoLASER cis, het donors |6 hr      |                     716|                                  586|            61|    40|
|Before FDR               |0 hr      |                     194|                                  172|            24|    18|
|Before FDR               |1 hr      |                     359|                                  333|            57|    39|
|Before FDR               |6 hr      |                     403|                                  361|            36|    26|
|After FDR                |0 hr      |                      21|                                   20|             5|     4|
|After FDR                |1 hr      |                      27|                                   26|             4|     3|
|After FDR                |6 hr      |                      39|                                   33|             5|     4|

**Correlation**

|Set                      |Timepoint | Pairs|     All: R (p)| All: expected sign| GTEx p < 1e-5: expected sign|
|:------------------------|:---------|-----:|--------------:|------------------:|----------------------------:|
|isoLASER cis, het donors |0 hr      |    38|   -0.24 (0.16)|              24/38|                          4/5|
|isoLASER cis, het donors |1 hr      |    83|  -0.26 (0.018)|              50/83|                        13/15|
|isoLASER cis, het donors |6 hr      |    61|  -0.29 (0.023)|              35/61|                         8/10|
|Before FDR               |0 hr      |    24| -0.57 (0.0038)|              18/24|                          2/2|
|Before FDR               |1 hr      |    57| -0.38 (0.0037)|              34/57|                        10/10|
|Before FDR               |6 hr      |    36|  -0.42 (0.011)|              28/36|                          6/6|
|After FDR                |0 hr      |     5|   -0.42 (0.48)|                5/5|                          2/2|
|After FDR                |1 hr      |     4|  -0.93 (0.067)|                4/4|                          3/3|
|After FDR                |6 hr      |     5| -0.97 (0.0068)|                5/5|                          3/3|

**Sign consistency** (pairs with GTEx p < 0.05; the binomial p-values are exploratory)

|Set                      |Timepoint                      | Pairs| Consistent| Consistent (%)| Binomial p, two-sided| Binomial p, one-sided|
|:------------------------|:------------------------------|-----:|----------:|--------------:|---------------------:|---------------------:|
|isoLASER cis, het donors |0 hr                           |    11|         11|            100|               0.00098|               0.00049|
|isoLASER cis, het donors |1 hr                           |    33|         24|             73|                 0.014|                0.0068|
|isoLASER cis, het donors |6 hr                           |    21|         15|             71|                 0.078|                 0.039|
|isoLASER cis, het donors |All timepoints, each pair once |    47|         33|             70|                0.0079|                 0.004|
|Before FDR               |0 hr                           |     9|          9|            100|                0.0039|                 0.002|
|Before FDR               |1 hr                           |    25|         20|             80|                0.0041|                 0.002|
|Before FDR               |6 hr                           |    14|         13|             93|                0.0018|               0.00092|
|Before FDR               |All timepoints, each pair once |    36|         30|             83|                 7e-05|               3.5e-05|
|After FDR                |0 hr                           |     3|          3|            100|                  0.25|                  0.12|
|After FDR                |1 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |6 hr                           |     4|          4|            100|                  0.12|                 0.062|
|After FDR                |All timepoints, each pair once |     5|          5|            100|                 0.062|                 0.031|

## Summary across tissues


|Tissue                          | isoLASER cis, het donors|      Before FDR|   After FDR|
|:-------------------------------|------------------------:|---------------:|-----------:|
|Cerebellum                      |            38/61 (0.036)|  31/44 (0.0048)| 5/5 (0.031)|
|Cerebellar Hemisphere           |           39/57 (0.0038)| 31/40 (0.00034)| 5/5 (0.031)|
|Caudate basal ganglia           |           37/52 (0.0016)| 31/36 (6.5e-06)| 5/5 (0.031)|
|Cortex                          |          42/54 (2.6e-05)| 37/42 (2.2e-07)| 5/5 (0.031)|
|Frontal Cortex BA9              |           36/54 (0.0099)| 31/39 (0.00015)| 5/5 (0.031)|
|Hippocampus                     |           38/54 (0.0019)| 32/40 (9.1e-05)|  5/6 (0.11)|
|Hypothalamus                    |           34/47 (0.0015)| 30/36 (3.5e-05)| 5/5 (0.031)|
|Nucleus accumbens basal ganglia |           35/51 (0.0055)| 30/38 (0.00024)| 5/5 (0.031)|
|Putamen basal ganglia           |            33/47 (0.004)| 30/36 (3.5e-05)| 5/5 (0.031)|

Sign consistency with each pair once, by tissue: consistent pairs / pairs with
GTEx p < 0.05, with the one-sided binomial p (exploratory; see
[How the testing works](#how-the-testing-works)). Across the nine tissues, the share of consistent pairs is
62&ndash;78% for the cis set, 70&ndash;88% before FDR and 83&ndash;100% after FDR. The tissues share many
GTEx donors, so they are not independent replications.

Download the [points](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_points.tsv),
[correlation statistics](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_stats.tsv),
[sign consistency](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_consistency.tsv) and
[matching counts](assets/isolaser_gtex_reads10nc_q010_hetcis/brain_tissues_funnel.tsv).

Reproduce with `long_read_RNA/10.isolaser_permutation/`:
`27.gtex_fdr_comparison.py --prepare-full-cerebellum --cis-het`,
`... --min-dpsi 0.05 --before-fdr` and
`... --min-dpsi 0.05 --max-q 0.10` (`ADAPTIVE_RULE=reads10nc`) for the three
sets; then `56.gtex_brain_tissues.sbatch` (extraction, one task per tissue), and
with `AFTER_Q=0.10` and `PAPER_SET=hetcis`: `55.gtex_brain_tissues.R summarize`, `58.gtex_pi1.R` and
`57.gtex_gene_venn.R`. 

# Estimated non-null proportion among GTEx-matched associations (Storey's &pi;<sub>1</sub>) {.tabset}



For each association in the cis and before-FDR sets, we take the GTEx
p-value of its event's skipping junction for our SNV, as in the scatter plots, and
estimate Storey's π<sub>1</sub> from these p-values, for each timepoint separately.
When GTEx tests several skipping junctions of the event (2% of matched
associations), we use the one shared by the most annotated transcripts that skip
the part, chosen without looking at GTEx p-values. This is exploratory.

**What it estimates:** GTEx p-values of associations with no effect in GTEx are
spread evenly between 0 and 1, and real effects tend to produce smaller p-values
when GTEx has sufficient power. The estimator measures the flat part,
π<sub>0</sub>, from the larger p-values, and π<sub>1</sub> = 1 − π<sub>0</sub> is
the estimated proportion of non-null associations among matched GTEx tests.
Limited power can make weak non-null effects look null and underestimate
π<sub>1</sub>, so π<sub>1</sub> cannot distinguish false positives in our study
from context-specific effects or effects that GTEx has insufficient power to
detect. It also ignores direction, which is checked under [Testing](#testing).

**After FDR:** only 4&ndash;6 associations are matched per tissue and
timepoint, too few for a stable π<sub>1</sub>: one p-value crossing 0.5 moves it
by 2/n, 0.50 at n = 4. Each tab lists them
instead, with their GTEx p-value and direction. **Expected direction** means
GTEx's beta has the opposite sign to our ΔPSI at every timepoint where the
association is reported, as in the sign-consistency test.

## Cerebellum

**&pi;<sub>1</sub>: cis set and before FDR**

|Set                      |Timepoint | Associations| Matched in GTEx| GTEx p < 0.05| &pi;<sub>1</sub>|Estimator      |
|:------------------------|:---------|------------:|---------------:|-------------:|----------------:|:--------------|
|isoLASER cis, het donors |0 hr      |          355|              37|           51%|             0.46|&lambda; = 0.5 |
|isoLASER cis, het donors |1 hr      |          656|              83|           49%|             0.77|smoother       |
|isoLASER cis, het donors |6 hr      |          716|              64|           41%|             0.31|smoother       |
|Before FDR               |0 hr      |          194|              24|           54%|             0.42|&lambda; = 0.5 |
|Before FDR               |1 hr      |          359|              57|           47%|             0.65|smoother       |
|Before FDR               |6 hr      |          403|              39|           41%|             0.22|smoother       |

**Estimator**: how `qvalue::pi0est` estimated &pi;<sub>0</sub>. **smoother** (its default, used with 30 or more p-values): &pi;<sub>0</sub> is computed at each &lambda; from 0.05 to 0.95 as #(p &gt; &lambda;) / (n(1 &minus; &lambda;)), the share of p-values above &lambda; scaled to the whole range; a spline is fitted through these values and read at &lambda; = 0.95. **&lambda; = 0.5** (fewer than 30 p-values, too few for the spline): &pi;<sub>1</sub> = max(0, 1 &minus; #(p &gt; 0.5) / (0.5 n)), so one p-value moves it by 2/n.

**After FDR: each matched association**

Matched at 0, 1 and 6 hr: 5 of 21, 4 of 27 and 5 of 39 associations. Of the 8 distinct ones, 5 have GTEx p < 0.05, 5 of them in the expected direction.

|Gene     |Variant             |Exonic part                 |Reported at      |          &Delta;PSI|  GTEx p| GTEx beta|Expected direction |
|:--------|:-------------------|:---------------------------|:----------------|-------------------:|-------:|---------:|:------------------|
|HNRNPK   |chr9:83980154:C>T   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.21, -0.22, -0.27| 8.2e-27|     +0.97|yes                |
|HNRNPK   |chr9:83978398:G>C   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.12, -0.11, -0.16| 3.2e-21|     +0.92|yes                |
|PPA2     |chr4:105396271:C>G  |chr4:105438014-105438036:-  |1 hr             |               +0.46| 1.1e-19|     -0.86|yes                |
|SNHG5    |chr6:85678169:G>T   |chr6:85677794-85677868:-    |6 hr             |               +0.38| 8.9e-15|     -0.69|yes                |
|ATP5MJ   |chr14:103915164:T>C |chr14:103914478-103914633:- |0 hr, 1 hr, 6 hr | +0.09, +0.10, +0.09| 6.2e-11|     -1.02|yes                |
|ASRGL1   |chr11:62337539:T>G  |chr11:62356324-62356467:+   |0 hr             |               -0.44|     0.3|     +0.10|yes                |
|C11orf58 |chr11:16755584:T>G  |chr11:16748096-16748157:+   |6 hr             |               -0.07|    0.34|     +0.04|yes                |
|DGCR6L   |chr22:20319732:G>A  |chr22:20316118-20316219:-   |0 hr             |               -0.10|    0.91|     +0.00|yes                |

## Cerebellar Hemisphere

**&pi;<sub>1</sub>: cis set and before FDR**

|Set                      |Timepoint | Associations| Matched in GTEx| GTEx p < 0.05| &pi;<sub>1</sub>|Estimator      |
|:------------------------|:---------|------------:|---------------:|-------------:|----------------:|:--------------|
|isoLASER cis, het donors |0 hr      |          355|              40|           42%|             0.32|smoother       |
|isoLASER cis, het donors |1 hr      |          656|              82|           41%|             0.00|smoother       |
|isoLASER cis, het donors |6 hr      |          716|              68|           41%|             0.24|smoother       |
|Before FDR               |0 hr      |          194|              26|           50%|             0.38|&lambda; = 0.5 |
|Before FDR               |1 hr      |          359|              57|           37%|             0.16|smoother       |
|Before FDR               |6 hr      |          403|              41|           46%|             0.51|&lambda; = 0.5 |

**Estimator**: how `qvalue::pi0est` estimated &pi;<sub>0</sub>. **smoother** (its default, used with 30 or more p-values): &pi;<sub>0</sub> is computed at each &lambda; from 0.05 to 0.95 as #(p &gt; &lambda;) / (n(1 &minus; &lambda;)), the share of p-values above &lambda; scaled to the whole range; a spline is fitted through these values and read at &lambda; = 0.95. **&lambda; = 0.5** (fewer than 30 p-values, too few for the spline): &pi;<sub>1</sub> = max(0, 1 &minus; #(p &gt; 0.5) / (0.5 n)), so one p-value moves it by 2/n.

**After FDR: each matched association**

Matched at 0, 1 and 6 hr: 5 of 21, 4 of 27 and 5 of 39 associations. Of the 8 distinct ones, 5 have GTEx p < 0.05, 5 of them in the expected direction.

|Gene     |Variant             |Exonic part                 |Reported at      |          &Delta;PSI|  GTEx p| GTEx beta|Expected direction |
|:--------|:-------------------|:---------------------------|:----------------|-------------------:|-------:|---------:|:------------------|
|HNRNPK   |chr9:83980154:C>T   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.21, -0.22, -0.27| 2.2e-22|     +0.97|yes                |
|PPA2     |chr4:105396271:C>G  |chr4:105438014-105438036:-  |1 hr             |               +0.46| 1.4e-19|     -0.86|yes                |
|HNRNPK   |chr9:83978398:G>C   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.12, -0.11, -0.16|   4e-18|     +0.92|yes                |
|SNHG5    |chr6:85678169:G>T   |chr6:85677794-85677868:-    |6 hr             |               +0.38| 8.2e-15|     -0.78|yes                |
|ATP5MJ   |chr14:103915164:T>C |chr14:103914478-103914633:- |0 hr, 1 hr, 6 hr | +0.09, +0.10, +0.09| 1.3e-11|     -1.06|yes                |
|ASRGL1   |chr11:62337539:T>G  |chr11:62356324-62356467:+   |0 hr             |               -0.44|   0.082|     +0.17|yes                |
|DGCR6L   |chr22:20319732:G>A  |chr22:20316118-20316219:-   |0 hr             |               -0.10|    0.25|     +0.04|yes                |
|C11orf58 |chr11:16755584:T>G  |chr11:16748096-16748157:+   |6 hr             |               -0.07|    0.38|     -0.03|no                 |

## Caudate basal ganglia

**&pi;<sub>1</sub>: cis set and before FDR**

|Set                      |Timepoint | Associations| Matched in GTEx| GTEx p < 0.05| &pi;<sub>1</sub>|Estimator      |
|:------------------------|:---------|------------:|---------------:|-------------:|----------------:|:--------------|
|isoLASER cis, het donors |0 hr      |          355|              38|           45%|             0.63|&lambda; = 0.5 |
|isoLASER cis, het donors |1 hr      |          656|              85|           41%|             0.64|smoother       |
|isoLASER cis, het donors |6 hr      |          716|              60|           38%|             0.40|&lambda; = 0.5 |
|Before FDR               |0 hr      |          194|              24|           46%|             0.50|&lambda; = 0.5 |
|Before FDR               |1 hr      |          359|              59|           39%|             0.47|smoother       |
|Before FDR               |6 hr      |          403|              35|           40%|             0.31|&lambda; = 0.5 |

**Estimator**: how `qvalue::pi0est` estimated &pi;<sub>0</sub>. **smoother** (its default, used with 30 or more p-values): &pi;<sub>0</sub> is computed at each &lambda; from 0.05 to 0.95 as #(p &gt; &lambda;) / (n(1 &minus; &lambda;)), the share of p-values above &lambda; scaled to the whole range; a spline is fitted through these values and read at &lambda; = 0.95. **&lambda; = 0.5** (fewer than 30 p-values, too few for the spline): &pi;<sub>1</sub> = max(0, 1 &minus; #(p &gt; 0.5) / (0.5 n)), so one p-value moves it by 2/n.

**After FDR: each matched association**

Matched at 0, 1 and 6 hr: 5 of 21, 4 of 27 and 5 of 39 associations. Of the 8 distinct ones, 5 have GTEx p < 0.05, 5 of them in the expected direction.

|Gene     |Variant             |Exonic part                 |Reported at      |          &Delta;PSI|  GTEx p| GTEx beta|Expected direction |
|:--------|:-------------------|:---------------------------|:----------------|-------------------:|-------:|---------:|:------------------|
|SNHG5    |chr6:85678169:G>T   |chr6:85677794-85677868:-    |6 hr             |               +0.38|   1e-33|     -1.00|yes                |
|PPA2     |chr4:105396271:C>G  |chr4:105438014-105438036:-  |1 hr             |               +0.46| 1.3e-15|     -0.77|yes                |
|HNRNPK   |chr9:83980154:C>T   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.21, -0.22, -0.27|   8e-07|     +0.50|yes                |
|ATP5MJ   |chr14:103915164:T>C |chr14:103914478-103914633:- |0 hr, 1 hr, 6 hr | +0.09, +0.10, +0.09| 1.1e-06|     -0.79|yes                |
|HNRNPK   |chr9:83978398:G>C   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.12, -0.11, -0.16| 2.6e-05|     +0.46|yes                |
|ASRGL1   |chr11:62337539:T>G  |chr11:62356324-62356467:+   |0 hr             |               -0.44|    0.39|     +0.09|yes                |
|DGCR6L   |chr22:20319732:G>A  |chr22:20316118-20316219:-   |0 hr             |               -0.10|    0.66|     +0.02|yes                |
|C11orf58 |chr11:16755584:T>G  |chr11:16748096-16748157:+   |6 hr             |               -0.07|    0.93|     +0.01|yes                |

## Cortex

**&pi;<sub>1</sub>: cis set and before FDR**

|Set                      |Timepoint | Associations| Matched in GTEx| GTEx p < 0.05| &pi;<sub>1</sub>|Estimator      |
|:------------------------|:---------|------------:|---------------:|-------------:|----------------:|:--------------|
|isoLASER cis, het donors |0 hr      |          355|              39|           51%|             0.44|&lambda; = 0.5 |
|isoLASER cis, het donors |1 hr      |          656|              80|           41%|             0.00|smoother       |
|isoLASER cis, het donors |6 hr      |          716|              61|           41%|             0.01|smoother       |
|Before FDR               |0 hr      |          194|              26|           58%|             0.46|&lambda; = 0.5 |
|Before FDR               |1 hr      |          359|              57|           42%|             0.00|smoother       |
|Before FDR               |6 hr      |          403|              37|           46%|             0.45|smoother       |

**Estimator**: how `qvalue::pi0est` estimated &pi;<sub>0</sub>. **smoother** (its default, used with 30 or more p-values): &pi;<sub>0</sub> is computed at each &lambda; from 0.05 to 0.95 as #(p &gt; &lambda;) / (n(1 &minus; &lambda;)), the share of p-values above &lambda; scaled to the whole range; a spline is fitted through these values and read at &lambda; = 0.95. **&lambda; = 0.5** (fewer than 30 p-values, too few for the spline): &pi;<sub>1</sub> = max(0, 1 &minus; #(p &gt; 0.5) / (0.5 n)), so one p-value moves it by 2/n.

**After FDR: each matched association**

Matched at 0, 1 and 6 hr: 6 of 21, 4 of 27 and 5 of 39 associations. Of the 9 distinct ones, 5 have GTEx p < 0.05, 5 of them in the expected direction.

|Gene     |Variant             |Exonic part                 |Reported at      |          &Delta;PSI|  GTEx p| GTEx beta|Expected direction |
|:--------|:-------------------|:---------------------------|:----------------|-------------------:|-------:|---------:|:------------------|
|SNHG5    |chr6:85678169:G>T   |chr6:85677794-85677868:-    |6 hr             |               +0.38| 2.2e-33|     -1.06|yes                |
|PPA2     |chr4:105396271:C>G  |chr4:105438014-105438036:-  |1 hr             |               +0.46| 5.8e-19|     -0.78|yes                |
|HNRNPK   |chr9:83978398:G>C   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.12, -0.11, -0.16| 3.3e-14|     +0.68|yes                |
|HNRNPK   |chr9:83980154:C>T   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.21, -0.22, -0.27|   8e-14|     +0.64|yes                |
|ATP5MJ   |chr14:103915164:T>C |chr14:103914478-103914633:- |0 hr, 1 hr, 6 hr | +0.09, +0.10, +0.09| 1.8e-10|     -1.03|yes                |
|C11orf58 |chr11:16755584:T>G  |chr11:16748096-16748157:+   |6 hr             |               -0.07|    0.19|     +0.08|yes                |
|ASRGL1   |chr11:62337539:T>G  |chr11:62356324-62356467:+   |0 hr             |               -0.44|    0.36|     +0.09|yes                |
|DGCR6L   |chr22:20319732:G>A  |chr22:20316118-20316219:-   |0 hr             |               -0.10|    0.87|     -0.01|no                 |
|HM13     |chr20:31569222:A>G  |chr20:31547606-31547692:+   |0 hr             |               +0.37|    0.88|     -0.02|yes                |

## Frontal Cortex BA9

**&pi;<sub>1</sub>: cis set and before FDR**

|Set                      |Timepoint | Associations| Matched in GTEx| GTEx p < 0.05| &pi;<sub>1</sub>|Estimator      |
|:------------------------|:---------|------------:|---------------:|-------------:|----------------:|:--------------|
|isoLASER cis, het donors |0 hr      |          355|              39|           41%|             0.38|&lambda; = 0.5 |
|isoLASER cis, het donors |1 hr      |          656|              83|           42%|             0.46|smoother       |
|isoLASER cis, het donors |6 hr      |          716|              63|           41%|             0.50|smoother       |
|Before FDR               |0 hr      |          194|              25|           44%|             0.28|&lambda; = 0.5 |
|Before FDR               |1 hr      |          359|              58|           41%|             0.48|smoother       |
|Before FDR               |6 hr      |          403|              39|           44%|             0.37|smoother       |

**Estimator**: how `qvalue::pi0est` estimated &pi;<sub>0</sub>. **smoother** (its default, used with 30 or more p-values): &pi;<sub>0</sub> is computed at each &lambda; from 0.05 to 0.95 as #(p &gt; &lambda;) / (n(1 &minus; &lambda;)), the share of p-values above &lambda; scaled to the whole range; a spline is fitted through these values and read at &lambda; = 0.95. **&lambda; = 0.5** (fewer than 30 p-values, too few for the spline): &pi;<sub>1</sub> = max(0, 1 &minus; #(p &gt; 0.5) / (0.5 n)), so one p-value moves it by 2/n.

**After FDR: each matched association**

Matched at 0, 1 and 6 hr: 5 of 21, 4 of 27 and 5 of 39 associations. Of the 8 distinct ones, 5 have GTEx p < 0.05, 5 of them in the expected direction.

|Gene     |Variant             |Exonic part                 |Reported at      |          &Delta;PSI|  GTEx p| GTEx beta|Expected direction |
|:--------|:-------------------|:---------------------------|:----------------|-------------------:|-------:|---------:|:------------------|
|SNHG5    |chr6:85678169:G>T   |chr6:85677794-85677868:-    |6 hr             |               +0.38| 6.9e-29|     -1.06|yes                |
|HNRNPK   |chr9:83980154:C>T   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.21, -0.22, -0.27| 3.2e-15|     +0.74|yes                |
|PPA2     |chr4:105396271:C>G  |chr4:105438014-105438036:-  |1 hr             |               +0.46|   6e-15|     -0.83|yes                |
|HNRNPK   |chr9:83978398:G>C   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.12, -0.11, -0.16| 1.4e-12|     +0.72|yes                |
|ATP5MJ   |chr14:103915164:T>C |chr14:103914478-103914633:- |0 hr, 1 hr, 6 hr | +0.09, +0.10, +0.09| 6.5e-07|     -0.81|yes                |
|C11orf58 |chr11:16755584:T>G  |chr11:16748096-16748157:+   |6 hr             |               -0.07|    0.29|     +0.05|yes                |
|ASRGL1   |chr11:62337539:T>G  |chr11:62356324-62356467:+   |0 hr             |               -0.44|    0.46|     +0.08|yes                |
|DGCR6L   |chr22:20319732:G>A  |chr22:20316118-20316219:-   |0 hr             |               -0.10|    0.69|     -0.02|no                 |

## Hippocampus

**&pi;<sub>1</sub>: cis set and before FDR**

|Set                      |Timepoint | Associations| Matched in GTEx| GTEx p < 0.05| &pi;<sub>1</sub>|Estimator      |
|:------------------------|:---------|------------:|---------------:|-------------:|----------------:|:--------------|
|isoLASER cis, het donors |0 hr      |          355|              40|           45%|             0.75|&lambda; = 0.5 |
|isoLASER cis, het donors |1 hr      |          656|              84|           39%|             0.41|smoother       |
|isoLASER cis, het donors |6 hr      |          716|              65|           40%|             0.64|smoother       |
|Before FDR               |0 hr      |          194|              25|           48%|             0.76|&lambda; = 0.5 |
|Before FDR               |1 hr      |          359|              58|           40%|             0.47|smoother       |
|Before FDR               |6 hr      |          403|              38|           47%|             0.58|&lambda; = 0.5 |

**Estimator**: how `qvalue::pi0est` estimated &pi;<sub>0</sub>. **smoother** (its default, used with 30 or more p-values): &pi;<sub>0</sub> is computed at each &lambda; from 0.05 to 0.95 as #(p &gt; &lambda;) / (n(1 &minus; &lambda;)), the share of p-values above &lambda; scaled to the whole range; a spline is fitted through these values and read at &lambda; = 0.95. **&lambda; = 0.5** (fewer than 30 p-values, too few for the spline): &pi;<sub>1</sub> = max(0, 1 &minus; #(p &gt; 0.5) / (0.5 n)), so one p-value moves it by 2/n.

**After FDR: each matched association**

Matched at 0, 1 and 6 hr: 5 of 21, 4 of 27 and 5 of 39 associations. Of the 8 distinct ones, 6 have GTEx p < 0.05, 5 of them in the expected direction.

|Gene     |Variant             |Exonic part                 |Reported at      |          &Delta;PSI|  GTEx p| GTEx beta|Expected direction |
|:--------|:-------------------|:---------------------------|:----------------|-------------------:|-------:|---------:|:------------------|
|SNHG5    |chr6:85678169:G>T   |chr6:85677794-85677868:-    |6 hr             |               +0.38| 3.1e-29|     -1.05|yes                |
|PPA2     |chr4:105396271:C>G  |chr4:105438014-105438036:-  |1 hr             |               +0.46| 7.3e-10|     -0.65|yes                |
|HNRNPK   |chr9:83980154:C>T   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.21, -0.22, -0.27| 2.2e-05|     +0.51|yes                |
|ATP5MJ   |chr14:103915164:T>C |chr14:103914478-103914633:- |0 hr, 1 hr, 6 hr | +0.09, +0.10, +0.09| 3.2e-05|     -0.67|yes                |
|HNRNPK   |chr9:83978398:G>C   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.12, -0.11, -0.16| 0.00012|     +0.48|yes                |
|DGCR6L   |chr22:20319732:G>A  |chr22:20316118-20316219:-   |0 hr             |               -0.10|   0.044|     -0.11|no                 |
|C11orf58 |chr11:16755584:T>G  |chr11:16748096-16748157:+   |6 hr             |               -0.07|     0.1|     +0.09|yes                |
|ASRGL1   |chr11:62337539:T>G  |chr11:62356324-62356467:+   |0 hr             |               -0.44|    0.43|     -0.07|no                 |

## Hypothalamus

**&pi;<sub>1</sub>: cis set and before FDR**

|Set                      |Timepoint | Associations| Matched in GTEx| GTEx p < 0.05| &pi;<sub>1</sub>|Estimator      |
|:------------------------|:---------|------------:|---------------:|-------------:|----------------:|:--------------|
|isoLASER cis, het donors |0 hr      |          355|              39|           41%|             0.23|smoother       |
|isoLASER cis, het donors |1 hr      |          656|              81|           38%|             0.62|smoother       |
|isoLASER cis, het donors |6 hr      |          716|              62|           35%|             0.50|smoother       |
|Before FDR               |0 hr      |          194|              26|           46%|             0.38|&lambda; = 0.5 |
|Before FDR               |1 hr      |          359|              59|           37%|             0.54|smoother       |
|Before FDR               |6 hr      |          403|              37|           38%|             0.51|&lambda; = 0.5 |

**Estimator**: how `qvalue::pi0est` estimated &pi;<sub>0</sub>. **smoother** (its default, used with 30 or more p-values): &pi;<sub>0</sub> is computed at each &lambda; from 0.05 to 0.95 as #(p &gt; &lambda;) / (n(1 &minus; &lambda;)), the share of p-values above &lambda; scaled to the whole range; a spline is fitted through these values and read at &lambda; = 0.95. **&lambda; = 0.5** (fewer than 30 p-values, too few for the spline): &pi;<sub>1</sub> = max(0, 1 &minus; #(p &gt; 0.5) / (0.5 n)), so one p-value moves it by 2/n.

**After FDR: each matched association**

Matched at 0, 1 and 6 hr: 6 of 21, 4 of 27 and 5 of 39 associations. Of the 9 distinct ones, 5 have GTEx p < 0.05, 5 of them in the expected direction.

|Gene     |Variant             |Exonic part                 |Reported at      |          &Delta;PSI|  GTEx p| GTEx beta|Expected direction |
|:--------|:-------------------|:---------------------------|:----------------|-------------------:|-------:|---------:|:------------------|
|SNHG5    |chr6:85678169:G>T   |chr6:85677794-85677868:-    |6 hr             |               +0.38| 9.9e-27|     -0.98|yes                |
|PPA2     |chr4:105396271:C>G  |chr4:105438014-105438036:-  |1 hr             |               +0.46| 4.2e-12|     -0.71|yes                |
|HNRNPK   |chr9:83980154:C>T   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.21, -0.22, -0.27| 8.3e-10|     +0.70|yes                |
|HNRNPK   |chr9:83978398:G>C   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.12, -0.11, -0.16| 1.2e-09|     +0.72|yes                |
|ATP5MJ   |chr14:103915164:T>C |chr14:103914478-103914633:- |0 hr, 1 hr, 6 hr | +0.09, +0.10, +0.09|   0.034|     -0.40|yes                |
|ASRGL1   |chr11:62337539:T>G  |chr11:62356324-62356467:+   |0 hr             |               -0.44|    0.11|     +0.16|yes                |
|C11orf58 |chr11:16755584:T>G  |chr11:16748096-16748157:+   |6 hr             |               -0.07|    0.12|     +0.11|yes                |
|HM13     |chr20:31569222:A>G  |chr20:31547606-31547692:+   |0 hr             |               +0.37|    0.52|     -0.08|yes                |
|DGCR6L   |chr22:20319732:G>A  |chr22:20316118-20316219:-   |0 hr             |               -0.10|    0.71|     +0.02|yes                |

## Nucleus accumbens basal ganglia

**&pi;<sub>1</sub>: cis set and before FDR**

|Set                      |Timepoint | Associations| Matched in GTEx| GTEx p < 0.05| &pi;<sub>1</sub>|Estimator      |
|:------------------------|:---------|------------:|---------------:|-------------:|----------------:|:--------------|
|isoLASER cis, het donors |0 hr      |          355|              40|           38%|             0.24|smoother       |
|isoLASER cis, het donors |1 hr      |          656|              86|           36%|             0.64|smoother       |
|isoLASER cis, het donors |6 hr      |          716|              62|           45%|             0.73|smoother       |
|Before FDR               |0 hr      |          194|              26|           42%|             0.46|&lambda; = 0.5 |
|Before FDR               |1 hr      |          359|              60|           33%|             0.70|&lambda; = 0.5 |
|Before FDR               |6 hr      |          403|              38|           55%|             0.63|&lambda; = 0.5 |

**Estimator**: how `qvalue::pi0est` estimated &pi;<sub>0</sub>. **smoother** (its default, used with 30 or more p-values): &pi;<sub>0</sub> is computed at each &lambda; from 0.05 to 0.95 as #(p &gt; &lambda;) / (n(1 &minus; &lambda;)), the share of p-values above &lambda; scaled to the whole range; a spline is fitted through these values and read at &lambda; = 0.95. **&lambda; = 0.5** (fewer than 30 p-values, too few for the spline): &pi;<sub>1</sub> = max(0, 1 &minus; #(p &gt; 0.5) / (0.5 n)), so one p-value moves it by 2/n.

**After FDR: each matched association**

Matched at 0, 1 and 6 hr: 5 of 21, 4 of 27 and 5 of 39 associations. Of the 8 distinct ones, 5 have GTEx p < 0.05, 5 of them in the expected direction.

|Gene     |Variant             |Exonic part                 |Reported at      |          &Delta;PSI|  GTEx p| GTEx beta|Expected direction |
|:--------|:-------------------|:---------------------------|:----------------|-------------------:|-------:|---------:|:------------------|
|SNHG5    |chr6:85678169:G>T   |chr6:85677794-85677868:-    |6 hr             |               +0.38| 1.4e-38|     -1.14|yes                |
|PPA2     |chr4:105396271:C>G  |chr4:105438014-105438036:-  |1 hr             |               +0.46| 2.8e-17|     -0.79|yes                |
|HNRNPK   |chr9:83980154:C>T   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.21, -0.22, -0.27| 8.6e-14|     +0.76|yes                |
|ATP5MJ   |chr14:103915164:T>C |chr14:103914478-103914633:- |0 hr, 1 hr, 6 hr | +0.09, +0.10, +0.09| 1.7e-10|     -0.94|yes                |
|HNRNPK   |chr9:83978398:G>C   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.12, -0.11, -0.16| 3.3e-10|     +0.69|yes                |
|C11orf58 |chr11:16755584:T>G  |chr11:16748096-16748157:+   |6 hr             |               -0.07|    0.45|     +0.06|yes                |
|DGCR6L   |chr22:20319732:G>A  |chr22:20316118-20316219:-   |0 hr             |               -0.10|     0.8|     -0.01|no                 |
|ASRGL1   |chr11:62337539:T>G  |chr11:62356324-62356467:+   |0 hr             |               -0.44|       1|     +0.00|yes                |

## Putamen basal ganglia

**&pi;<sub>1</sub>: cis set and before FDR**

|Set                      |Timepoint | Associations| Matched in GTEx| GTEx p < 0.05| &pi;<sub>1</sub>|Estimator      |
|:------------------------|:---------|------------:|---------------:|-------------:|----------------:|:--------------|
|isoLASER cis, het donors |0 hr      |          355|              38|           32%|             0.08|smoother       |
|isoLASER cis, het donors |1 hr      |          656|              83|           40%|             0.60|smoother       |
|isoLASER cis, het donors |6 hr      |          716|              60|           35%|             0.38|smoother       |
|Before FDR               |0 hr      |          194|              24|           38%|             0.42|&lambda; = 0.5 |
|Before FDR               |1 hr      |          359|              57|           44%|             0.47|&lambda; = 0.5 |
|Before FDR               |6 hr      |          403|              35|           40%|             0.59|smoother       |

**Estimator**: how `qvalue::pi0est` estimated &pi;<sub>0</sub>. **smoother** (its default, used with 30 or more p-values): &pi;<sub>0</sub> is computed at each &lambda; from 0.05 to 0.95 as #(p &gt; &lambda;) / (n(1 &minus; &lambda;)), the share of p-values above &lambda; scaled to the whole range; a spline is fitted through these values and read at &lambda; = 0.95. **&lambda; = 0.5** (fewer than 30 p-values, too few for the spline): &pi;<sub>1</sub> = max(0, 1 &minus; #(p &gt; 0.5) / (0.5 n)), so one p-value moves it by 2/n.

**After FDR: each matched association**

Matched at 0, 1 and 6 hr: 5 of 21, 4 of 27 and 5 of 39 associations. Of the 8 distinct ones, 5 have GTEx p < 0.05, 5 of them in the expected direction.

|Gene     |Variant             |Exonic part                 |Reported at      |          &Delta;PSI|  GTEx p| GTEx beta|Expected direction |
|:--------|:-------------------|:---------------------------|:----------------|-------------------:|-------:|---------:|:------------------|
|SNHG5    |chr6:85678169:G>T   |chr6:85677794-85677868:-    |6 hr             |               +0.38| 5.3e-29|     -1.03|yes                |
|PPA2     |chr4:105396271:C>G  |chr4:105438014-105438036:-  |1 hr             |               +0.46| 4.9e-16|     -0.88|yes                |
|HNRNPK   |chr9:83978398:G>C   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.12, -0.11, -0.16| 1.6e-07|     +0.56|yes                |
|HNRNPK   |chr9:83980154:C>T   |chr9:83980118-83980152:-    |0 hr, 1 hr, 6 hr | -0.21, -0.22, -0.27| 2.1e-06|     +0.49|yes                |
|ATP5MJ   |chr14:103915164:T>C |chr14:103914478-103914633:- |0 hr, 1 hr, 6 hr | +0.09, +0.10, +0.09|   0.001|     -0.53|yes                |
|DGCR6L   |chr22:20319732:G>A  |chr22:20316118-20316219:-   |0 hr             |               -0.10|    0.49|     +0.04|yes                |
|C11orf58 |chr11:16755584:T>G  |chr11:16748096-16748157:+   |6 hr             |               -0.07|    0.73|     +0.03|yes                |
|ASRGL1   |chr11:62337539:T>G  |chr11:62356324-62356467:+   |0 hr             |               -0.44|    0.82|     +0.03|yes                |

## Summary across tissues


|Set                      |Timepoint | Matched in GTEx| &pi;<sub>1</sub>|
|:------------------------|:---------|---------------:|----------------:|
|isoLASER cis, het donors |0 hr      |     37&ndash;40|  0.08&ndash;0.75|
|isoLASER cis, het donors |1 hr      |     80&ndash;86|  0.00&ndash;0.77|
|isoLASER cis, het donors |6 hr      |     60&ndash;68|  0.01&ndash;0.73|
|Before FDR               |0 hr      |     24&ndash;26|  0.28&ndash;0.76|
|Before FDR               |1 hr      |     57&ndash;60|  0.00&ndash;0.70|
|Before FDR               |6 hr      |     35&ndash;41|  0.22&ndash;0.63|

The ranges are across the nine tissues.


|Tissue                          | Matched after-FDR associations| GTEx p < 0.05| Of those, expected direction|
|:-------------------------------|------------------------------:|-------------:|----------------------------:|
|Cerebellum                      |                              8|             5|                            5|
|Cerebellar Hemisphere           |                              8|             5|                            5|
|Caudate basal ganglia           |                              8|             5|                            5|
|Cortex                          |                              9|             5|                            5|
|Frontal Cortex BA9              |                              8|             5|                            5|
|Hippocampus                     |                              8|             6|                            5|
|Hypothalamus                    |                              9|             5|                            5|
|Nucleus accumbens basal ganglia |                              8|             5|                            5|
|Putamen basal ganglia           |                              8|             5|                            5|

After FDR, each distinct association counts once per tissue, over all timepoints.
Download [the estimates](assets/isolaser_gtex_reads10nc_q010_hetcis/pi1.tsv) and [the after-FDR
matches](assets/isolaser_gtex_reads10nc_q010_hetcis/after_fdr_matches.tsv) (made by `58.gtex_pi1.R`).


# Gene-level overlap with GTEx sGenes {.tabset}

One tab per tissue, with the same layout as the scatter plots: rows are the
three sets and columns the timepoints. The numbers in each panel are:

- **isoLASER genes only**: genes with at least one association of the set at
  that timepoint that are not GTEx sGenes;
- **both**: genes that are both;
- **GTEx sGenes only**: GTEx sGenes of the tissue (gene-level q < 0.05) without
  an association of ours.

Each panel is restricted to genes tested in both studies at that timepoint: in
our permutation run and by GTEx in that tissue. This overlap is at the gene level.
A gene counts as shared when GTEx finds an sQTL in it through any variant and
junction, not necessarily our SNV or our event. The scatter plots require both, so
their gene counts are smaller.

## Cerebellum

![](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Cerebellum.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Cerebellum.pdf)

## Cerebellar Hemisphere

![](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Cerebellar_Hemisphere.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Cerebellar_Hemisphere.pdf)

## Caudate basal ganglia

![](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Caudate_basal_ganglia.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Caudate_basal_ganglia.pdf)

## Cortex

![](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Cortex.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Cortex.pdf)

## Frontal Cortex BA9

![](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Frontal_Cortex_BA9.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Frontal_Cortex_BA9.pdf)

## Hippocampus

![](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Hippocampus.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Hippocampus.pdf)

## Hypothalamus

![](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Hypothalamus.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Hypothalamus.pdf)

## Nucleus accumbens basal ganglia

![](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Nucleus_accumbens_basal_ganglia.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Nucleus_accumbens_basal_ganglia.pdf)

## Putamen basal ganglia

![](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Putamen_basal_ganglia.png)

[Open as PDF](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_Brain_Putamen_basal_ganglia.pdf)

Download the [gene counts](assets/isolaser_gtex_reads10nc_q010_hetcis/venn_counts.tsv) for every tissue, set and
timepoint (made by `57.gtex_gene_venn.R`).

<br>
<p>
<button type="button" class="btn btn-default btn-workflowr btn-workflowr-sessioninfo"
  data-toggle="collapse" data-target="#workflowr-sessioninfo"
  style = "display: block;">
  <span class="glyphicon glyphicon-wrench" aria-hidden="true"></span>
  Session information
</button>
</p>

<div id="workflowr-sessioninfo" class="collapse">

```
R version 4.2.0 (2022-04-22)
Platform: x86_64-pc-linux-gnu (64-bit)
Running under: CentOS Linux 7 (Core)

Matrix products: default
BLAS/LAPACK: /software/openblas-0.3.13-el7-x86_64/lib/libopenblas_haswellp-r0.3.13.so

locale:
[1] C

attached base packages:
[1] stats     graphics  grDevices utils     datasets  methods   base     

other attached packages:
[1] data.table_1.14.2

loaded via a namespace (and not attached):
 [1] Rcpp_1.0.12      rstudioapi_0.13  whisker_0.4      knitr_1.39      
 [5] magrittr_2.0.3   workflowr_1.7.0  R6_2.5.1         rlang_1.1.2     
 [9] fastmap_1.1.0    fansi_1.0.3      highr_0.9        stringr_1.5.1   
[13] tools_4.2.0      xfun_0.41        utf8_1.2.2       cli_3.6.1       
[17] git2r_0.30.1     jquerylib_0.1.4  htmltools_0.5.2  rprojroot_2.0.3 
[21] yaml_2.3.5       digest_0.6.29    tibble_3.2.1     lifecycle_1.0.4 
[25] later_1.3.0      sass_0.4.1       vctrs_0.6.5      promises_1.2.0.1
[29] fs_1.5.2         glue_1.6.2       evaluate_0.15    rmarkdown_2.25  
[33] stringi_1.7.6    bslib_0.3.1      compiler_4.2.0   pillar_1.9.0    
[37] jsonlite_1.8.0   httpuv_1.6.5     pkgconfig_2.0.3 
```
</div>
