# Gibbs Prior Diagnostics

Code for the AISTATS 2022 paper titled "Discovering Inductive Bias with Gibbs Priors: A Diagnostic Tool for Approximate Bayesian Inference" by Luca Rendsburg, Agustinus Kristiadi, Philipp Hennig, and Ulrike von Luxburg.

## Setting up:

1. Install CUDA >=11 and CuDNN >=8.2: <https://gist.github.com/kmhofmann/cee7c0053da8cc09d62d74a6a4c1c5e4>.
2. Install Miniconda: <https://docs.conda.io/en/latest/miniconda.html>.
3. Create a virtual environment: `conda create --name {ENV_NAME} --file requirements.txt`, for an arbitrary `{ENV_NAME}`.
4. Activate: `conda activate {ENV_NAME}`.


## Reproducing the paper's results:
1. Choose a folder in experiments/ to reproduce the experiments for the log-normals model in Section 5.1 (experiments/log_normal),
   for the volatility model in Section 5.2 (experiments/volatility), for the baseline (experiments/baseline), or for convergence monitoring
   (experiments/convergence)
2. Run the `run_%.ipynb` file(s) to generate the data, which are saved in the corresponding folder in `results/`
3. Run the `eval_%.ipynb` file to create the figures used in the paper.

## Citing the paper:

```
@inproceedings{rendsburg2022gibbs-prior,
  title={Discovering Inductive Bias with {G}ibbs Priors: A Diagnostic Tool for Approximate {B}ayesian Inference},
  author={Rendsburg, Luca and Kristiadi, Agustinus and Hennig, Philipp and von Luxburg, Ulrike},
  booktitle={AISTATS},
  year={2022}
}
```
