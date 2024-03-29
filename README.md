# Robust Confidence Sequences

This project contains example notebooks exhibiting confidence sequences that are robust, i.e., converge for observations with infinite variance.

  * [Robust Mean Demo](csrobustmean.ipynb): The basic technique for covering the running conditional mean in a nonstationary environment.  Includes the use of approximate sufficient statistics to bound space and time complexity.
  * [Off-Policy Quantile Demo](csnsopquantile.ipynb): Off-policy quantile identification functions can exhibit infinite variance (unlike the on-policy case).  In this case the importance weights are Pareto distributed with infinite variance: this might arise in a continuous action problem.
  * [Expectile Demo](csnsexpectile.ipynb): Expectile identification functions can exhibit heavy tails.  In this case the observation is Lognormal distributed.

## Key Papers

  * [Anytime-valid off-policy inference for contextual bandits](https://arxiv.org/abs/2210.10768): contains important background material on anytime valid off policy inference. 
 The running counterfactual mean is covered even with unbounded importance weights; but finite variance is assumed.
  * [A lower confidence sequence for the changing mean of non-negative right heavy-tailed observations with bounded mean](https://arxiv.org/abs/2210.11133): extends the previous paper to support adapting to an unknown moment $q \in (1, 2]$.
  * [Time-uniform confidence bands for the CDF under nonstationarity](https://arxiv.org/abs/2302.14248): extends the previous two papers to support covering the entire counterfactual CDF rather than just the mean.

## Contributing

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

## Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft 
trademarks or logos is subject to and must follow 
[Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/en-us/legal/intellectualproperty/trademarks/usage/general).
Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.
Any use of third-party trademarks or logos are subject to those third-party's policies.
