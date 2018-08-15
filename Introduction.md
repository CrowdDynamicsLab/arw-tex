# Introduction

## What is the problem?

In this paper, we present a network growth model that explains how distinct structural properties of attributed networks can emerge from local edge formation processes. In real-world networks, individuals tend to form edges under resource constraints such as limited information and partial network access. Additionally, sociological phenomena such as triadic closure and homophily \textit{simultaneously} impact individuals’ decisions to form edges. Over time, these decisions cumulatively shape real-world networks as they exhibit rich structural characteristics: heavy-tailed indegree distribution, skewed local clustering and homophilic mixing patterns. However, we lack mechanisms that incorporate the effect of resource constraints and \textit{multiple} sociological factors on edge formation as well as preserve global network structure.

## Why is it important?

Existing models of network growth tend to make unrealistic assumptions about how individuals form edges. Consider a simple stylized example: the process of finding a set of papers to cite when writing an article. In preferential attachment \cite{barabasi1999emergence} or fitness \cite{X} based models, a node making $m$ citations would pick papers from the \textit{entire} network in proportion to their indegree or fitness respectively. This process assumes that individuals possess complete knowledge of indegree or fitness of every node in the network. An equivalent formulation — vertex copying \cite{X} — induces preferential attachment: for every citation, a node would pick a paper uniformly at random from \textit{all} papers, and either cite it or copy its citations. Notice that the copying mechanism assumes individuals have complete access to the network and form each edge independently. Although these models explain the emergence of power law degree distributions, they are unrealistic representations of how individuals make decisions about edge formation. A realistic representation of how individuals form edges necessitates modeling the effect of multiple sociological phenomena on edge formation under resource constraints.

## Why is the problem hard?

The problem of developing a model of network growth, where individuals act under resource constraints, including access to only local information is hard. The problem lies in identifying simple mechanisms with few parameters that unifies multiple sociological phenomena to \textit{jointly} preserve structural properties and attribute mixing patterns of attributed networks.

#### Contributions

We propose an Attributed Random Walk \texttt{ARW} model that jointly explains
the emergence of in-degree distributions, local clustering, clustering-degree
relationship and attribute mixing patterns through a resource constrained mechanism
based on random walks.
In \texttt{ARW}, incoming nodes select a seed node based on attribute similarity
and initiate a biased random walk: At each step of the walk, the incoming node either
jumps back to its seed or chooses an outgoing link or incoming link to visit another
node. It links to each visited node with some probability and halts after forming a
few connections. We have three primary contributions:
\begin{itemize}
\item model effect of multiple sociological phenomena on edge formation simulatenously
\item provide a realistic representation of how individuals form edges under constraints of limited information and partial network access.
\item jointly preserve key structural properties and attribute mixing patterns of real-world attributed networks.
\end{itemize}

This paragraph discusses expriment and results.

This is the ToC paragraph.
