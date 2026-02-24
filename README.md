# FDEGNNFD
This repository contains the official implementation of the paper: "Embeddedness Theory-Driven Graph Neural Network: Fraud Detection in Multi-Relational Social Networks". The code implements a novel graph neural network framework guided by Granovetter's embeddedness theory to detect fraudulent behaviors in multi-relational social networks (e.g., review fraud, telecom fraud). The model integrates four key modules: heterogeneous edge filtering, feature decoupling, intra-relationship aggregation, and inter-relationship aggregation.
# Overview
Fraud detection in multi-relational social networks is challenging due to camouflage strategies, multi-relational feature confusion, and heterogeneous neighbor information. FDEGNNFD tackles these challenges through a theory-driven design based on structural, cognitive, informational, and relational embeddedness. The framework:
Purifies the graph by filtering cross-category spurious connections using adversarial learning (GraphGAN).
Decouples node features into shared common features and relation-specific features.
Aggregates neighbor information within each relation using a gating mechanism (for reliability) and attention (for importance).
Combines multi-relational representations by learning relationship importance weights adaptively.
Experiments on three real-world datasets (YelpChi, Amazon, Telecom) show state-of-the-art performance.
# Dataset Preparation
The code supports three datasets used in the paper:
YelpChi (hotel/restaurant reviews, 45,954 nodes, 14.5% fraud)
Amazon (musical instrument reviews, 11,944 nodes, 6.9% fraud)
Telecom (telecom call/SMS records, 6,106 nodes, 32.1% fraud)
