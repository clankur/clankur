# Hey, I'm Ankur!

An independent LLM researcher with experience in distributed systems and machine learning, currently investigating different approaches to shrink the KV Cache. Previously worked @ Microsoft and AWS.

## 🔬 Current Research

- **Reducing the KV Cache's Footprint**
  - Implemented a [Large Concept Model](https://github.com/clankur/lcm/blob/main/docs/lcm.ipynb) with jointly trained encoder/decoder for KV Cache compression
  - Explored [shared projection for K/V](https://github.com/clankur/muGPT/blob/da8b3e17bd16ce27ed88f7b5ff279ca380ba2409/docs/sharedkv.md) as an alternative to GQA
  - Implemented [multi-head latent attention](https://github.com/clankur/mla) and [MixAttention](https://github.com/clankur/mixatt) - two different approaches to shrink the KV Cache during inference
  - Identified [patterns between heads](https://github.com/clankur/sparsev/blob/main/analysis.ipynb) that sparsely accessed V without additional training
  - Investigated [calibrating cluster centers for Q/K](https://github.com/clankur/sparsev/blob/main/query_clustering_analysis.ipynb) to partition and sparsify KV Cache access

- **Hyperparameter Transfer**
  - Compared two different approaches for hyperparameter transfer described by [Yang et al. (2022)](https://arxiv.org/pdf/2203.03466) and [Everett et al. (2024)](https://arxiv.org/pdf/2407.05872) and reproduced Everett's findings that [standard parameterization with scaling exponents](https://github.com/clankur/muGPT/blob/main/docs/lr_transfer.ipynb) outperforms muP when scaling hyperparameters from 37m to 1b
  - Implemented [power scheduler](https://github.com/clankur/muGPT/tree/power_scheduler) from [Shen et al (2024)](https://arxiv.org/pdf/2408.13359) for batch size and training length optimization

- **Other work**
  - Implemented [Llama 3](https://github.com/clankur/muGPT/blob/0c1ebc8a228957ea13c19d83a69bfcfa7e30a07c/load_llama.py#L83C5-L83C15) and [Gemma 2](https://github.com/clankur/muGPT/blob/e898c82f9112994f880209e593219327b9039f7f/load_gemma.py) within muGPT
  - Designed a [synthetic benchmark](https://github.com/clankur/longbench) to assess the impact of position embeddings (RoPE, Alibi, CoPE, NoPE) and attention modifications (e.g., KV Cache reuse, multi-head latent attention) on long-context performance

## 💻 Technical Skills

- **Languages**: Python, C++, TypeScript
- **Frameworks**: JAX, Pallas, PyTorch, TensorFlow
- **Cloud & Infrastructure**: Google TPUs, AWS Lambda, CloudFormation
- **Areas of Expertise**: Transformers, Machine Learning Infrastructure, Distributed Systems

## 🎓 Education

- BS in Computer Science from University of Maryland @ College Park (2021)
  - Graduated in 3 years with President's Scholarship
- Thomas Jefferson High School for Science and Technology (2018)

[![clankur's GitHub stats](https://github-readme-stats.vercel.app/api?username=clankur)](https://github.com/anuraghazra/github-readme-stats)
