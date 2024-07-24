---
title: 'Reproducability in Management Science'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - fisar
  - greiner
  - huber
  - katok
  - ozkes
  - collaborators

date: '2024-03-31T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
#publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
#publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
#publication: '<span style="font-size:0.95em;">2024-05-10: **Journal Submission**<br>
#  2023-06-21: **Plato Market Innovator Conference**<br>
#  2022-12-15: **Paris December Finance Meeting**<br>
#  2022-10-20: **Financial Management Association Meeting**<br>
#  2022-03-05: **Finance Down Under Conference**</span><br>'
#publication_short: In *ICW*

#abstract: Securities markets continuously innovate to keep pace with technology. It is often debated if such innovation is beneficial, and which market participants capture the benefits. We contribute to this debate by examining the effects of a wide range of proprietary enhancements to the trading process introduced by the stock exchanges in the United States. Generally, exchange innovation is associated with improvements in liquidity and price efficiency, although the reduction in liquidity costs primarily benefits investors trading in small quantities. Institutional investors experience less favorable outcomes; while their trading costs remain unchanged, their market participation declines.


# Summary. An optional shortened abstract.
summary: With the help of more than 700 reviewers, we assess the reproducibility of nearly 500 articles published in the journal Management Science before and after the introduction of a new Data and Code Disclosure policy in 2019. When considering only articles for which data accessibility and hardware and software requirements were not an obstacle for reviewers, the results of more than 95% of articles under the new disclosure policy could be fully or largely computationally reproduced. However, for 29% of articles, at least part of the data set was not accessible to the reviewer. Considering all articles in our sample reduces the share of reproduced articles to 68%. These figures represent a significant increase compared with the period before the introduction of the disclosure policy, where only 12% of articles voluntarily provided replication materials, of which 55% could be (largely) reproduced. Substantial heterogeneity in reproducibility rates across different fields is mainly driven by differences in data set accessibility. Other reasons for unsuccessful reproduction attempts include missing code, unresolvable code errors, weak or missing documentation, and software and hardware requirements and code complexity. Our findings highlight the importance of journal code and data disclosure policies and suggest potential avenues for enhancing their effectiveness.

tags:
  Published in <em>Management Science</em>

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://drive.google.com/file/d/1kMe2G62gmxtMEa-IfyocuTC87YDBqJ0H/view?usp=sharing'
#url_code: 'https://github.com/HugoBlox/hugo-blox-builder'
#url_dataset: 'https://github.com/HugoBlox/hugo-blox-builder'
#url_poster: ''
#url_project: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  #caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
#projects:
#  - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
#slides: example
---
<table style="width:100%; border-collapse: collapse; border:none;">
  <tr style="border:none;">
    <td colspan="2" style="font-size:24px; font-weight:bold; text-align:center; border:none;">
      Abstract
    </td>
  </tr>
  <tr style="border:none;">
    <td colspan="2" style="font-size:16px; text-align:left; border:none;">
      With the help of more than 700 reviewers, we assess the reproducibility of nearly 500 articles published in the journal Management Science before and after the introduction of a new Data and Code Disclosure policy in 2019. When considering only articles for which data accessibility and hardware and software requirements were not an obstacle for reviewers, the results of more than 95% of articles under the new disclosure policy could be fully or largely computationally reproduced. However, for 29% of articles, at least part of the data set was not accessible to the reviewer. Considering all articles in our sample reduces the share of reproduced articles to 68%. These figures represent a significant increase compared with the period before the introduction of the disclosure policy, where only 12% of articles voluntarily provided replication materials, of which 55% could be (largely) reproduced. Substantial heterogeneity in reproducibility rates across different fields is mainly driven by differences in data set accessibility. Other reasons for unsuccessful reproduction attempts include missing code, unresolvable code errors, weak or missing documentation, and software and hardware requirements and code complexity. Our findings highlight the importance of journal code and data disclosure policies and suggest potential avenues for enhancing their effectiveness.
    </td>
  </tr>
      </table>
    </td>
  </tr>
</table>

##### **Introduction**

<span style="font-size:0.8em;">

