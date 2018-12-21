# How to use
First you need to install git, Node.JS and NPM:

	sudo apt-get update
	sudo apt-get install nodejs npm git

After that you clone the repository and install all NPM dependencies:
	
	git clone https://github.com/yuriolive/request2block.git
	cd request2block/
	npm install

Then you have to make the request2block executable:

	sudo chmod +x request2block

Then you can run in terminal:

	./request2block -u https://www.example.com -t 5 -r 5000

This will run for the website https://wwww.example.com, throttle to 5 requests per second and run 5000 requests in total.

To see all the options you can run:
	
	./request2block -h

This will return:

	Usage: request2block [options]

	Options:
	  -v, --version       output the version number
	  -u, --url <url>     url to be tested
	  -t, --throttle [n]  how many request per second, default is 10
	  -r, --requests [n]  how many total requests, default is 10000
	  -h, --help          output usage information

