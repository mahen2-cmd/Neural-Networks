# Neural networks from scratch (NumPy)

A fully connected neural network written with NumPy only: forward pass, backpropagation (hand-derived gradients), gradient descent, MSE loss and a learning-rate scheduler, trained on a 2D regression dataset (`data2D.csv`).

It starts from a single neuron (a perceptron) and builds up. The notebook records what I learned along the way:
- why ReLU outputs can't go negative and how a neuron that falls too far negative stops learning ("dying ReLU"),
- how easily training gets stuck in a local minimum when every weight moves at once,
- why initialisation matters (He initialisation).

`nn_from_scratch.ipynb` is the main notebook; `nn_from_scratch2.ipynb` is a cleaner second version.

Stack: Python, NumPy, Matplotlib.

## How to run

```bash
pip install numpy matplotlib tqdm jupyter
jupyter notebook nn_from_scratch.ipynb
```

Run the cells top to bottom. `data2D.csv` is included.
