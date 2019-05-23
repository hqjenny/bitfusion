# Setup Steps 

## 1. Setup simulator 
```
git clone --recursive git@github.com:hqjenny/bitfusion.git
git clone https://github.com/hsharma35/dnnweaver2.git
cp -r dnnweaver2/dnnweaver2 bitfusion/
cd bitfusion
export PYTHONPATH=`pwd`/dnnweaver2:${PYTHONPATH}
cd sram/cacti
make
```

## 2. Add Network Configuration 
Add the model configuration in `bitfusion/src/benchmarks/benchmarks.py`.

## 3. Run the IPython Notebook
First remove the result file `rm bitfusion/results/bitfusion-eyeriss-sim-sweep.csv` then run the IPython Notebook.
The result is store in `bitfusion/results/bitfusion-eyeriss-sim-sweep.csv`, the script does not run if the result file exists.

 
