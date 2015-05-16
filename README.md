# Node.js

## Updating Node via npm

	sudo npm cache clean -f
	sudo npm install -g n
	sudo n stable

# npm

## Fixing npm permissions

Find the path to npm's directory: 

	npm config get prefix
	
For many systems, this will be `/usr/local`. Change the owner of npm's directory's to the effective name of the current user: 

	sudo chown -R `whoami` <directory>

[(Source)](https://docs.npmjs.com/getting-started/fixing-npm-permissions)
