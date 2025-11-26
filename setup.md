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
