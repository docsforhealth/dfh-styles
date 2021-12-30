# Docs for Health Base Styles

Foundational SCSS styles shared between all relevant Docs for Health repositories. 

## Requirements

1. Usually embedded within other projects as a submodule mounted at `src/scss/base`
1. The containing project must define the `$path-base-styles` SCSS variable to point to the project-relative path the base styles are mounted at in order for the embedded `base-assets` urls to resolve properly 
