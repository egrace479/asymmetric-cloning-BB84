# Asymmetric Phase-Covariant Cloning to Eavesdrop on BB84

This repository contains the continuation of the QuForce Innovation Fellows Project: [Asymmetric Cloning to Eavesdrop on BB84 Protocol](https://github.com/egrace479/QuForceBB84Proj), which was completed by Elizabeth Campolongo, Brian Pigott, and Hardik Routray with advice from Alex Khan. The original project was selected for 1st Place on Demo Day in August 2022, slides available on [the original project repo](https://github.com/egrace479/QuForceBB84Proj/blob/main/EGC_BP_HR_Asymmetric_Cloning_to_Eavesdrop_on_BB84_Protocol.pdf), recording of Demo Day and more information on QuForce is available in this [Quantum Insider Article](https://thequantuminsider.com/2022/08/22/quforce-emerging-as-worlds-leading-community-for-post-quantum-cryptography-experts-academics-enthusiasts/). Our paper on these results, _Eavesdropping on the BB84 Protocol using Phase-Covariant Cloning: Experimental Results_,  is available on [arXiv](https://doi.org/10.48550/arXiv.2409.16284).

The BB84 protocol is known to be a secure method of quantum key distribution, even in the case when an eavesdropper has unlimited resources at their disposal. However, the security of the protocol is only obtained below the level of noise that occurs in the quantum channel. The purpose of this project is twofold:

1. Develop an optimal strategy for an eavesdropper who is using asymmetric cloning; that is, develop and implement a strategy that gives the eavesdropper maximum information about the channel while minimizing the disturbance to the signal.

2. Consider the Quantum Bit Error Rate (QBER) in a lossy quantum channel with the presence of the eavesdropping strategy developed in (1) and implement error-correcting algorithms to derive a secure key.

Here we develop a reproducible test to determine the security--or lack thereof--of the BB84 protocol in practice. With this test, we measure how much information an eavesdropper can obtain about a raw key when transmitted under the BB84 protocol using the optimal  eavesdropping approach (asymmetric phase-covariant cloning).
Here we provide the code used in running [experiments](experiments) simulating BB84, which we implemented on the IonQ Harmony quantum computer, to uncover these quantities
Thus we obtain an experimental estimate of the information that can be gained by an adversary using asymmetric phase-covariant cloning to eavesdrop on the BB84 protocol.
