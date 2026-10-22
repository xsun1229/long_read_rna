---
title: "Genome-wide FDR with genotype-panel donors (rerun)"
author: "XSun"
date: "2026-10-21"
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
  <p><strong>Last updated:</strong> 2026-10-21</p>
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
<a data-toggle="collapse" data-parent="#workflowr-checks" href="#strongRepositoryversionstrongahrefhttpsgithubcomxsun1229longreadrnatreee1bc6bf6d5e7456abf8cac2700cea90e2c2123bctargetblanke1bc6bfa">
  <span class="glyphicon glyphicon-ok text-success" aria-hidden="true"></span>
  <strong>Repository version:</strong> <a href="https://github.com/xsun1229/long_read_rna/tree/e1bc6bf6d5e7456abf8cac2700cea90e2c2123bc" target="_blank">e1bc6bf</a>
</a>
</p>
</div>
<div id="strongRepositoryversionstrongahrefhttpsgithubcomxsun1229longreadrnatreee1bc6bf6d5e7456abf8cac2700cea90e2c2123bctargetblanke1bc6bfa" class="panel-collapse collapse">
<div class="panel-body">
  
<p>
Great! You are using Git for version control. Tracking code development and
connecting the code version to the results is critical for reproducibility.
</p>

<p>
The results in this page were generated with repository version <a href="https://github.com/xsun1229/long_read_rna/tree/e1bc6bf6d5e7456abf8cac2700cea90e2c2123bc" target="_blank">e1bc6bf</a>.
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
Unstaged changes:
	Modified:   analysis/isolaser_fdr_panel10.Rmd

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
to the R Markdown (<code>analysis/isolaser_fdr_panel10.Rmd</code>) and HTML (<code>docs/isolaser_fdr_panel10.html</code>)
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
<td><a href="https://github.com/xsun1229/long_read_rna/blob/ec3f404c78db0679021a605a0801bce4613a775f/analysis/isolaser_fdr_panel10.Rmd" target="_blank">ec3f404</a></td>
<td>XSun</td>
<td>2026-10-21</td>
<td>update</td>
</tr>
<tr>
<td>html</td>
<td><a href="https://rawcdn.githack.com/xsun1229/long_read_rna/ec3f404c78db0679021a605a0801bce4613a775f/docs/isolaser_fdr_panel10.html" target="_blank">ec3f404</a></td>
<td>XSun</td>
<td>2026-10-21</td>
<td>update</td>
</tr>
<tr>
<td>Rmd</td>
<td><a href="https://github.com/xsun1229/long_read_rna/blob/79006b34f9580bdb24666e917d242319fea2095d/analysis/isolaser_fdr_panel10.Rmd" target="_blank">79006b3</a></td>
<td>XSun</td>
<td>2026-10-21</td>
<td>update</td>
</tr>
<tr>
<td>html</td>
<td><a href="https://rawcdn.githack.com/xsun1229/long_read_rna/79006b34f9580bdb24666e917d242319fea2095d/docs/isolaser_fdr_panel10.html" target="_blank">79006b3</a></td>
<td>XSun</td>
<td>2026-10-21</td>
<td>update</td>
</tr>
<tr>
<td>Rmd</td>
<td><a href="https://github.com/xsun1229/long_read_rna/blob/45459a52e6043a4167001f388ed3d026a8cc43d7/analysis/isolaser_fdr_panel10.Rmd" target="_blank">45459a5</a></td>
<td>XSun</td>
<td>2026-10-21</td>
<td>update</td>
</tr>
<tr>
<td>html</td>
<td><a href="https://rawcdn.githack.com/xsun1229/long_read_rna/45459a52e6043a4167001f388ed3d026a8cc43d7/docs/isolaser_fdr_panel10.html" target="_blank">45459a5</a></td>
<td>XSun</td>
<td>2026-10-21</td>
<td>update</td>
</tr>
<tr>
<td>Rmd</td>
<td><a href="https://github.com/xsun1229/long_read_rna/blob/2b0e0d3bcd745cd8c7f5f16705f6b2752cd53825/analysis/isolaser_fdr_panel10.Rmd" target="_blank">2b0e0d3</a></td>
<td>XSun</td>
<td>2026-10-21</td>
<td>update</td>
</tr>
<tr>
<td>html</td>
<td><a href="https://rawcdn.githack.com/xsun1229/long_read_rna/2b0e0d3bcd745cd8c7f5f16705f6b2752cd53825/docs/isolaser_fdr_panel10.html" target="_blank">2b0e0d3</a></td>
<td>XSun</td>
<td>2026-10-21</td>
<td>update</td>
</tr>
<tr>
<td>Rmd</td>
<td><a href="https://github.com/xsun1229/long_read_rna/blob/5149846aa5a6796cd87ac93500cf019ec1fef2fb/analysis/isolaser_fdr_panel10.Rmd" target="_blank">5149846</a></td>
<td>XSun</td>
<td>2026-10-21</td>
<td>update</td>
</tr>
<tr>
<td>html</td>
<td><a href="https://rawcdn.githack.com/xsun1229/long_read_rna/5149846aa5a6796cd87ac93500cf019ec1fef2fb/docs/isolaser_fdr_panel10.html" target="_blank">5149846</a></td>
<td>XSun</td>
<td>2026-10-21</td>
<td>update</td>
</tr>
</tbody>
</table>
</div>

