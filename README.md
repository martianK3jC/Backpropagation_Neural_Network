# Backpropagation Neural Network - 4-Input AND Gate
IS1 Assignment

## Experiment results

### Configuration
- Input neurons: 4
- Output neurons: 1
- Gate type: AND (output 1 only when all inputs are 1)

### Finding Minimum Hidden Neurons

| Hidden Neurons | Epochs | (1,1,1,1) Output | (0,0,0,0) Output | Result   |
|----------------|--------|------------------|------------------|----------|
| 10             | 3000   | 0.915            | 0.000            | ✅ Works |
| 8              | 3000   | 0.912            | 0.000            | ✅ Works |
| 6              | 3000   | 0.903            | 0.000            | ✅ Works |
| 4              | 3000   | 0.900            | 0.000            | ✅ Works |
| 2              | 3000   | 0.873            | 0.000            | ⚠️ Works (borderline)|
| 1              | 3000   | 0.838            | 0.003            | ⚠️ Works (borderline)|

**Minimum Hidden Neurons: 4 (much more stable)**

### Finding Minimum Epochs
(Using 4 hidden neurons)
| Epochs | (1,1,1,1) Output | (0,0,0,0) Output | Result      |
|--------|------------------|------------------|-------------|
| 5000   | 0.921            | 0.000            | ✅ Works    |
| 4000   | 0.927            | 0.000            | ✅ Works    |
| 3000   | 0.906            | 0.000            | ✅ Works    |
| 2000   | 0.831            | 0.000            | ⚠️ Works (borderline)|
| 1000   | 0.255            | 0.013            | ❌ Failed   |
| 500    | 0.127            | 0.043            | ❌ Failed   |

**Minimum Epochs: 2000**
