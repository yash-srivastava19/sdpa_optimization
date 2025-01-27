# SDPA Optimization
Scripts and Notebooks for my blog on "SDPA Optimization Case Study - A Worklog"
Link to the original blog [here](https://yash-sri.xyz/blog/sdpa_optim)

## Introduction
*Excerpt taken from the original blog*

In my FlexAttention [blog](https://yash-sri.xyz/blog/flex_attention), I explained in detail how the straightforward implementation of SDPA has quadratic compute and memory complexity with respect to sequence length. It is because of these bottlenecks, using optimized version of SDPA such as Flash Attention or Flex Attention are preferred for deployment. 

While I was working on the FlexAttention blog, and was beginning to understand how each approach optimized the standard SDPA(or different variants of SDPA), especially from memory constraints, I **found three different directions which I should explore** and experiment which is the most promising amongst them - which are cache, quantizations, and device specific optimizations.

## Resources
Linked in this repository are jupyter [notebook](https://www.kaggle.com/code/yashsrivastava51213/sdpabenchmarking) used to perform experiment. I'm also plaaning on adding standalone CLI scripts to perform the experiments too.
