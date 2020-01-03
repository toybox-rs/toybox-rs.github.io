## toybox.rs

Welcome to [toybox.rs](http://toybox.rs)!

- Main repository with tests/experimentation support provided by a customized openai/baselines: [toybox-rs/Toybox](https://github.com/toybox-rs/Toybox)
- Core repository with implementations of the games: [toybox-rs/toybox-rs](https://github.com/toybox-rs/toybox-rs). Releases available on PyPI: [![PyPI version](https://badge.fury.io/py/ctoybox.svg)](https://badge.fury.io/py/ctoybox)


## What is Toybox?

A set of games designed for testing deep RL agents.

If you use this code, or otherwise are inspired by our white-box testing approach, please cite our [NeurIPS workshop paper](https://arxiv.org/abs/1812.02850):

```bibtex
@inproceedings{foley2018toybox,
  title={Toybox: Better Atari Environments for Testing Reinforcement Learning Agents},
  author={Foley, John and Tosch, Emma and Clary, Kaleigh and Jensen, David},
  booktitle={NeurIPS 2018 Workshop on Systems for ML},
  year={2018}
}
```

## How do I try it? [![PyPI version](https://badge.fury.io/py/ctoybox.svg)](https://badge.fury.io/py/ctoybox)

```bash
pip install ctoybox
pip install pygame # optional dependency for human_play
python -m ctoybox.human_play amidar
```

---
Website still under construction: contact the authors with questions, or [post an issue on this repo](https://github.com/toybox-rs/toybox-rs.github.io/issues).
