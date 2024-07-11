
# Setting up a Conda Environment on Mac

1. Install Miniconda using Homebrew:
   ```
   brew install --cask miniconda
   ```

2. Initialize conda for your shell:
   ```
   conda init "$(basename "${SHELL}")"
   ```

3. Add conda-forge to your channels:
   ```
   conda config --add channels conda-forge
   ```

4. Disable auto-activation of the base environment:
   ```
   conda config --set auto_activate_base false
   ```

5. Reload your shell to apply changes:
   ```
   exec zsh -l
   ```

6. Create a new conda environment with a specified name and install packages from a requirements file:
   ```
   conda create --name env_name --file requirements.txt
   ```
