# SPCoast_KiCad_Libraries
SPCoast symbols, footprints, 3d models

To use on your system

install kilm - a command line KiCad Library Manager

```code
# Install pipx if you don't have it
python -m pip install --user pipx
python -m pipx ensurepath

# Install kilm
pipx install kilm
```

git clone this repo somewhere on your computer and use kilm to add it to your kicad installation:
```shell
% git clone https://github.com/plocher/SPCoast_KiCad_Libraries.git
% cd SPCoast_KiCad_Libraries
% kilm init
% cd 3dmodels/SPCoast.3dshapes
% kilm add-3d
% kilm setup
% kilm pin --symbols SPCoast --footprints SPCoast
```

To update your library when/if it gets changed on github
```code
% cd SPCoast_KiCad_Libraries   # ... wherever you git cloned it...
% git pull
% kilm setup
```


