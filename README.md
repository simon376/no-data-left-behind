# No Data Left Behind - Exogenous Variables in Long-Term Forecasting of Nursing Staff Capacity

## Setup

All dependencies are included in the pyproject.toml and can be installed using poetry.

## How to run 

python train.py -cn config_name

runs an experiment based on a config in the /configs folder. The `-config-name,-cn` parameter sets the "base" config to use in `hydra.main()`.
Apart from that you can use hydra's [Override Syntax](https://hydra.cc/docs/advanced/override_grammar/basic/) to set pre-configured experiment configs or change specific values.

python train.py -cn lightgbm-uni trains a lightgbm model using univariate data only.

...
