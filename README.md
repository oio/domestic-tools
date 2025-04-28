# Domestic AI Tools
Welcome to the Domestic AI Tools' repo. Here are stored all the snippets accessible by the [Domestic AI Universe](https://github.com/oio/domestic-ai). 
The tools are self-sustaining apps running locally on your computer. They expose an API on a port so that the [Domestic AI API](https://github.com/oio/domestic-API). See there for more infos about the project.
## Contributing
Domestic AI Tools is a container of submodules. You can add yours or update existing ones. 

### Add a new tool
A tool is an independent applet that runs on a specific port in your computer. Please check the ports that are already taken in order to avoid conflicts. You can find the list of busy ports in the [Domestic AI repo](https://github.com/oio/domestic-ai). Here are the steps to follow to create a new tool.
1. Create a new repository 
1. Push your code to it 
1. Document the API
1. Move to the Domestic AI Tools repo via ```cd [PATH_TO_YOUR_oio-domestic-ai-tools]```
1. ```git submodule add [GITHUB_LINK_OF_THE_REPO_YOU_JUST_CREATED]```
1. ```git add .```
1. ```git commit -m 'added new tool with name [NAME_OF_THE_SUBMODULE]'```
1. ```git push```

### Update an existing tool
If you just need to update an existing tool, you can just  edit it from its folder inside this repo, and then update this repo with the pushed changes. Here's how to do it.

1. Make your edits within the submodule's folder.
1. Move to the Domestic Tools repo via `cd [PATH_TO_YOUR_oio-domestic-ai-tools]`
1. ```
	git add .
	git commit -m 'added new submodule with name [NAME_OF_THE_SUBMODULE]'
	git push -u origin HEAD:main
	```
1. Lastly, go to your clone of the Domestic AI universe and update remote so that your tool is accessible for all. Follow the instructions to `Update existing submodules or pool new tools` in the [Domestic AI repo](https://github.com/oio/domestic-ai).