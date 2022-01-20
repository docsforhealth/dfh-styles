# Docs for Health Base Styles

Foundational SCSS styles shared between all relevant Docs for Health repositories. 

## Requirements

1. Usually embedded within other projects as a submodule mounted at `src/scss/base`
2. The containing project must define the `$path-base-styles` SCSS variable to point to the project-relative path the base styles are mounted at in order for the embedded `base-assets` urls to resolve properly 
3. Depends on `scut` so make sure to `yarn add --dev scut@latest` in the containing project

## Setting-up

In the repository you use to [embed these base styles as a submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules):

- Initial set-up: `git submodule add git@github.com:docsforhealth/dfh-styles.git <your desired path>`
- When cloning the repo subsequently, initialize the submodule with: `git submodule update --init --recursive` 

## Usage

In the repository you have embedded this repo as a submodule: 

- If you want to use all base styles, you can import the `_import.scss` file which imports all of the base styling files in the correct order
- To receive the latest updates to this shared styles repo, you need to `cd` into the submodule directory and `git pull`
- If you make any changes to this shared styles repo, you need to `cd` into the submodule directory and `git push` (make sure to `git pull` first)
