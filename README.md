# <img src="logo.png" width="32" /> Nevergrove VSCode
###### The four variants of the Nevergrove color palette brought straight into your VSCode.
Nevergrove is an everforest-inspired color palette designed to be soft, yet vibrant and provide the right amount of contrast without causing strain on your eyes.

### Testing, packaging and installing locally
Development versions can be tested by cloning this repo, opening it in vscode and pressing `f5`. An easier but still way too convoluted way is cloning the [parent palette repo](https://github.com/IcaroJam/nevergrove) directly and modifying `vscode/themeSrc.jsonc`, then running the `updateVars.sh` script.

To package the theme for installation you'll need to have [vsce](https://github.com/microsoft/vscode-vsce) installed via `npm install -g @vscode/vsce`. Then run `vsce pack` in the root of this repo. This will create the `.vsix` file with the color themes.

To locally install the resulting package, hit `ctrl+shift+p` inside vscode and enter `Install from VSIX`, then select the packaged theme and you are good to go!