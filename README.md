# Data-generator

### Training

Run the following to generate KP instances in KP file (that had been created).
```
for i in {0..4}; do python3 generate_KP.py KP/3KP-10-$i.lp 10 3; done
```
to generate 4 instances

Run the following to generate samples for training GNN.
```
for i in {0..99}; do python3 -m moiptimiser ../tests/examples/zgenerator/KP/3KP-100-$i.lp; done
```
to generate 4 instances

