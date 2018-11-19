# scipion-em-plugins
This repo groups all Scipion plugins. The main goal is to facilitate the development workflow of the different plugin repos. Instead of having a single project for each one, here all of them are contained as submodules.

## To add submodule:
Run `git submodule add https://github.com/scipion-em/scipion-em-repo`

## To remove submodule:
1. Delete the relevant section from the _.gitmodules_ file.
2. Stage the _.gitmodules_ changes: `git add .gitmodules`.
3. Delete the relevant section from _.git/config_.
4. Run `git rm --cached path_to_submodule` (no trailing slash).
5. Run `rm -rf .git/modules/path_to_submodule` (no trailing slash).

## To update all submodules:
`git submodule update --recursive --remote`

## To clone this repo:
`git clone --recurse-submodules -j8 https://github.com/azazellochg/scipion-em-plugins.git`
