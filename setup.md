# Installing Miniconda

Download the Miniconda package and install it (use your preferred location).

## Permanently add Miniconda to PATH

Add this line to your shell config:

```
export PATH="/Users/Desktop/miniconda3/bin:$PATH"
```

For bash, edit `~/.bashrc` (macOS Terminal users: `~/.bash_profile`).  
For zsh, use `~/.zshrc`.

Reload your shell:

```
source ~/.bashrc # or source ~/.zshrc
```

Check Conda:

```
conda --version
```


## Set up environment

```
conda create -n env1 python=3.11
conda activate env1
conda install mamba -c conda-forge
```

You can also use mamba for all normal environment management tasks, such as:

Creating environments:
```
mamba create -n myenv python=3.11
```

Activating environments: (The activate command still uses conda, that's normal!)

```
conda activate myenv
```

Installing any package: (Use mamba install for fast package installs)

```
mamba install <package-name>
```


