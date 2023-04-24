# lst-analysis-config
Configuration files for LST Analyses

To be used as a submodule in the [main analysis repository](https://github.com/nbiederbeck/lst-agn-analysis).

## Organization

```
lst-analysis-config/{source}/{analysis}/
```

Each directory in this repository holds configuration for a specific source.
The general data selection, which All-Sky MC to use, how to process their IRFs, and a matplotlibrc.

Each source directory additionally holds one or more directories for analyses of that source.
In each of those directories is the Gammapy analysis config and Gammapy model config.

One source can have multiple analyses, e.g. for differing energy or time regimes.

## Usage

Fork this repository, change the settings to your liking, add another source, add another analysis etc.
Afterwards, clone your fork into the analysis repository.
```
git clone https://github.com/<your-username>/lst-analysis-config.git configs/<your-username>
```
