# Cheval (wsp-cheval)

Cheval is a Python package for high-performance evaluation of discrete-choice (logit) models. It's largely built upon the Pandas, NumPy, and NumExpr packages; along with some custom Numba code for performance-critical bottlenecks.

The name is an acronym for "CHoice EVALuator" but has a double-meaning as _cheval_ is the French word for "horse" - and this package has a lot of horsepower! It has been designed for use in travel demand modelling, specifically microsimulated discrete choice models that need to process hundreds of thousands of records through a logit model. It also supports "stochastic" models, where the probabilities are the key outputs.

## Key features

Cheval contains two main components:

- `cheval.ChoiceModel` which is the main entry point for discrete choice modelling
- `cheval.LinkedDataFrame` which helps to simplify complex utility calculations.

These components can be used together or separately.

Cheval is compatible with Python 3.7+