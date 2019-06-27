# scAlign
A deep learning-based tool for alignment and integration of single cell genomic data across multiple datasets, species, conditions, batches

## Tutorials

[Unsupervised alignment and projection of HSCs](https://github.com/quon-titative-biology/examples/blob/master/scAlign_paired_alignment/scAlign_kowalcyzk_et_al.md)

[Multiway alignment using all pairs method](https://github.com/quon-titative-biology/examples/blob/master/scAlign_multiway_alignment/scAlign_multiway_pancreas.md)

[Supervised/Semi-supervised alignment](https://github.com/quon-titative-biology/examples/blob/master/scAlign_supervised_alignment/scAlign_supervised_alignment.md)

## Updates

#### (5/9/2019) Updated to version 1.0! Tutorials for multiple modes of operation now available. 

## R Package and Bioconductor

Bioconductor for now will only support the Linux version of scAlign. For Windows and Mac please download/install the package directly from [github](https://github.com/quon-titative-biology/). 

```
install.packages('devtools')
devtools::install_github(repo = 'quon-titative-biology/scAlign')
library(scAlign)
```

## Package requirements

Guide to installing python and tensorflow on different operating systems.

### On Windows:
1. Download Python 3.6.8. Note, newer versions of Python (e.g. 3.7) cannot use TensorFlow at this time. 
2. Make sure pip is included in the installation.
3. Open Windows Command Prompt, or PowerShell.
4. Navigate to your Python installation directory (for Windows 10, the default seems to be C:\Users\userid\AppData\Local\Programs\Python\Python36\Scripts, where userid is your own username).
5. Run .\pip install --upgrade tensorflow

### On Ubuntu:
1. sudo apt update
2. sudo apt install python3-dev python3-pip
3. pip3 install --user --upgrade tensorflow  # install in $HOME
4. python3 -c "import tensorflow as tf; tf.enable_eager_execution(); print(tf.reduce_sum(tf.random_normal([1000, 1000])))"

### On MacOS (homebrew):
1. /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
2. export PATH="/usr/local/bin:/usr/local/sbin:$PATH"
3. brew update
4. brew install python  # Python 3
5. pip3 install --user --upgrade tensorflow  # install in $HOME
6. python3 -c "import tensorflow as tf; tf.enable_eager_execution(); print(tf.reduce_sum(tf.random_normal([1000, 1000])))"

Further details at: https://www.tensorflow.org/install
