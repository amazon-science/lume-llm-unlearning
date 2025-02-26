# LUME: LLM Unlearning with Multitask Evaluations

<p align="center">
    <a href="http://arxiv.org/abs/2502.15097"><img src="https://img.shields.io/badge/paper-arXiv-red" alt="Paper"></a>
        <img src="https://img.shields.io/github/license/amazon-science/ssepy" alt="Apache-2.0">
</p>

Unlearning is a promising line of research for LLM safety since it can be used to remove a variety of sensitive information from LLMs’ parametric memory such as toxic/unsafe/biased/creative content, as well as private information (pertaining to either individuals or institutions). Effective unlearning avoids expensive (and often infeasible) retraining of the model from scratch without the corresponding training data samples. However, this line of research is still in a relatively nascent stage, and there is a need for benchmarks which can provide thorough evaluations of new unlearning algorithms in removing different categories of sensitive information. Towards this goal, we develop and release a comprehensive new benchmark named LUME (LLM Unlearning with Multitask Evaluations) for unlearning creative, sensitive, and private content from LLMs.

## Benchmark

<p align="center"><img src="https://github.com/amazon-science/lume-llm-unlearning/blob/main/examples.png?raw=true" width="700" height="470"></p>

Our benchmark includes three distinct tasks to provide a comprehensive evaluation of LLM unlearning algorithms spanning creative documents, PII and biographies. 

- Task 1: Synthetic creative documents
- Task 2: Synthetic biographies with sensitive PII
- Task 3: Real biographies

For each of these tasks, we create prompts for regurgitation and knowledge tests. We split our benchmark into forget and retain sets (in 1:1 ratio) and also release two model checkpoints (7B and 1B parameters) fine-tuned to memorize this dataset.

## Citation

If you use this benchmark in your research, please cite this paper:

```bibtex
@article{ramakrishna2025lumellmunlearningmultitask,
      title={LUME: LLM Unlearning with Multitask Evaluations}, 
      author={Anil Ramakrishna and Yixin Wan and Xiaomeng Jin and Kai-Wei Chang and Zhiqi Bu and Bhanukiran Vinzamuri and Volkan Cevher and Mingyi Hong and Rahul Gupta},
      journal={arXiv preprint arXiv:2502.15097},
      year={2025},
}
```

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This project is licensed under the Apache-2.0 License.

