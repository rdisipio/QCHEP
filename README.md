# Quantum Computing HEP applications

Install and Setup
=================

Create virtual environment based on python3
```
module load python/3.7.0
virtualenv env-qc
source env-qc/bin/activate
```

Install Cirq from https://github.com/quantumlib/Cirq

```
git clone https://github.com/quantumlib/Cirq.git
cd Cirq
python setup.py install
```

Lots of dependencies: numpy, scipy, matplotlib, etc..

Does it work?

```
python -c 'import cirq; print(cirq.google.Foxtail)'

(0, 0)───(0, 1)───(0, 2)───(0, 3)───(0, 4)───(0, 5)───(0, 6)───(0, 7)───(0, 8)───(0, 9)───(0, 10)
│        │        │        │        │        │        │        │        │        │        │
│        │        │        │        │        │        │        │        │        │        │
(1, 0)───(1, 1)───(1, 2)───(1, 3)───(1, 4)───(1, 5)───(1, 6)───(1, 7)───(1, 8)───(1, 9)───(1, 10)
```

A bit more advanced example is found in ```hello_qbit.py```. More examples: https://github.com/quantumlib/Cirq/tree/master/examples
