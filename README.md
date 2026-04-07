<h3 align="center">
	<img src="imgs/logo.png" width="96" />
	<br>
	Nevergrove VSCode
</h3>
<h5 align="center">
	The four variants of the Nevergrove color palette brought straight into your VSCode.
</h5>
<h6 align="center">
	This theme is part of <a href="https://github.com/IcaroJam/nevergrove">the official set of Nevergrove themes!</a>
</h6>
<br>

Nevergrove is an [everforest](https://github.com/sainnhe/everforest)-inspired color palette designed to be soft, yet vibrant and provide the right amount of contrast without causing strain on your eyes.

## The Looks
Nevergrove comes in four variants, each centered around a main accent and a secondary inverse accent for contrast on elements that require your attention.

### Maple - Red
![](imgs/maple.png)

### Aspen - Yellow
![](imgs/aspen.png)

### Eucalyptus - Teal
![](imgs/eucalyptus.png)

### Jacaranda - Purple
![](imgs/jacaranda.png)


## Version Disclaimer

> [!Warning]
> The theme is still in alpha. Expect changes, broken stuff, and bright neon colors in places I've yet to test. Sorry for the inconvenience!

It is my first time making a theme for vscode, on top of that I've chosen a semi-manual building method that doesn't allow theme settings as far as I know since I'm directly generating the theme's JSON file from a template I then run sed on a bunch of times to substitute "variables" with their respective colors.

_Why do that?_ I hear you ask. I'm developing this theme together with themes for a bunch other programs, and I found it works great for the most part without having to use any external tools. When I first started making the vscode theme I didn't know any better either and I'd like to revamp it all in the future, mainly to allow for theme settings, but I just haven't got the time at the moment.

### Testing, packaging and installing locally
Development versions can be tested by cloning this repo, opening it in vscode and pressing `f5`. An easier but still way too convoluted way is cloning the [parent palette repo](https://github.com/IcaroJam/nevergrove) directly and modifying `vscode/themeSrc.jsonc`, then running the `updateVars.sh` script.

To package the theme for installation you'll need to have [vsce](https://github.com/microsoft/vscode-vsce) installed via `npm install -g @vscode/vsce`. Then run `vsce pack` in the root of this repo. This will create the `.vsix` file with the color themes.

To locally install the resulting package, hit `ctrl+shift+p` inside vscode and enter `Install from VSIX`, then select the packaged theme and you are good to go!