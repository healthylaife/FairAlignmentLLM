# Aligning (Medical) LLMs for (Counterfactual) Fairness

Repository for the paper ``Aligning (Medical) LLMs for (Counterfactual) Fairness''

Our repository is divided into two parts: eval, and mitigation.

![framework](https://github.com/healthylaife/FairAlignmentLLM/blob/main/images/framework.png)
The eval folder contains the code required to run the evaluation framework for each dataset presented in the paper.


![diagram](https://github.com/healthylaife/FairAlignmentLLM/blob/main/images/diagram.png)
The mitigation folder contains the code to align the LLMs for counterfactual fairness. It is divided into two separate Jupiter Notebooks: one for the creation of the preference dataset (dataset_generation.ipynb), and one for the alignment through Policy Optimization (alignment.ipynb).
Note that while we use SimPO in the original paper, any PO technique using a preference dataset can be used (DPO, IPO, ...). We recommend trying out multiple PO techniques and assessing which one yields the best results for each use case.
