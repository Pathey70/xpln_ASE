# xpln_ASE
[![Unit tests](https://github.com/Pathey70/xpln_ASE/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/Pathey70/xpln_ASE/actions/workflows/unit-tests.yml)
[![DOI](https://zenodo.org/badge/606823743.svg)](https://zenodo.org/badge/latestdoi/606823743)



# HW 6 XPLN


### Contributors

- Pathey Shah
- Prit Modi
- Nikhil Mehra


## Instructions


- To view all command line options run 
    ```python3 Main.py --help True ```

- To Run test cases 
    ```python3 Main.py --go <test-name>```


    e.g.
    
    ```python3 Main.py --go xpln```
 

```
Here are the list of options

  
OPTIONS:
  -b  --bins    initial number of bins       = 16
  -c  --cliffs  cliff's delta threshold      = .147
  -d  --d       different is over sd*d       = .35
  -f  --file    data file                    = ../etc/data/auto93.csv
  -F  --Far     distance to distant          = .95
  -g  --go      start-up action              = nothing
  -h  --help    show help                    = False
  -H  --Halves  search space for clustering  = 512
  -m  --min     size of smallest cluster     = .5
  -M  --Max     numbers                      = 512
  -p  --p       dist coefficient             = 2
  -r  --rest    how many of rest to sample   = 4
  -R  --Reuse   child splits reuse a parent pole = True
  -s  --seed    random number seed           = 937162211
ACTIONS:



  

```

## To run all test cases

```python3 Main.py --go  all ```

## Output
```
all			best:14, rest:56

Clndrs -inf 4 0.72 {'best': 14, 'rest': 22}
Clndrs 4 inf 0.0 {'rest': 34}

Volume -inf 90 0.42 {'best': 7, 'rest': 5}
Volume 90 116 0.19 {'best': 4, 'rest': 8}
Volume 116 141 0.15 {'best': 3, 'rest': 5}
Volume 141 inf 0.0 {'rest': 38}

Model -inf 71 0.0 {'rest': 4}
Model 71 73 0.02 {'best': 1, 'rest': 11}
Model 73 74 0.4 {'best': 6, 'rest': 2}
Model 74 75 0.34 {'best': 6, 'rest': 6}
Model 75 77 0.02 {'best': 1, 'rest': 13}
Model 77 inf 0.0 {'rest': 20}

origin 1 1 0.0 {'rest': 39}
origin 2 2 0.85 {'best': 14, 'rest': 10}
origin 3 3 0.0 {'rest': 7}
✅PASS : eg_bins
> 1.0 False
> 1.02 False
> 1.05 False
> 1.08 False
> 1.1 False
> 1.13 False
> 1.16 False
> 1.19 False
> 1.22 True
✅PASS : eg_cliffs
{'Lbs-': 2970.4, 'Acc+': 15.6, 'Mpg+': 23.8}
{'Lbs-': 2970.4, 'Acc+': 15.6, 'Mpg+': 23.8}
✅PASS : eg_clone
✅PASS : eg_csv
68 455 193.42587939698493 104.269838171196
{'Lbs-': 2970.4, 'Acc+': 15.6, 'Mpg+': 23.8}
✅PASS : eg_data
{'lo': 0.0, 'hi': 0.8746495688429434, 'mid': 0.5, 'div': 0.25}
✅PASS : eg_dist
200 198
l {'Lbs-': 2360.88, 'Acc+': 16.39, 'Mpg+': 28.35}
r {'Lbs-': 3586.13, 'Acc+': 14.74, 'Mpg+': 19.29}
✅PASS : eg_half
{'bins': 16, 'cliffs': 0.147, 'd': 0.35, 'file': '../etc/data/auto93.csv', 'Far': 0.95, 'go': 'all', 'help': False, 'Halves': 512, 'min': 0.5, 'Max': 512, 'p': 2, 'rest': 4, 'Reuse': True, 'seed': 937162211}
✅PASS : eg_is
1 0.5 0.3
2 0.3 0.3
✅PASS : eg_nums
✅PASS : eg_rand
{1: 1, 2: 2, 3: 3, 4: 4, 5: 5, 6: 6, 7: 7, 8: 8, 9: 9, 10: 10, 11: 11, 12: 12, 13: 13, 14: 14, 15: 15, 16: 16, 17: 17, 18: 18, 19: 55, 20: 20, 21: 21, 22: 22, 23: 23, 24: 24, 25: 25, 26: 26, 27: 27, 28: 28, 29: 29, 30: 30, 31: 31, 32: 32}
✅PASS : eg_some

all  {'Lbs-': 2970.42, 'Acc+': 15.57, 'Mpg+': 23.84}
     {'Lbs-': 846.84, 'Acc+': 2.76, 'Mpg+': 8.34}

best {'Lbs-': 2290.5, 'Acc+': 15.44, 'Mpg+': 27.14}
     {'Lbs-': 376.84, 'Acc+': 1.59, 'Mpg+': 4.69}

rest {'Lbs-': 3313.55, 'Acc+': 15.84, 'Mpg+': 21.61}
     {'Lbs-': 910.7, 'Acc+': 2.69, 'Mpg+': 9.1}

all ~= best? {'Lbs-': True, 'Acc+': True, 'Mpg+': True}
best ~= rest? {'Lbs-': True, 'Acc+': True, 'Mpg+': True}
✅PASS : eg_sway
a 1.38
✅PASS : eg_syms
398 {'Lbs-': 2970.4, 'Acc+': 15.6, 'Mpg+': 23.8}
| 200 
| | 101 
| | | 51 
| | | | 26 {'Lbs-': 2230.3, 'Acc+': 16.7, 'Mpg+': 26.5}
| | | | 25 {'Lbs-': 2221.6, 'Acc+': 16.8, 'Mpg+': 25.6}
| | | 50 
| | | | 26 {'Lbs-': 2297.9, 'Acc+': 16.1, 'Mpg+': 30.4}
| | | | 24 {'Lbs-': 2211.0, 'Acc+': 16.1, 'Mpg+': 34.2}
| | 99 
| | | 50 
| | | | 26 {'Lbs-': 2297.2, 'Acc+': 15.8, 'Mpg+': 28.1}
| | | | 24 {'Lbs-': 2621.3, 'Acc+': 17.8, 'Mpg+': 31.7}
| | | 49 
| | | | 25 {'Lbs-': 2630.5, 'Acc+': 16.4, 'Mpg+': 23.6}
| | | | 24 {'Lbs-': 2393.0, 'Acc+': 15.4, 'Mpg+': 27.1}
| 198 
| | 100 
| | | 51 
| | | | 26 {'Lbs-': 3026.9, 'Acc+': 16.2, 'Mpg+': 24.6}
| | | | 25 {'Lbs-': 2485.7, 'Acc+': 16.4, 'Mpg+': 30.4}
| | | 49 
| | | | 25 {'Lbs-': 3409.6, 'Acc+': 17.5, 'Mpg+': 20.0}
| | | | 24 {'Lbs-': 3263.8, 'Acc+': 16.7, 'Mpg+': 20.0}
| | 98 
| | | 50 
| | | | 26 {'Lbs-': 4176.3, 'Acc+': 13.6, 'Mpg+': 17.3}
| | | | 24 {'Lbs-': 4164.3, 'Acc+': 13.0, 'Mpg+': 15.0}
| | | 48 
| | | | 25 {'Lbs-': 4109.4, 'Acc+': 12.8, 'Mpg+': 12.4}
| | | | 23 {'Lbs-': 4103.5, 'Acc+': 11.4, 'Mpg+': 13.9}
✅PASS : eg_tree

Clndrs -inf 4
Clndrs 4 inf

Volume -inf 90
Volume 90 116
Volume 116 141
Volume 141 inf

Model -inf 71
Model 71 73
Model 73 74
Model 74 75
Model 75 77
Model 77 inf

origin 1 1
origin 2 2
origin 3 3

origin 2 2 0.85 {'best': 14, 'rest': 10}
Clndrs -inf 4 0.72 {'best': 14, 'rest': 22}
Volume -inf 90 0.42 {'best': 7, 'rest': 5}
Model 73 74 0.4 {'best': 6, 'rest': 2}
Model 74 75 0.34 {'best': 6, 'rest': 6}
Volume 90 116 0.19 {'best': 4, 'rest': 8}
Volume 116 141 0.15 {'best': 3, 'rest': 5}
Model 71 73 0.02 {'best': 1, 'rest': 11}
Model 75 77 0.02 {'best': 1, 'rest': 13}
Clndrs 4 inf 0.0 {'rest': 34}
Volume 141 inf 0.0 {'rest': 38}
Model -inf 71 0.0 {'rest': 4}
Model 77 inf 0.0 {'rest': 20}
origin 1 1 0.0 {'rest': 39}
origin 3 3 0.0 {'rest': 7}

{'origin': [2]}
{'origin': [2], 'Clndrs': [[-inf, 4]]}
{'origin': [2], 'Clndrs': [[-inf, 4]], 'Volume': [[-inf, 90]]}
{'origin': [2], 'Clndrs': [[-inf, 4]], 'Volume': [[-inf, 90]], 'Model': [[73, 74]]}
{'origin': [2], 'Clndrs': [[-inf, 4]], 'Volume': [[-inf, 90]], 'Model': [[73, 75]]}
{'origin': [2], 'Clndrs': [[-inf, 4]], 'Volume': [[-inf, 116]], 'Model': [[73, 75]]}
{'origin': [2], 'Clndrs': [[-inf, 4]], 'Volume': [[-inf, 141]], 'Model': [[73, 75]]}

-----------
explain= {'origin': [2]}
all                {'Lbs-': 2290.5, 'Acc+': 15.44, 'Mpg+': 27.14} {'Lbs-': 376.84, 'Acc+': 1.59, 'Mpg+': 4.69}
sway with  6 evals {'Lbs-': 2290.5, 'Acc+': 15.44, 'Mpg+': 27.14} {'Lbs-': 376.84, 'Acc+': 1.59, 'Mpg+': 4.69}
xpln with  6 evals {'Lbs-': 2423.3, 'Acc+': 16.79, 'Mpg+': 28.57} {'Lbs-': 490.04, 'Acc+': 3.05, 'Mpg+': 6.66}
sort with  398 evals {'Lbs-': 4633.14, 'Acc+': 12.96, 'Mpg+': 10.0} {'Lbs-': 356.67, 'Acc+': 2.05, 'Mpg+': 0.0}
✅PASS : eg_xpln