<hr>
</div>
</div>
</div>








This page repeats the [genome-wide FDR analysis](isolaser_fdr.html) with a
different way of choosing donors and associations. Many variant calls behind
the original results have no support in the donors' own genotype panel (see
[technical artifacts in isoLASER variant calls](isolaser_variant_artifacts.html)).
The original page and its results are unchanged.

**What changed (our definitions):**

- **Donors:** a donor is used for an association only if our genotype panel
  calls it heterozygous at that variant. The panel site must be directly
  genotyped or imputed with R² ≥ 0.8, with the same two alleles. The donor also
  needs ≥ 10 informative reads, isoLASER's own default. The original rule was
  ≥ 30 reads and an RNA alternative-allele fraction of 0.25–0.75.
- **Associations:** every variant × exonic part recorded in any donor. The
  original run used only the rows of isoLASER's joint output, which drops parts
  seen in a single donor.
- **Tested family:** additionally ≥ 20 raw reads summed over the donors used.
  Fewer can never give the ≥ 10 reads per allele that isoLASER needs to score
  an association.
- **Unchanged:** the shuffles, the scoring with isoLASER's functions, the
  adaptive rounds, BH within each timepoint, and the `cis` / |ΔPSI| ≥ 0.10
  screen applied afterwards.
- **Not yet done:** calibration runs. The original calibration used a
  different donor rule, so it does not carry over to this run.

**Main result:** 64 associations in
**26 genes** have q < 0.05 and pass the screen,
against 375 in
131 genes originally. 7 genes are
significant at all three timepoints.

# Genome-wide results


|Timepoint     | Tested associations| Paper's cutoff|    Screen| Screen + q < 0.10| Screen + q < 0.05|
|:-------------|-------------------:|--------------:|---------:|-----------------:|-----------------:|
|0hr           |              40,164|   10,419 (978)| 259 (119)|           29 (13)|           25 (12)|
|1hr           |              60,866| 11,880 (1,362)| 435 (184)|           51 (22)|           41 (17)|
|6hr           |              63,223| 12,086 (1,350)| 425 (183)|           39 (18)|           35 (16)|
|any timepoint |              76,939| 23,251 (2,101)| 995 (396)|           73 (31)|           64 (26)|

Cells other than **Tested associations** show **associations (genes)**.

- **Paper's cutoff:** isoLASER's own `cis` call with no other filter, as in the
  isoLASER paper. It comes from isoLASER's joint output, so it is the same as on
  the original page.
- **Screen** (our definition), before FDR control: among the tested
  associations, isoLASER's `cis` rule computed on the panel-heterozygous donors
  only, plus |ΔPSI| ≥ 0.10.

**Any timepoint** counts each gene or variant–part association once across
timepoints. BH targets FDR within each timepoint's full family; the
effect-filtered subset and the union across timepoints have no separate 5% FDR
guarantee.

# Compared with the original run


|Timepoint     | Tested: original| Tested: rerun| Screen + q < 0.05: original| Screen + q < 0.05: rerun|
|:-------------|----------------:|-------------:|---------------------------:|------------------------:|
|0hr           |           37,156|        40,164|                    191 (64)|                  25 (12)|
|1hr           |           57,517|        60,866|                    183 (73)|                  41 (17)|
|6hr           |           60,860|        63,223|                    174 (74)|                  35 (16)|
|any timepoint |           77,954|        76,939|                   375 (131)|                  64 (26)|

The rerun tests a similar number of associations, but far fewer reach
q < 0.05. Most original hits used variants that are not in the panel, which
the new donor rule cannot use.

<!-- ```{r gene_changes} -->
<!-- knitr::kable(gc[, .N, by=status][match(c("both", "original only", "rerun only"), status)][, -->
<!--   .(`Significant genes`=c("In both runs", "Original run only", "Rerun only"), Genes=N)], align="lr") -->
<!-- ``` -->

<!-- The rerun-only genes are ANKRD36C, CRYBB2P1, HSP90B1, RPS27L. ANKRD36C (and -->
<!-- ANKRD36B, significant in both runs) and the pseudogene CRYBB2P1 belong to -->
<!-- paralog or pseudogene families. Misaligned reads remain possible there even at -->
<!-- real SNPs (our inference), so they need care. -->
<!-- [Download the gene comparison](assets/fdr_panel10/gene_changes.tsv). -->

