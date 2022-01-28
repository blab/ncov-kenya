# SARS-CoV-2 Nextstrain phylogeny for Kenya Research Group study
This phylogenetic analysis was designed to analyze samples collected by the Kenya Research Group in the context of other SARS-CoV-2 samples in Kenya.

The phylogeny created by this analysis can be viewed at [nextstrain.org/groups/blab/ncov/kenya](https://nextstrain.org/groups/blab/ncov/kenya).

This repository was inspired by [blab/ncov-africa](https://github.com/blab/ncov-africa) created by John Huddleston.

## Running the analysis
[Setup the Nextstrain software environment and download the ncov workflow](https://nextstrain.github.io/ncov/setup.html).
For example, to download the workflow you can run the following command.

```bash
git clone https://github.com/nextstrain/ncov.git
```

Download this repository into a separate directory.

```bash
git clone https://github.com/blab/ncov-kenya.git
```

Change directories to the `ncov` workflow.

``` bash
cd ncov/
```

Run the workflow using the nextstrain-cli. Specify number of `--cores` as needed.

``` bash
nextstrain build . --configfile ../ncov-kenya/builds.yaml --cores 4
```

To edit the workflow configuration:

```bash
open ../ncov-kenya/builds.yaml
```

To edit the Auspice configuration, setting the `build_url` and `maintainers`, as needed.

```bash
open ../ncov-kenya/auspice_config.json
```

