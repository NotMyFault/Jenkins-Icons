# Jenkins-Icons

## How to use
Cross CI icon repository created for the [Jenkins Sidebar Links](https://plugins.jenkins.io/sidebar-link) plugin.
You don't have file access to `/userContent/` on a CI but want to use custom icons? No problem!    
Simply set up a job with this repository to import the icons. You don't need any build tasks, just let the CI import this repository.    
After that, you can point the `Link Icon` field to a job, e.g. `job/<job name>/ws/icons/discord.jpg` and it will display the discord icon.    

## Troubleshooting
If your CI or job uses project-based security (Matrix based security), make sure to grant `Anonymous Users` or generally everyone Workspace access to this job, otherwise Jenkins cannot display the icons.

## Adding custom icons
You want to add your icons to this repository? Fork this repository and shoot me a pr! Simply create a folder matching your username and add the icons into it.