# How the test works

The test is the one described on the [original page](isolaser_fdr.html#how-the-test-works).
Only the donor and family rules above differ. An association's eligible
donors are fixed before shuffling, from read counts and the panel genotype,
neither of which a shuffle changes. Eligible associations without a computable
observed score stay in the family with p = 1.


|Timepoint | Stopped at 1,000| Stopped at 10,000| Stopped at 100,000| Reached 1,000,000|
|:---------|----------------:|-----------------:|------------------:|-----------------:|
|0hr       |           39,753|               295|                 68|                48|
|1hr       |           60,186|               509|                 91|                80|
|6hr       |           62,597|               497|                 63|                66|

**Stopped** means at least 20 hits at that checkpoint, or no observed score
(p = 1). Every association with zero hits after a million shuffles has
q < 0.05, so more shuffles would not change the results.

![](assets/fdr_panel10/qq.png)

Real data only; there are no calibration runs for this donor rule. The bulk
lies below the diagonal: many associations tie with their shuffles at an AMI of
0, which isoLASER rounds to three decimals, so their p-values are
conservative. The upper plateau is the minimum attainable p-value.

# Genes to follow up



We highlight genes that meet two conditions (our definitions):

1. **Reported only after stimulation:** q < 0.05 plus the `cis` /
   effect-size screen at 1 or 6 hours, and not at 0 hours.
2. **Neuron- or stimulation-related:** a neuronal GO term, a brain disorder in
   SFARI or DDG2P, or a change in expression or splicing after stimulation in
   our data (the annotation columns of the full gene table below).

7 genes meet both; five are shown. Not shown: **ALDH3A2**, because
isoLASER recorded no test of this association at 0 hours, so there is no
0-hour comparison; and **UBE2Q2P2**, a pseudogene, where reads from similar
copies can be misaligned (our inference).


|Gene   |     0 hr|      1 hr|      6 hr| Best q| Het donors|Relevance                                                                           |
|:------|--------:|---------:|---------:|------:|----------:|:-----------------------------------------------------------------------------------|
|KPNA2  | +8 (125)|  +2 (284)| +12 (500)| 0.0160|          3|Synapse, synaptic signaling (GO)                                                    |
|PARK7  | -7 (595)| -17 (980)|  -8 (969)| 0.0016|          2|Neuron projection, neuron death (GO); the Parkinson's disease gene DJ-1             |
|ZNF749 | -26 (88)|  -17 (84)| -74 (127)| 0.0019|          3|Splicing after stimulation (our scan), at this exon's donor sites                   |
|ASAH1  |  +7 (36)| +21 (104)|   +8 (65)| 0.0280|          2|Farber disease; spinal muscular atrophy with progressive myoclonic epilepsy (DDG2P) |
|LMBRD1 | +74 (35)|  +85 (37)|  +93 (76)| 0.0019|          2|Methylmalonic aciduria and homocystinuria, cblF type (DDG2P)                        |

**0 / 1 / 6 hr**: allelic effect in percentage points, alternative minus
reference inclusion, with pooled informative coverage in brackets. **Best q**:
the lowest timepoint-specific q-value. **Het donors**: the largest number of
panel-heterozygous donors used, out of four. All numbers refer to each gene's
representative association.

**How to read each gene's figures:**

- **Permutation test:** one panel per timepoint. Grey bars are the first 1,000
  shuffled scores; the blue line is the observed score (AMI). The p-value uses
  the full adaptive run, up to a million shuffles.
- **Read alignments:** isoLASER's `nigiri_plot` sashimi renderer with the
  project's plotting fixes. Reads are split into REF (blue) and ALT (orange) by
  isoLASER's allele assignments and pooled over the donors used at each
  timepoint (heterozygous in the panel, ≥ 10 reads). Yellow marks the tested
  part. Coverage and arc numbers are raw read counts, on one scale per gene.
  **Raw inclusion** comes from isoLASER's transcript assignment, so a read can
  count without reaching the plotted region. Each plot's subtitles give how many
  reads reach it. The test uses donor-normalized tables, so its dPSI can differ
  slightly from the raw counts.
- **Isoforms and haplotypes**, at 0 hours and at the significant timepoint,
  drawn like Fig. 2d of the isoLASER paper:
  - **Rows:** annotated transcripts with their GENCODE v44 name and Ensembl ID.
    **Novel** transcripts are IsoQuant models from our annotation, shown with
    their SQANTI3 category against GENCODE v44. NIC is a new combination of
    known splice sites; fusion spans two genes.
  - **Which rows:** the three transcripts with the most reads in each group are
    drawn, and a grey row sums the rest. Introns are shortened.
  - **Marks:** green is the tested part. Orange marks the tested SNP, plus the
    nearest in-phase SNP when that one is closer to the part.
  - **Numbers:** reads per transcript from each haplotype, labelled by the
    tested SNP's alleles, as raw counts summed over the donors used.
  - **PSI row:** each haplotype's inclusion from those raw counts: reads in
    transcripts that include the part, divided by all its reads, drawn and
    undrawn transcripts together.
  - **Test line:** ΔPSI and q are the test's values. The test pools
    donor-normalized tables, so its ΔPSI can differ slightly from the
    difference between the two raw PSIs.

## KPNA2

The tested part is a whole 100-base intron between exons 6 and 7. KPNA2-221
keeps it, and the other annotated transcripts splice it out. isoLASER counts
ALT (C) reads as keeping the intron more often than REF (T) reads: at 6 hours,
12.7% vs 2.5% (+12 pp, q = 0.016). At 0 and 1 hours the difference is +8 and
+2 pp, below threshold. The tested SNP (rs12752) is in the first exon, 7.2 kb
upstream. In the three donors, all 20 heterozygous panel SNPs within the gene
are phased the same way, so T and C reads come from two whole-gene haplotypes. The
nearest SNP to the intron, rs4638, is 135 bases downstream, with G on the T
haplotype.

#### Permutation test

![](assets/fdr_panel10/KPNA2_null.png)

#### Read alignments

![](assets/fdr_panel10/KPNA2_sashimi.png)


|Timepoint |Donors            | REF inclusion (raw)| ALT inclusion (raw)| Test dPSI (normalized, pp)|
|:---------|:-----------------|-------------------:|-------------------:|--------------------------:|
|0 hr      |CD_21,CD_31,CD_36 |         5/60 (8.3%)|       12/64 (18.8%)|                       +8.2|
|1 hr      |CD_21,CD_31,CD_36 |        7/166 (4.2%)|        8/119 (6.7%)|                       +1.9|
|6 hr      |CD_21,CD_31,CD_36 |        7/281 (2.5%)|      28/220 (12.7%)|                      +11.6|

[Open as PDF](assets/fdr_panel10/KPNA2_sashimi.pdf).

#### Isoforms and haplotypes

![](assets/fdr_panel10/isoforms_KPNA2_0hr.png)

![](assets/fdr_panel10/isoforms_KPNA2_6hr.png)

## PARK7

The first exon ends at one of two donor sites 58 bases apart, an alternative 5′
splice site, and both sites splice to the same next exon. The tested 12-base
part is the extra stretch of the longer first exon; the adjacent 46-base part
gives the same result. ALT (C) reads use the shorter exon more often than REF
(T) reads. The difference has the same direction at all three timepoints and in
both donors, and is largest at 1 hour (−17 pp, q = 0.002), the only
significant timepoint; at 0 and 6 hours it is −7 and −8 pp. This describes each
timepoint separately and is not a test of a change over time. The variant
(rs226249) lies in the first exon, 18 bases before the shorter exon's donor
site.

#### Permutation test

![](assets/fdr_panel10/PARK7_null.png)

#### Read alignments

![](assets/fdr_panel10/PARK7_sashimi.png)


|Timepoint |Donors      | REF inclusion (raw)| ALT inclusion (raw)| Test dPSI (normalized, pp)|
|:---------|:-----------|-------------------:|-------------------:|--------------------------:|
|0 hr      |CD_21,CD_48 |     243/365 (66.6%)|     136/229 (59.4%)|                       -7.3|
|1 hr      |CD_21,CD_48 |     473/661 (71.6%)|     174/319 (54.5%)|                      -17.3|
|6 hr      |CD_21,CD_48 |     440/640 (68.8%)|     200/329 (60.8%)|                       -8.1|

[Open as PDF](assets/fdr_panel10/PARK7_sashimi.pdf).

#### Isoforms and haplotypes

![](assets/fdr_panel10/isoforms_PARK7_0hr.png)

![](assets/fdr_panel10/isoforms_PARK7_1hr.png)

## ZNF749

The tested part is a 355-base alternative last exon. Transcripts that use it
end there, and the others continue to exons further downstream. REF (G) reads
end in it far more often than ALT (C) reads. The difference is significant only
at 6 hours (−74 pp, q = 0.002); at 0 and 1 hours it is −26 and −17 pp and below
threshold. In our stimulation splicing scan, the balance between the two donor
sites that splice into this exon shifts between 0 and 6 hours.

The jump at 6 hours partly reflects which donors are used:

- **CD_21** has a large effect at every timepoint: REF 92% vs ALT 15% inclusion
  at 0 hours, 86% vs 6% at 6 hours.
- **CD_48** shows no difference at 0 hours, from only 8 ALT reads, and a large
  one at 6 hours (85% vs 19%).
- **CD_36** has an inconsistent effect (−19 pp at 0 hours, +8 pp at 1 hour)
  and no reads at 6 hours.

#### Permutation test

![](assets/fdr_panel10/ZNF749_null.png)

#### Read alignments

![](assets/fdr_panel10/ZNF749_sashimi.png)


|Timepoint |Donors            | REF inclusion (raw)| ALT inclusion (raw)| Test dPSI (normalized, pp)|
|:---------|:-----------------|-------------------:|-------------------:|--------------------------:|
|0 hr      |CD_21,CD_36,CD_48 |       45/55 (81.8%)|       15/32 (46.9%)|                      -25.5|
|1 hr      |CD_21,CD_36       |       39/50 (78.0%)|       19/34 (55.9%)|                      -17.2|
|6 hr      |CD_21,CD_48       |       72/84 (85.7%)|        6/44 (13.6%)|                      -74.1|

[Open as PDF](assets/fdr_panel10/ZNF749_sashimi.pdf).

#### Isoforms and haplotypes

![](assets/fdr_panel10/isoforms_ZNF749_0hr.png)

![](assets/fdr_panel10/isoforms_ZNF749_6hr.png)

## ASAH1

The tested part is a 115-base alternative first exon: ASAH1-264 starts with it,
and the other transcripts start at another first exon. isoLASER counts ALT (A)
reads as using it more often than REF (G) reads at 1 hour (+21 pp,
q = 0.028). At 0 and 6 hours the difference is +7 and +8 pp, below threshold.
The 1-hour test uses two donors (CD_21 and CD_31); 0 and 6 hours use CD_21
only. The tested SNP (rs7508) is in the last exon, about 19 kb away in the
genome, and about half of the reads reach the plotted region.

#### Permutation test

![](assets/fdr_panel10/ASAH1_null.png)

#### Read alignments

![](assets/fdr_panel10/ASAH1_sashimi.png)


|Timepoint |Donors      | REF inclusion (raw)| ALT inclusion (raw)| Test dPSI (normalized, pp)|
|:---------|:-----------|-------------------:|-------------------:|--------------------------:|
|0 hr      |CD_21       |         0/22 (0.0%)|         1/14 (7.1%)|                       +7.1|
|1 hr      |CD_21,CD_31 |         0/52 (0.0%)|       10/52 (19.2%)|                      +20.8|
|6 hr      |CD_21       |         0/40 (0.0%)|         2/25 (8.0%)|                       +8.0|

[Open as PDF](assets/fdr_panel10/ASAH1_sashimi.pdf).

#### Isoforms and haplotypes

![](assets/fdr_panel10/isoforms_ASAH1_0hr.png)

![](assets/fdr_panel10/isoforms_ASAH1_1hr.png)

## LMBRD1

The first exon ends at one of two donor sites, an alternative 5′ splice site,
and the 77-base part is the extra stretch of the longer first exon in
LMBRD1-225. isoLASER counts nearly all ALT (A) reads as including it and no REF
(G) reads: +93 pp at 6 hours (q = 0.002).

- **0 hours:** a similar difference, +74 pp, but from 35 reads in two donors
  and below threshold (nominal p = 0.007).
- **1 hour:** +85 pp, from only one qualifying donor.
- **The gene at 1 hour:** it is reported through a different part.

The tested SNP (rs9185) is in the last exon, about 120 kb away in the genome.
rs3752787, 113 bases from the part, is in phase with it (C on the A
haplotype). Few reads reach the plotted region (8 of 76 at 6 hours).

#### Permutation test

![](assets/fdr_panel10/LMBRD1_null.png)

#### Read alignments

![](assets/fdr_panel10/LMBRD1_sashimi.png)


|Timepoint |Donors      | REF inclusion (raw)| ALT inclusion (raw)| Test dPSI (normalized, pp)|
|:---------|:-----------|-------------------:|-------------------:|--------------------------:|
|0 hr      |CD_31,CD_36 |         0/13 (0.0%)|       17/22 (77.3%)|                      +73.9|
|1 hr      |CD_31       |         0/11 (0.0%)|       22/26 (84.6%)|                      +84.6|
|6 hr      |CD_31,CD_36 |         0/31 (0.0%)|       41/45 (91.1%)|                      +93.2|

[Open as PDF](assets/fdr_panel10/LMBRD1_sashimi.pdf).

#### Isoforms and haplotypes

![](assets/fdr_panel10/isoforms_LMBRD1_0hr.png)

![](assets/fdr_panel10/isoforms_LMBRD1_6hr.png)

## Data

**Isoform figures** (PDF, and reads per transcript as a table):

- **KPNA2**: 0 hr ([PDF](assets/fdr_panel10/isoforms_KPNA2_0hr.pdf), [reads per transcript](assets/fdr_panel10/isoforms_KPNA2_0hr_transcripts.tsv)); 6 hr ([PDF](assets/fdr_panel10/isoforms_KPNA2_6hr.pdf), [reads per transcript](assets/fdr_panel10/isoforms_KPNA2_6hr_transcripts.tsv))
- **PARK7**: 0 hr ([PDF](assets/fdr_panel10/isoforms_PARK7_0hr.pdf), [reads per transcript](assets/fdr_panel10/isoforms_PARK7_0hr_transcripts.tsv)); 1 hr ([PDF](assets/fdr_panel10/isoforms_PARK7_1hr.pdf), [reads per transcript](assets/fdr_panel10/isoforms_PARK7_1hr_transcripts.tsv))
- **ZNF749**: 0 hr ([PDF](assets/fdr_panel10/isoforms_ZNF749_0hr.pdf), [reads per transcript](assets/fdr_panel10/isoforms_ZNF749_0hr_transcripts.tsv)); 6 hr ([PDF](assets/fdr_panel10/isoforms_ZNF749_6hr.pdf), [reads per transcript](assets/fdr_panel10/isoforms_ZNF749_6hr_transcripts.tsv))
- **ASAH1**: 0 hr ([PDF](assets/fdr_panel10/isoforms_ASAH1_0hr.pdf), [reads per transcript](assets/fdr_panel10/isoforms_ASAH1_0hr_transcripts.tsv)); 1 hr ([PDF](assets/fdr_panel10/isoforms_ASAH1_1hr.pdf), [reads per transcript](assets/fdr_panel10/isoforms_ASAH1_1hr_transcripts.tsv))
- **LMBRD1**: 0 hr ([PDF](assets/fdr_panel10/isoforms_LMBRD1_0hr.pdf), [reads per transcript](assets/fdr_panel10/isoforms_LMBRD1_0hr_transcripts.tsv)); 6 hr ([PDF](assets/fdr_panel10/isoforms_LMBRD1_6hr.pdf), [reads per transcript](assets/fdr_panel10/isoforms_LMBRD1_6hr_transcripts.tsv)) 

- **Sashimi plots:** [inclusion counts](assets/fdr_panel10/sashimi_summary.tsv),
  [per-donor counts](assets/fdr_panel10/sashimi_donor_counts.tsv),
  [normalized test counts](assets/fdr_panel10/sashimi_normalized_counts.tsv),
  [junction counts](assets/fdr_panel10/sashimi_junction_counts.tsv).
- **Scripts**, all with `ADAPTIVE_RULE=panel10`:
  - in `10.isolaser_permutation/`: `24.plot_association.R` (permutation
    tests), `25.sashimi_candidates.py` and `36.refresh_sashimi_labels.R`
    (sashimi);
  - in `11.fdr_results/`: `4.transcript_counts.py`, then
    `7.grant_figure_transcripts.R` (isoform figures).

# All reported genes

Here, **reported** means q < 0.05 plus the `cis` / effect-size screen.


|Pattern                                     | Genes|
|:-------------------------------------------|-----:|
|Significant at 3 timepoints                 |     7|
|Significant at 2 timepoints                 |     5|
|One timepoint; nominal support elsewhere    |     8|
|One timepoint; no nominal support elsewhere |     4|
|One timepoint; no usable score elsewhere    |     2|

For genes reported at one timepoint, the last three categories describe the
representative association at the other timepoints: nominal p < 0.05,
p ≥ 0.05 where scored, or no usable score. They are not tests of an allele ×
time interaction. Among comparisons of significant associations with another
timepoint, 88% had nominal p < 0.05 there and
99% had the same effect direction.

## Full interactive gene table

All **26 reported genes**. The variant, part, timepoint effects, best q
and donor count refer to the representative association; **Significant at**
describes the gene across all its associations. **In original run** marks
genes also reported on the original page.


```{=html}
<div id="htmlwidget-b79198de2c3cef88097c" style="width:100%;height:auto;" class="datatables html-widget"></div>
<script type="application/json" data-for="htmlwidget-b79198de2c3cef88097c">{"x":{"filter":"top","vertical":false,"filterHTML":"<tr>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"number\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"display: none;position: absolute;width: 200px;opacity: 1\">\n      <div data-min=\"0.0016\" data-max=\"0.03\" data-scale=\"4\"><\/div>\n      <span style=\"float: left;\"><\/span>\n      <span style=\"float: right;\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"integer\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"display: none;position: absolute;width: 200px;opacity: 1\">\n      <div data-min=\"1\" data-max=\"3\"><\/div>\n      <span style=\"float: left;\"><\/span>\n      <span style=\"float: right;\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"logical\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\" disabled=\"\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n    <div style=\"width: 100%; display: none;\">\n      <select multiple=\"multiple\" style=\"width: 100%;\" data-options=\"[&quot;true&quot;,&quot;false&quot;,&quot;na&quot;]\"><\/select>\n    <\/div>\n  <\/td>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n  <td data-type=\"character\" style=\"vertical-align: top;\">\n    <div class=\"form-group has-feedback\" style=\"margin-bottom: auto;\">\n      <input type=\"search\" placeholder=\"All\" class=\"form-control\" style=\"width: 100%;\"/>\n      <span class=\"glyphicon glyphicon-remove-circle form-control-feedback\"><\/span>\n    <\/div>\n  <\/td>\n<\/tr>","extensions":["Buttons"],"caption":"<caption>Search or filter genes, sort columns, and export the filtered table as CSV.<\/caption>","data":[["CST3","CYBA","HNRNPK","NAA38","RPS5","TBCA","CHORDC1","HSP90B1","ANKRD36C","ASAH1","KPNA2","ALDH3A2","SNHG5","RPS27L","RPS2","ATP5MJ","CRYBB2P1","UBE2Q2P2","LEPROT","PARK7","ZNF749","DNTTIP2","ANKRD36B","PFKP","ZFAND2A","LMBRD1"],["Significant at 3 timepoints","Significant at 3 timepoints","Significant at 3 timepoints","Significant at 3 timepoints","Significant at 3 timepoints","Significant at 3 timepoints","Significant at 3 timepoints","One timepoint; no nominal support elsewhere","One timepoint; no nominal support elsewhere","One timepoint; no nominal support elsewhere","One timepoint; no nominal support elsewhere","One timepoint; no usable score elsewhere","One timepoint; no usable score elsewhere","One timepoint; nominal support elsewhere","One timepoint; nominal support elsewhere","One timepoint; nominal support elsewhere","One timepoint; nominal support elsewhere","One timepoint; nominal support elsewhere","One timepoint; nominal support elsewhere","One timepoint; nominal support elsewhere","One timepoint; nominal support elsewhere","Significant at 2 timepoints","Significant at 2 timepoints","Significant at 2 timepoints","Significant at 2 timepoints","Significant at 2 timepoints"],["0hr, 1hr, 6hr","0hr, 1hr, 6hr","0hr, 1hr, 6hr","0hr, 1hr, 6hr","0hr, 1hr, 6hr","0hr, 1hr, 6hr","0hr, 1hr, 6hr","0hr","0hr","1hr","6hr","1hr","6hr","1hr","0hr","1hr","6hr","6hr","1hr","1hr","6hr","1hr, 6hr","0hr, 6hr","0hr, 1hr","1hr, 6hr","1hr, 6hr"],["-56 (1,294)","+48 (154)","-20 (303)","-36 (150)","+50 (935)","+15 (465)","+48 (79)","-11 (419)","+22 (69)","+7 (36)","+8 (125)","no score","no score","no score","+12 (929)","+8 (1,230)","+90 (70)","+68 (31)","+18 (53)","-7 (595)","-26 (88)","no score","+48 (61)","+21 (140)","+52 (51)","+74 (35)"],["-53 (2,285)","+58 (156)","-18 (523)","-36 (225)","+53 (1,530)","+12 (851)","+52 (124)","no score","+4 (118)","+21 (104)","+2 (284)","+46 (96)","no score","+66 (52)","no score","+10 (2,211)","no score","+29 (40)","+37 (113)","-17 (980)","-17 (84)","-46 (70)","+25 (78)","+11 (297)","+40 (63)","+85 (37)"],["-58 (2,567)","+70 (202)","-21 (326)","-49 (223)","+56 (1,404)","+10 (801)","+54 (242)","+1 (412)","-1 (174)","+8 (65)","+12 (500)","no score","+20 (266)","+50 (49)","no score","+5 (2,074)","+98 (116)","+43 (98)","+38 (81)","-8 (969)","-74 (127)","no score","+34 (113)","+10 (340)","+49 (120)","+93 (76)"],[0.0016,0.0016,0.0016,0.0016,0.0016,0.0016,0.0016,0.0024,0.026,0.028,0.016,0.0016,0.03,0.0066,0.0024,0.0016,0.0019,0.016,0.0066,0.0016,0.0019,0.0016,0.0024,0.0066,0.0019,0.0019],[3,1,3,1,1,2,2,1,2,2,3,2,2,2,1,2,1,2,2,2,3,2,2,2,2,2],["yes","yes","yes","yes","yes","yes","yes","no","no","yes","yes","yes","yes","no","yes","yes","no","yes","yes","yes","yes","yes","yes","yes","yes","yes"],["","","","","","","","","","","synapse; synaptic signaling","","","","","","","","","neuron projection; neuron death","","","","","",""],["","","SFARI score 2, syndromic; HNRNPK-related Au-Kline syndrome","","","","","","","ASAH1-related Farber lipogranulomatosis; ASAH1-related spinal muscular atrophy with progressive myoclonic epilepsy","","ALDH3A2-related Sjogren-Larsson syndrome","","","","","","","","","","","","","","LMBRD1-related methylmalonic aciduria and homocystinuria"],[null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null,null],["","","","yes","","","","","yes","","","","","","","","","yes","","","yes","","yes","","",""],["chr20:23637789:C&gt;T","chr16:88646827:A&gt;G","chr9:83980154:C&gt;T","chr17:7857385:A&gt;G","chr19:58394795:T&gt;C","chr5:77776296:G&gt;C","chr11:90223037:G&gt;A","chr12:103934200:C&gt;T","chr2:95991826:A&gt;G","chr8:18056460:G&gt;A","chr17:68035783:T&gt;C","chr17:19675559:A&gt;T","chr6:85678169:G&gt;T","chr15:63157480:C&gt;G","chr16:1964589:C&gt;T","chr14:103915164:T&gt;C","chr22:25459491:G&gt;A","chr15:82404653:A&gt;G","chr1:65420714:T&gt;C","chr1:7961717:T&gt;C","chr19:57435555:G&gt;C","chr1:93879159:C&gt;T","chr2:97547720:C&gt;G","chr10:3136622:G&gt;C","chr7:1159995:T&gt;C","chr6:69675816:G&gt;A"],["chr20:23637932-23637945:-","chr16:88643289-88643312:-","chr9:83980118-83980152:-","chr17:7857198-7857263:-","chr19:58388417-58388480:+","chr5:77691498-77693265:-","chr11:90211318-90211335:-","chr12:103930683-103930800:+","chr2:95938828-95938901:-","chr8:18075922-18076037:-","chr17:68042999-68043099:+","chr17:19648850-19648877:+","chr6:85677794-85677868:-","chr15:63152782-63153852:-","chr16:1962909-1962949:-","chr14:103914478-103914633:-","chr22:25459515-25459681:+","chr15:82395232-82395301:+","chr1:65421327-65421459:+","chr1:7961735-7961747:+","chr19:57438101-57438456:+","chr1:93875644-93875665:-","chr2:97550103-97550166:-","chr10:3129006-3129818:+","chr7:1153224-1153241:-","chr6:69796413-69796490:-"]],"container":"<table class=\"display\">\n  <thead>\n    <tr>\n      <th>Gene<\/th>\n      <th>Pattern<\/th>\n      <th>Significant at<\/th>\n      <th>0 hr<\/th>\n      <th>1 hr<\/th>\n      <th>6 hr<\/th>\n      <th>Best q<\/th>\n      <th>Het donors<\/th>\n      <th>In original run<\/th>\n      <th>Neuronal GO term<\/th>\n      <th>Developmental disorder or autism<\/th>\n      <th>Expression after stimulation<\/th>\n      <th>Splicing after stimulation<\/th>\n      <th>Variant<\/th>\n      <th>Exonic part<\/th>\n    <\/tr>\n  <\/thead>\n<\/table>","options":{"pageLength":10,"lengthMenu":[10,25,50],"scrollX":true,"order":[],"dom":"Blfrtip","buttons":["copy","csv"],"columnDefs":[{"className":"dt-right","targets":[6,7]}],"autoWidth":false,"orderClasses":false,"orderCellsTop":true}},"evals":[],"jsHooks":[]}</script>
```

The annotations use the same rules as on the
[original page](isolaser_fdr.html#full-interactive-gene-table). They help select
examples and are not enrichment tests.

**Data:** `10.isolaser_permutation/` with `ADAPTIVE_RULE=panel10`: inputs from
`38.prepare_panel_inputs.R`, then scripts 18–22 (see that folder's README). This
page's tables come from `11.fdr_results/3.page_tables.R` run with
`ADAPTIVE_RULE=panel10`, which writes only to `docs/assets/fdr_panel10/`.

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
[1] DT_0.22           data.table_1.14.2

loaded via a namespace (and not attached):
 [1] Rcpp_1.0.12       highr_0.9         pillar_1.9.0      compiler_4.2.0   
 [5] bslib_0.3.1       later_1.3.0       jquerylib_0.1.4   git2r_0.30.1     
 [9] workflowr_1.7.0   tools_4.2.0       digest_0.6.29     jsonlite_1.8.0   
[13] evaluate_0.15     lifecycle_1.0.4   tibble_3.2.1      pkgconfig_2.0.3  
[17] rlang_1.1.2       cli_3.6.1         rstudioapi_0.13   crosstalk_1.2.0  
[21] yaml_2.3.5        xfun_0.41         fastmap_1.1.0     stringr_1.5.1    
[25] knitr_1.39        fs_1.5.2          vctrs_0.6.5       sass_0.4.1       
[29] htmlwidgets_1.5.4 rprojroot_2.0.3   glue_1.6.2        R6_2.5.1         
[33] fansi_1.0.3       rmarkdown_2.25    magrittr_2.0.3    whisker_0.4      
[37] promises_1.2.0.1  htmltools_0.5.2   httpuv_1.6.5      utf8_1.2.2       
[41] stringi_1.7.6    
```
</div>
