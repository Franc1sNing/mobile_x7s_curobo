# MemoryMatters Benchmark

## 📖 Usage

**1. IsaacSim Installation**

Benchmark is built upon **IsaacSim 5.0.0**, please refer to [NVIDIA Official Document](https://docs.isaacsim.omniverse.nvidia.com/latest/installation/download.html) for download. 

```We recommend placing the Isaac Sim source folder at `~/isaacsim_5.0.0` to match the Python interpreter path specified in the `.vscode/settings.json` file we provide. If you prefer to use a custom location, please make sure that the Python interpreter path in `.vscode/settings.json` is updated accordingly.```

We will use **~/isaacsim_5.0.0/python.sh** to run the isaacsim's python file. To facilitate the running, we can define a new alias in '.bashrc' file.

```bash
echo 'alias isaacsim="~/isaacsim_5.0.0/python.sh"' >> ~/.bashrc
source ~/.bashrc
```



Install the curobo.

```bash
# curobo
cd curobo
isaacsim -m pip install -e . --no-build-isolation # may take a while

# (optional) validate the installation
isaacsim curobo/examples/isaac_sim/motion_gen_reacher.py
```


