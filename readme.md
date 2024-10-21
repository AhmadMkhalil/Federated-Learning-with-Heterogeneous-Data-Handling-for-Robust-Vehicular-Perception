# Federated Learning with Heterogeneous Data Handling for Robust Vehicular Perception

Welcome to the official GitHub repository for the paper **"Federated Learning with Heterogeneous Data Handling for Robust Vehicular Perception,"** submitted to the **IEEE Intelligent Vehicles Symposium 2024**. This repository is a fork of the [original repository](https://github.com/TixXx1337/Federated-Learning-with-Heterogeneous-Data-Handling-for-Robust-Vehicular-Perception) by my co-author **Tizian Dege**, where we have implemented our novel federated learning approach tailored specifically for vehicular networks.

## Overview

This project focuses on addressing the key challenges of **Federated Learning (FL)** in autonomous driving systems, particularly in environments where data is not identically distributed among clients (i.e., non-IID data). As autonomous vehicles generate massive amounts of sensory data from cameras, LiDAR, and other sensors, FL offers a decentralized framework for training deep learning models without transferring raw data to a central server—preserving privacy and bandwidth.

### Key Contributions

- **FedProx+LA (Label-Aware)**: Our novel method, **FedProx+LA**, combines the strengths of **FedProx** and **FedLA** to handle data heterogeneity, making it especially effective in **vehicular networks**.
- **Heterogeneous Data Handling**: The proposed model is designed to address **quantity skew**, **label skew**, and other types of non-IID data distributions, which are common in real-world federated learning scenarios, particularly in vehicular systems.
- **30% Faster Convergence**: Both **FedLA** and **FedProx+LA** significantly improve the convergence speed of the model by 30% compared to baseline FL methods.
- **Improved Object Detection Performance**: FedProx+LA demonstrates substantial improvements in object detection performance, especially in scenarios with highly heterogeneous label distributions.

## Abstract

As fully autonomous driving technology advances, continual online model training becomes increasingly important to ensure the precision of perception models. Federated Learning (FL) within vehicular networks offers a robust framework for this purpose, allowing for model updates without transferring raw sensory data from vehicles. However, traditional FL methods struggle with non-identically distributed (non-IID) data, leading to slower convergence and suboptimal model performance.

In our previous work, we introduced **FedLA**, a Label-Aware aggregation method designed to address data heterogeneity in general FL settings. In this paper, we extend this by proposing **FedProx+LA**, a new FL method that builds on the foundations of **FedProx** and **FedLA** to effectively manage data heterogeneity in vehicular networks. Our evaluations show that **FedProx+LA** significantly outperforms both conventional and state-of-the-art methods in terms of convergence speed and detection accuracy, particularly when handling highly heterogeneous label distributions.

## Implementation Details

This repository contains the following key components:
- **Federated Learning Implementation**: Core code for simulating federated learning in a vehicular context, supporting various data distribution schemes.
- **FedLA and FedProx+LA Aggregation Methods**: Custom aggregation methods that tackle data heterogeneity, integrated into the FL framework.
- **Experiments on Real-World Datasets**: Object detection models trained on real-world datasets such as **KITTI**, **NuScenes**, and **COCO**, showcasing the application of FedProx+LA in continuous online learning scenarios.


## Future Work

- **Scalability Testing**: Extend our experiments to larger vehicular networks with more complex communication structures.
- **Integration with Edge Computing**: Explore the integration of FedProx+LA with real-time edge computing for real-world autonomous vehicle applications.
- **Data Privacy**: Investigate advanced privacy-preserving techniques, such as differential privacy and secure aggregation, to further enhance the security of federated learning in vehicular networks.

## Citation

If you find this work useful or use it in your research, please cite our paper:

```
@article{khalil2024federated,
  title={Federated Learning with Heterogeneous Data Handling for Robust Vehicular Object Detection},
  author={Khalil, Ahmad and Dege, Tizian and Golchin, Pegah and Olshevskyi, Rostyslav and Anta, Antonio Fernandez and Meuser, Tobias},
  journal={arXiv preprint arXiv:2405.01108},
  year={2024}
}
```



