# Jenkins-Icons
Cross CI icon repository created for the [Jenkins Sidebar Links](https://plugins.jenkins.io/sidebar-link) plugin.

You don't have file access to `/userContent/` on a CI but want to use custom icons? No problem!  
Simply follow the instrtuctions below and you're good to go.

## How to use

### On CodeMC.io
If you have a project on the [CodeMC CI server](https://ci.codemc.io), then you can skip setting up a own job and use the one from IntellectualSites.  
The base-path is `job/IntellectualSites/job/Jenkins-Buttons/ws/icons/` followed by either the icon-name (e.g. `discord.jpg`) or the path to the icon (e.g. `plugins/IntellectualSites/Fawe.jpg`).

### Own Jenkins
If you have your own Jenkins server setup, simply create a new job with this repository to import the icons. This job doesn't require any build tasks, just let the CI import this repository.  
After that can you use the path to your newly created job in the `Link Icon` field. For example `job/<job name>/ws/icons/discord.jpg` will display the [Discord Icon](/icons/discord.jpg)

You can use icons in jobs, view tabs, folders or on the main page. Generally everywhere where you have the management bar on the left side.

One job per CI is enough. You don't need to setup multiple jobs for this project, once Jenkins imported the icons, everyone can use them.

## Troubleshooting
If your CI or job uses project-based security (Matrix based security), make sure to grant `Anonymous Users` or generally everyone Workspace access to this job, otherwise Jenkins cannot display the icons.  
Some CIs have issues with png files. For the best experience, make sure you are using jpg files.

## Adding custom icons
You want to add your icons to this repository? Fork this repository and shoot me a pr! Simply create a folder matching your username and add the icons into it.

**Important!**  
If you add icons with the goal to later use them in a project on CodeMC, make sure, that the icons are saved as jpg-images and below a certain file-size (currently unknown) as the Jenkins Sidebar Links-plugin seems to have minor issues with large png-files and won't display those.
