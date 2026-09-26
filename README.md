# MUSE

**Revisiting Diffusion Fine-Tuning for Unsupervised Domain Adaptation**

Accepted at **NeurIPS 2026**.

Xuan Qi, Yi Wei, Daniele Berardini, Vito Paolo Pastore, Vittorio Murino

Istituto Italiano di Tecnologia · University of Genoa · Nanjing University · University of Verona

[Project page](https://xuanqi99.github.io/MUSE/) · [GitHub](https://github.com/xuanqi99/MUSE)

## Overview

MUSE (**Multi-target UDA-oriented Synthesis with Efficient diffusion fine-tuning**) is a parameter-efficient diffusion adaptation framework for multi-target data generation in unsupervised domain adaptation (UDA). It reuses one source-guided diffusion fine-tuning process to generate target-specific synthetic training data for multiple unlabeled target domains.

## Method

- **Shared semantics:** a shared semantic branch learns class information from labeled source data.
- **Target-specific styles:** lightweight private style branches capture the appearance of individual target domains.
- **Decoupled optimization:** separate semantic and style adaptation reduces cross-target interference and avoids repeating source-guided fine-tuning for every target.

Experiments on **Office-31, Office-Home, and miniDomainNet** show improved average target-domain accuracy and reduced diffusion fine-tuning cost compared with repeated per-target diffusion adaptation.

## Citation

```bibtex
@inproceedings{qi2026muse,
  title={Revisiting Diffusion Fine-Tuning for Unsupervised Domain Adaptation},
  author={Qi, Xuan and Wei, Yi and Berardini, Daniele and Pastore, Vito Paolo and Murino, Vittorio},
  booktitle={Advances in Neural Information Processing Systems},
  year={2026},
  url={https://github.com/xuanqi99/MUSE}
}
```
