# lst-analysis-config
Configuration files for LST Analyses

To be used as a submodule in the [main analysis repository](https://github.com/nbiederbeck/lst-agn-analysis).

## Organization

```
lst-analysis-config/{analysis}/
```

This directory holds one or more directories for analyses of that source.
In each of those directories is the Gammapy analysis config and Gammapy model config.

The analysis can have multiple analyses, e.g. for differing energy or time regimes.

## Usage

Fork this repository, change the settings to your liking, add another source, add another analysis etc.
*Important:* Currently the `datastore` path in the `analysis.yaml` config needs to
be set to `build/{name of this directory}/dl3`.
Afterwards, clone your fork into the analysis repository.
```
git clone https://github.com/<your-username>/lst-analysis-config.git configs
```
Make sure that `configs` is an emtpy directory.
