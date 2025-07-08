# Scripts, Modules, and Packages

1. Overall Structure
* Many different steps for a simulation or in a data analysis pipeline
  - loading the data file
  - extracting data
  - analysis part
  - visualization
  - saving results
  => Separate entities according to their functions (modularization or refactoring)

2. Classes
* Encoding a sequence with a dictionary

```python
NT = ['A','C','G','T']
Code = [[1,0,0,0],[0,1,0,0],[0,0,1,0],[0,0,0,1]]
Dict = {key: value for key, value in zip(NT, Code)}
Encoder = lambda Sequence: [Dict[s] for s in Sequence]
```
```python
Class EncodeMySeq():
  # reading and converting the sequence when we call the class
  def __init__(self ,Seq):
    self.E = np.array(Encoder(Seq)).transpose()
  # creating the plot by calling the plot routine
  def PlotMySeq(self):
    MyPlotRoutine(self.E, Seq)
    # don't forget the input arguments!
```

3. Let's build a Package!
* Goal: modelling the motiion of particles in a Lennard-Jones potential U_LJ
