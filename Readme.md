# A Comprehensive Analysis of Social Tie Strength: Definitions, Prediction Methods, and Future Directions

[![Awesome](https://awesome.re/badge.svg)](https://github.com/XueqiC/Awesome-Tie-Strength-Prediction) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/XueqiC/Awesome-Tie-Strength-Prediction/blob/main/LICENSE)
![](https://img.shields.io/badge/PRs-Welcome-red) 

## Introduction
The rapid growth of online social networks has underscored the importance of understanding the intensity of user relationships, referred to as ``tie strength." Over the past few decades, extensive efforts have been made to assess tie strength in networks. However, the lack of ground-truth tie strength labels and the differing perspectives on tie strength among researchers have complicated the development of effective prediction methods for real-world applications. 

In our study, we first categorize mainstream understandings of tie strength into seven standardized definitions and verify their effectiveness by investigating the class distributions and correlations across these definitions. We also draw key insights into tie resilience from the perspective of tie dissolution that (1) stronger ties are more resilient than weaker ones, and (2) this tie resiliency ratio increases as the network evolves. We then conduct extensive experiments to evaluate existing tie strength prediction methods under these definitions, revealing that (1) neural network methods capable of learning from semantic features hold great potential for high performance, (2) models struggle under definitions that offer limited understandings of tie strength in the network, (3) existing models face imbalance issues that cannot be addressed by traditional quantity imbalance techniques, and (4) different definitions of tie strength allow for the inference of not only the current state but also the future state of a tie. Building on these findings, we propose strategies to improve existing methods and suggest several promising directions for future research.

## Run the code
- To run the heurstic random forest experiments, please check the code in 'rf.sh'.
- To run the MLP experiments, please check the code in 'mlo.sh', where MLP is with edge features and MLP2 is without edge features.
- To run the GCN experiments, please check the code in 'gcn.sh'.
- To run the GTN experiments, please check the code in 'tran.sh'.
- `greedy.sh' is for the STC-greedy experiments, with the prediction results generated from this [STC-Greedy matlab code](https://bitbucket.org/ghentdatascience/stc-code-public/src/master/). 

## License
MIT License

## Contact 
Please feel free to email me (xueqi.cheng [AT] vanderbilt.edu) for any questions about this work.

## Citation
```
@article{cheng2024comprehensive,
  title     = {A Comprehensive Analysis of Social Tie Strength: Definitions, Prediction Methods, and Future Directions},
  author    = {Cheng, Xueqi and Yang, Catherine and Zhao, Yuying and Wang, Yu and Karimi, Hamid and Derr, Tyler},
  journal   = {arXiv preprint arXiv:2410.19214},
  year      = {2024}
}
```