To be relevant and credible, scientific results have to be verifiable. The integrity of academic endeavors rests on reproducibility, wherein independent researchers obtain consistent results using the same methodology and data, and replicability, which involves the application of similar procedures to new data. 
The significance of these twin principles for scientific research is commonly agreed upon. Yet, recent assessments of empirical studies in the social sciences suggest a concerning rate of non-reproducibility or non-replicability (Ioannidis 2005, Ioannidis and Doucouliagos 2013, Open Science Collaboration 2015). A replicability crisis does not only erode the confidence in individual studies, but casts a shadow over entire fields and literatures, and may potentially compromise business and policy decisions based on these findings. Assessing and addressing these issues is imperative to maintain the credibility of social science research, including management, psychology, economics, sociology, and political science, and its subsequent applications in economic policies and management strategies, guiding societal progress.
Several reasons are cited in the literature as contributing to reduced replicability, such as publication bias (De Long and Lang 1992), undisclosed analysis flexibility (Simmons et al. 2011), p-hacking (Brodeur et al. 2016), and plain fraud (List et al. 2001, John et al. 2012). Ensuring that published results can be reliably reproduced is a necessary foundation for addressing these issues. While tackling the underlying reasons for limited replicability may be difficult, the ability to reproduce results based on the original data and analyses can be seen as a minimum criterion for scientific credibility to be expected from all published research (Christensen and Miguel 2018, Nagel 2018, Welch 2019). Indeed, if published results cannot be reproduced because data are unavailable or code used for data or numerical analysis is missing, poorly documented, or error-ridden, then the replicability crisis is partly also a reproducibility crisis.
In this study, we directly assess the reproducibility of results reported in nearly 500 research articles published in Management Science, a premier general interest academic journal that comprises 14 departments covering a broad variety of areas in business and management. In 2019, the journal introduced a new Policy for Data and Code Disclosure,1 which stipulates that “Authors of accepted papers…must provide…the data, programs, and other details of the experiment and computations sufficient to permit replication.” While our focus is primarily on assessing the reproducibility of work published since the disclosure policy went into effect, we also analyze articles accepted before May 2019 for comparison.
To reproduce results in articles from a variety of subfields of the journal such as finance, accounting, marketing, operations management, organizations, strategy, and behavioral economics, we use a crowd science approach (Nosek et al. 2012, Uhlmann et al. 2019) to leverage the expertise of many researchers in these different subfields. Overall, 733 volunteers joined the Management Science Reproducibility Collaboration as reproducibility reviewers (see Online Appendix A for all names and affiliations), who together reportedly spent more than 6,500hours on attempting to reproduce the results reported in the articles, using the replication materials and information provided by the article authors.
For articles subject to the 2019 disclosure policy, we find that when the reviewers obtained all necessary data (because they were included, could be accessed elsewhere, or no data were needed) and managed to meet the software and hardware requirements of the analysis, then results in the vast majority of articles (95%) were fully or largely reproduced.2 However, in approximately 29% of the articles, data sets were unavailable either because they were proprietary or under a non-disclosure agreement (NDA) or because they originated in subscription data services to which reviewers did not have access. If we consider all assessed articles under the disclosure policy, then about 68% could be at least largely reproduced. Because data availability was by far the largest obstacle to reproducing results, the methodology used in an article is strongly correlated to its reproducibility. Namely, computational and simulation studies and online and laboratory experiments are more likely to be reproducible than field experiments, surveys, and other empirical studies. These differences in methodology and data availability are also the main drivers for substantial heterogeneity in reproducibility across the 14 departments of the journal.
Comparing these results to the period before the introduction of the mandatory disclosure policy, we observe a substantial increase in reproducibility. When code and data disclosure was voluntary, only 12% of article authors provided replication materials. Out of these selected articles, 55% could be (largely) reproduced.
The share of fully and largely reproduced results in our study appears high, in particular considering that the code and data editorial team at the journal primarily assesses the completeness of replication materials but does not attempt reproduction of the results themselves. That said, in addition to limited data availability, some replication materials suffered from insufficient documentation, missing code, or errors in the code, making reproduction impossible. For some studies, reviewers obtained different results and were not able to make out the reasons for the discrepancies. This implies that there is still room for improvement. We discuss implications for disclosure policies and procedures at Management Science and other journals in Section 4 of this paper.
Our results complement findings in a recent literature on reproducibility and replicability in the social sciences. The definitions of these terms vary somewhat across studies, with some overlaps in their meaning (Christensen and Miguel 2018, Welch 2019, Dreber and Johannesson 2023, Pe´rignon et al. 2023). “Replication” typically refers to verifying the results of a study using different data sets and different methods, thus exploring the robustness of results. The term “computational reproducibility” comes closest to the scope of our study and is defined as the extent to which results in studies can be reproduced based on the same data and analysis as the original study. Other types of reproducibility may consider recreation of analysis and data or explore robustness to alternative analytical decisions (see also Dreber and Johannesson 2023, for an in-depth discussion).
Recent systematic replication attempts of published results in the social sciences yielded replication rates of 36% in psychology (Open Science Collaboration 2015, n=100), 61% in laboratory experiments in economics (Camerer et al. 2016, n=18), 62% in social science experiments published in Nature and Science (Camerer et al. 2018, n=21), and 80% in behavioral operations management studies published in Management Science (Davis et al. 2023, n=10).
In the field of economics, a number of studies targeting different subfields have set out to evaluate the computational reproducibility of results. The Journal of Money, Credit and Banking (JMCB) was one of the first journals to introduce a “data availability policy” and one of the first ones to be evaluated. Dewald et al. (1986) assess the first 54 studies subject to the policy. Only eight studies (14.8%) submitted materials that were deemed sufficient to attempt a reproduction, and only four of these studies could be reproduced without major issues. As the authors put it, “inadvertent errors…are a commonplace rather than a rare occurrence” (Dewald et al. 1986, p. 587). McCullough et al. (2006) examine JMCB articles published between 1996 and 2002 and successfully reproduce 22.6% of 62 examined works with a code and data archive, and only 7.5% considering all 186 relevant empirical articles in the journal. McCullough et al. (2008) report that for articles published between 1993 and 2003 in the Federal Reserve Bank of St. Louis Review, only 9 of 125 studies (7.2%) with an archive could be successfully reproduced.
One of the top journals in economics, the American Economic Review, introduced a data and code availability policy in 2004, and other top journals followed. In examining this policy for studies published between 2006 and 2008, Glandon (2011) reports that, among the studies with sufficient data archives, five of nine studies (55.6%) could be reproduced without major issues. Overall, however, only 20 of 39 sampled studies (51.3%) contained a complete archive, and for 8 studies (20.5%), reproduction was not feasible without contacting the authors.
More recently, Chang and Li (2017) attempted to reproduce articles in macroeconomics published between 2008 and 2013 across several leading journals and successfully reproduced 22 of 67 studies (32.8%). Gertler et al. (2018) examined the reproducibility of 203 empirical studies published in 2016 that did not contain proprietary or otherwise restricted data, and were able to reproduce 37% of them (but only 14% from the raw data). For 72% of the studies in the sample, code was provided but executed without errors in only 40% of the attempts. Herbert et al. (2023) ask undergraduate economics students to attempt to reproduce 303 studies published in the American Economic Journal: Applied Economics between 2009 and 2018. Only 162 studies contained non-confidential and non-proprietary data. For these, 68 reproduction attempts (42.0%) were successful and another 69 (42.6%) were deemed partially successful. Perignon et al. (2023) leverage a set of 168 replication packages produced in the context of an open science multianalyst study in empirical finance (Menkveld et al. 2023). Of 1,008 hypothesis tests across all materials, 524 (52.0%) were fully reproducible, with another 114 (11.3%) yielding only small differences to the original results.
Reproducibility studies in other related fields show similarly limited reproducibility. For a sample of 24 studies subject to the Quarterly Journal of Political Science’s data and code review, Eubank (2016) finds that only 4 (16.7%) did not require any modification in order to reproduce the results. In genetics, Ioannidis et al. (2009) report that only 8 of 18 microarray gene expression analyses (44.4%) were reproducible. An analysis of biomedical randomized controlled trials yields 14 of 37 (37.8%) successfully reproduced studies (Naudet et al. 2018). Artner et al. (2021) attempt to reproduce the main results from 46 published articles in psychology with the underlying data but no code and were successful in 163 of 232 statistical tests (70.3%). Xiong and Cribben (2023) examine the reproducibility of 93 articles using functional magnetic resonance imaging (fMRI) published in prominent statistics journals between 2010 and 2021, of which only 23 (24.7%) included the actual data set and 14 (15.1%) could be fully reproduced.
A comparison of reproducibility rates across different studies is difficult. Different studies often apply different definitions and standards of reproducibility, and reasons for non-reproducibility may differ between different journals due to different policies and enforcement procedures and different methods and data availability conditions in their fields. For example, our share of 95% of (largely) reproduced articles (conditional on data being available to the reviewer and hardware and software requirements being met) appears to be in a similar ballpark as the 85% of at least partially successful reproductions at the AEJ: Applied Economics. However, although both journals have similar disclosure policies, in the respective time periods, replication materials of articles at AEJ:AE only underwent a cursory review, whereas the code and data editorial team at Management Science checked all replication packages for completeness.
In recent years, there have been significant developments in the institutional arrangements for reproducibility of journal articles. For economics, Vlaeminck (2021) report that in a sample of 327 journals, 59% have data availability policies, a significant increase compared with 21% in the year 2014. Similar developments are present in the fields of business and management. For example, several other journals published by INFORMS have adopted similar code and data disclosure policies after Management Science took the lead in 2019. At the time of writing this paper, 20 of the 24 journals used for the University of Texas Dallas Business School rankings have a code/data disclosure policy, but only 10 made code/ data sharing compulsory, and only 2 have a code and data editor enforcing the policy. Colliard et al. (2023) discuss journals’ incentives with respect to reproducibility, and Hoffler (2017) provides evidence that, in economics, journals with disclosure policies are more often cited than journals without such policies.
The ability to reproduce results reported in published articles by executing the code on the data, both provided by the authors, does not, by itself, guarantee that results are replicable. However, it does provide a useful baseline. It increases confidence that reported results could, in principle, be replicated. Allowing access to original code and data also makes it possible for independent research teams to scrutinize robustness, conduct their own analysis including meta-analytical work spanning multiple studies and data sets, reuse code in other research, and either build on the results or design studies to show the limitations of original results. The ability to do this promotes scientific discourse, and importantly, also decreases incentives for academic fraud and data falsification.

<a href="https://drive.google.com/file/d/1DIls7Nd8yXHXceqti9sAZ28v9E6OkIej/view?usp=sharing" target="_blank"> **Read more** </a>

</span>