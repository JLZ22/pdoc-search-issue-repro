# pdoc seearch issue repro

- reproducing an issue with pdoc search

## System Specs

```
~/Code/pdoc-search-issue-repro (main*) » pdoc --version       
pdoc: 14.6.0
Python: 3.12.4
Platform: macOS-14.6-arm64-arm-64bit
```

## Steps

1. create virtual environment
2. `pip install -r requirements.txt`
3. `pdoc src/*.py` 
    * this yields search results
4. `pdoc src/*.py --no-include-undocumented`
    * this does not yield search results