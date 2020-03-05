---
title: 'MPA: An accessible and robust cross-language implementation of the Matrix Profile'
tags:
  - Python
  - R
  - Golang
  - Time Series
  - Machine Learning
  - Data Science
authors:
  - name: Andrew H. Van Benschoten
    orcid: 
    affiliation: 1
  - name: Austin Ouyang
    affiliation: 1
  - name: Francisco Bischoff
    affiliation: 1
  - name: Tyler W. Marrs
    affiliation: 1
affiliations:
 - name: Matrix Profile Foundation
   index: 1

date: 4 March 2020
bibliography: paper.bib

---

# Summary
Two fundamental time-series tasks are identifying anomalous events (“discords”) and repeated patterns (“motifs”). Understanding how to accomplish these tasks is of the utmost importance across a myriad of disciplines, where accurate solutions can generate millions of dollars in profit, prevent catastrophic system failures or unlock novel technological abilities. While there are dozens of existing approaches for finding motifs and discords, they are nearly all limited by a steep learning curve, have numerous parameters that require tuning or scale poorly when applied to large datasets. These challenges have been compounded by the explosive growth of the data science community, where more practitioners possess backgrounds lacking advanced mathematical and statistical experience. Thus, there is a need for a more approachable solution to this question (note: finish this statement of need).

The Matrix Profile (a data structure & set of associated algorithms developed by the Keogh research group at UC-Riverside) is a powerful tool to help solve this dual problem of anomaly detection and motif discovery, as Matrix Profile is robust, scalable, and largely parameter-free.

Although the Matrix Profile can be a game-changer for time series analysis, leveraging it to produce insights is a multi-step computational process, where each step requires some level of domain experience. There are three facets that will make this code accessibile to the broader community: “out-of-the-box” working implementations, gentle introductions to core concepts that can naturally lead into deeper exploration, and multi-language accessibility.

The Matrix Profile API (MPA) is a common codebase written in R, Python and Golang that achieves all three of these goals. To parallel the natural flow of using the Matrix Profile, MPA consists of three core components: 1) _Compute_ (computing the Matrix Profile), 2. _Discover_ (evaluate the MP for motifs, discords, etc) and 3. _Visualize_ (display results through basic plots) These three capabilities are wrapped up into a high-level capability called _Analyze_. This is a user-friendly interface that enables people who know nothing about the inner workings of Matrix Profile to quickly leverage it for their own data. And as users gain more experience and intuition with MPA, they can easily dive deeper into any of the three core components to make further functional gains.

Other topics: pan-MP, code performance, etc.

# Mathematics

Single dollars ($) are required for inline mathematics e.g. $f(x) = e^{\pi/x}$

Double dollars make self-standing equations:

$$\Theta(x) = \left\{\begin{array}{l}
0\textrm{ if } x < 0\cr
1\textrm{ else}
\end{array}\right.$$

You can also use plain \LaTeX for equations
\begin{equation}\label{eq:fourier}
\hat f(\omega) = \int_{-\infty}^{\infty} f(x) e^{i\omega x} dx
\end{equation}
and refer to \autoref{eq:fourier} from text.

# Citations

Citations to entries in paper.bib should be in
[rMarkdown](http://rmarkdown.rstudio.com/authoring_bibliographies_and_citations.html)
format.

If you want to cite a software repository URL (e.g. something on GitHub without a preferred
citation) then you can do it with the example BibTeX entry below for @fidgit.

For a quick reference, the following citation commands can be used:
- `@author:2001`  ->  "Author et al. (2001)"
- `[@author:2001]` -> "(Author et al., 2001)"
- `[@author1:2001; @author2:2001]` -> "(Author1 et al., 2001; Author2 et al., 2002)"

# Figures

Figures can be included like this:
![Caption for example figure.\label{fig:example}](figure.png)
and referenced from text using \autoref{fig:example}.

Fenced code blocks are rendered with syntax highlighting:
```python
for n in range(10):
    yield f(n)
```	

# Acknowledgements

The authors would like to thank their fellow Matrix Foundation board members Jack Green and Frankie Cancino, as well as Eamonn Keogh, Abdullah Mueen and their numerous graduate students for creating the Matrix Profile and continuing to drive its development.

# References
