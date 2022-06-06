## toybox.rs

Welcome to [toybox.rs](http://toybox.rs)! This is the main organization and point of entry for using the Toybox platform for testing and experimentating with autonomous agents. 

- Main repository with tests/experimentation support provided by a customized openai/baselines: [toybox-rs/Toybox](https://github.com/toybox-rs/Toybox)
- Core repository with implementations of the games: [toybox-rs/toybox-rs](https://github.com/toybox-rs/toybox-rs). Releases available on PyPI: [![PyPI version](https://badge.fury.io/py/ctoybox.svg)](https://badge.fury.io/py/ctoybox)


## What is Toybox?

Toybox is a set of _highly intervenable_ environments for testing autonomous agents. While our efforts have focused on the efficient testing of deep RL agents, this work can be used in a variety of contexts that involve white-box testing of black-box agents. 

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

You can try playing our mocked Atari games locally:

```bash
pip install ctoybox
pip install pygame # optional dependency for human_play
python -m ctoybox.human_play amidar
```

The core repository is [`toybox-rs`](https://github.com/toybox-rs/toybox-rs). This contains the efficient Rust implementations of our current set of Atari mocks. The ffi exports Rust objects as Python objects; we also support exporting objects as JSON. The `ctoybox` package contains only low-level reading and writing to and from structured objects in the game. You can see the [Google Collab Notebook](https://colab.research.google.com/drive/1MMPseXpJ5esIXwTcHo0EBSG2iLaR0JPB?usp=sharing) for instructions on how to interact with the raw exports. 

Some games are quite complex. Therefore, we also provide an interface to both read and modify (i.e., intervene on) state via the [`Toybox`](https://github.com/toybox-rs/Toybox) repository. 

---
Website still under construction: contact the authors with questions, or [post an issue on this repo](https://github.com/toybox-rs/toybox-rs.github.io/issues).
