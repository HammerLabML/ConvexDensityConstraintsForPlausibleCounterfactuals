# Convex density constraints for computing plausible counterfactual explanations

This repository contains the implementation of the methods proposed in the paper [Convex density constraints for computing plausible counterfactual explanations](paper.pdf) by André Artelt and Barbara Hammer.

The proposed methods are implemented in [plausible_counterfactuals.py](plausible_counterfactuals.py). The experiments as described in the paper are implemented in [test.py](test.py).

The default solver is [SCS](https://github.com/cvxgrp/scs). If you want to use a different solver, you have to overwrite the `_solve` method in `plausible_counterfactuals.py`.

### Note on the implementation for decision trees

Note that the provided implementation of our proposed methods is *NOT efficiently implemented for decision trees!* There is a lot of room for improvements like pruning of leafs and high-density ellipsoids.

## Requirements

- Python3.6
- Packages as listed in `requirements.txt`

## License

MIT license - See [LICENSE](LICENSE)

## How to cite

You can cite the version on [arXiv](TODO).
