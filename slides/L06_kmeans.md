---
marp: true
theme: gaia
_class: lead
paginate: false
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.svg')
---

![bg left:40% 80%](../logo.png)

# **Feature Engineering**

## Nonlinear Manifold Feature Extraction


---

### Nonlinear manifolds

PCA is very useful when the data lies in a linear subspace, but what if the data forms a more complicated shape?

If a linear subspace is a flat sheet of paper, then a rolled up sheet of paper is a simple example of a **nonlinear manifold**.

If we could somehow unroll the Swiss roll, we’d recover the 2D plane. This is the goal of **nonlinear dimensionality reduction**, which assumes that the manifold is simpler than the full dimension it occupies and attempts to unfold it.

---
### Nonlinear manifolds

The key observation is that even when a big manifold looks complicated, *the local neighborhood around each point can often be well approximated with a patch of flat surface*.

Clustering algorithms can be seen as techniques for **local structure learning**. Points that are close to each other (where “closeness” can be defined by a chosen metric) belong to the same cluster. 

If the number of clusters is smaller than the number of features, then *the original data is compressed into a lower dimension*.

---

## k-Means Clustering

k-means is a clustering algorithm. Clustering algorithms group are **unsupervised** in that they do not require any sort of label: the algorithm’s job is to infer cluster labels based solely on the geometry of the data itself.

A clustering algorithm depends on a metric. The most popular metric is the *Euclidean distance*.

$$
|| x - y ||_2
$$

---

## k-Means Clustering

k-means establishes a hard clustering (one and only one cluster for each data point). The algorithm minimizes the total sum of the Euclidean distance between each data point and its cluster.

$$
\mathrm{min}_{C_1,\dots,C_k,\mu_1,\dots,\mu_k} \sum_{i=1}^{k} \sum_{x \in C_i} || x - \mu_i ||_2
$$

Each cluster $C_i$ contains a subset of data points and its center is:
$$ \mu_i = \sum_{x \in C_i} x/n_i  $$
