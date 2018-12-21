# How to use
First you need to install Node.JS and all NPM dependencies:

	sudo apt-get install nodejs
	sudo apt-get install npm
	npm install

Then you have to make the request2block executable:

	sudo chmod +x request2block

Then you can run in terminal:

	./request2block -u https://www.example.com -t 5

This will run for the website https://wwww.example.com and throttle to 5 requests per second.

To see all the options you can run:
	
	./request2block -h

This will return:

	Usage: request2block [options]

	Options:
	  -v, --version       output the version number
	  -u, --url <url>     url to be tested
	  -t, --throttle [n]  how many request per second, default is 10
	  -h, --help          output usage information
