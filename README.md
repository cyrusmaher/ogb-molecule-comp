# ogb-molecule-comp
This repository houses code for submission to the Open Graph Benchmark (OGB).

Results were submitted on September 21st, 2020 on behalf of Vir Biotechnology (www.vir.bio).

This submission focuses on two competitions related to molecular classification.

These are:
- ogb-molhiv (~40,000 compounds, one classification task)
- ogbg-molpcba (~430,000 compounds, 128 classification tasks)

For more information, see the graph classication datasets page on OGB:
https://ogb.stanford.edu/docs/graphprop/#ogbg-mol

Our aim with this submission is to establish a baseline for graph neural network
performance by demonstrating the performance of Morgan fingerprints combined
with untuned Random Forest classification.

# Results
For the ogb-molhiv competition, ROC AUC was 0.842 ± 0.003 on the validation set.
On the test set, ROC AUC was 0.806 ± 0.001. At the time of submission,
this resulted in a first place leaderboard standing.

For the ogbg-molpcba, average precision (AP) was 0.222 ± 0.0002 on the validation set.
Test set AP was 0.205 ± .0003. This was sufficient for fifth place standing
at the time of submission.

# Reproducibility
Below is the output of `conda list`
```
numpy                     1.18.5           py37ha1c710e_0
ogb                       1.2.2                    pypi_0    pypi
pandas                    1.1.0                    pypi_0    pypi
rdkit                     2020.03.3.0      py37hc20afe1_1    rdkit
tqdm                      4.48.2                     py_0
typing                    3.7.4.3                  pypi_0    pypi
scikit-learn              0.22.2.post1             pypi_0    pypi
```
Code was run on python 3.7.7.
