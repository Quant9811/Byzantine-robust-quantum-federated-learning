# Byzantine-robust-quantum-federated-learning
Circular versus Euclidean aggregation for Byzantine-robust quantum federated learning: a paired, geometry-controlled benchmark
This repository contains the Jupyter notebook for a geometry-controlled benchmark of Euclidean and circular robust aggregation methods in a variational-quantum-circuit (VQC) federated-learning setting.

The study investigates whether respecting the periodicity of VQC rotation parameters can affect aggregation behaviour under Byzantine and other adversarial conditions. It compares paired Euclidean and circular aggregation rules, evaluates a collection of attacks, and studies the effects of Byzantine fraction, data heterogeneity, circuit configuration, dataset, client count, and parameter/state-change diagnostics.
Reproducibility note: The notebook's default paper profile currently uses five seeds and ten communication rounds. These settings reproduce the configuration encoded in the notebook; they should not be interpreted as a claim of sufficient statistical power for every inferential comparison. See the statistical limitations discussed in the manuscript.
Repository contents
- Quantum_Science_and_Technology_Journal_Ready(Circular_Vs_Euclidean_Aggregators_in_QFL_setting)_(2).ipynb — main experiment notebook.
- requirements.txt — Python dependencies.
- README.md — setup and execution instructions.
- The notebook creates its result directories and CSV logs automatically.
Requirements
- Python 3.10 or newer is recommended.
- A Jupyter environment (Jupyter Notebook, JupyterLab, or Google Colab).
- The Python packages listed in requirements.txt.
The simulations use PennyLane devices (default.qubit for ideal state-vector simulation and default.mixed when depolarising noise is enabled). The notebook uses scikit-learn's built-in breast-cancer, wine, and digits datasets; no separate dataset download is required.
Running the notebook
Run the notebook cells in order, from top to bottom. The notebook defines the model, data partitioning, attack functions, aggregation methods, experiment runner, statistical summaries, and plots in earlier cells; later cells execute the studies and analyse their outputs.
