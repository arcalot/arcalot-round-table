# Title

Rename Carpenters repository to `arcalot/arcaflow-container-toolkit` and move reusable workflow yaml file to carpenter.

## Voting Period

The voting period for this proposal will be open for 7 days from its submission as an active PR.

## Benefits

Currently, carpenters repository is named `arcaflow-plugin-image-builder` with a pet name of carpenter. It currently shares the same naming convention as our offical plugins, however it itself is not a plugin. To clear this up I propose we rename the entire repository to simply arcalot/arcaflow-container-toolkit or any agreed upon name. 

This change will separate the tool from the plugins and pave way for a much clearer readme.md file I am currently working on [here](https://github.com/jdowni000/arcaflow-plugin-image-builder/blob/docs/README_UPDATE.md#using-carpenter-in-reusable-workflow). This will simplify the entrypoint for new users to the tool and cause less confusion in the documentation with naming convention as well as usage.

Also I believe it would be a good time to move the reusable workflow file from [arcaflow-reusable-workflows](https://github.com/arcalot/arcaflow-reusable-workflows/blob/main/.github/workflows/carpenter.yaml), into the carpenter project itself. This will centralize the project and keep everything carpenter, with carpenter.

## Drawbacks

This is a breaking change that impacts all repositories and users of carpenter. The naming convention change will require all projects to update the paths to use carpenter. Secondly, a new version will need to be released when this is done, once all PR's are merged it would be a good time for an official v1.0.0 release. Finally, any project using carpenter in a reusable workflow will need to update the path for the yaml file as well if the file was to move into carpenter. This can all be done pretty quickly with minimal effort but is very important to communicate to our end users and team. 