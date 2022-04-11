# Data-generator

### Training

Run the following to generate KP instances in KP file (that had been created). (cd tests/examples/zgenerator)
```
for i in {0..4}; do python3 generate_KP.py KP/3KP-10-$i.lp 10 3; done
```
to generate 4 instances

Run the following to generate samples for training GNN. (cd src)
```
for i in {0..99}; do python3 -m moiptimiser ../tests/examples/zgenerator/KP/3KP-100-$i.lp; done
```


Run the following to train GNN. (cd src)
```
python3 branch2learn_cl/02_train.py -p KP -m "gin1"
```



### Testing

Run the following to test an algorithm which is chosen in "cli.py". (cd src)
```
python3 -m moiptimiser ../tests/examples/zgenerator/KP/3KP-100-3.lp
```




