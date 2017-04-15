# CodeIgniter on Bluemix
A demo codeigniter framework boilerplate in IBM Bluemix (See the results: https://codeigniter-bluemix.mybluemix.net)

## Get Started
- a. Change Manifest.yml 
	```
		applications:
		- path: .
		  memory: 128M
		  instances: 1
		  domain: mybluemix.net
		  name: YOUR_NAME_APP
		  host: YOUR_HOST_NAME_APP
		  disk_quota: 1024M
		  services:
		  - YOUR_SERVICES_APP
	```
- b. Change options.json (in .bpconfig folder) for adding some PHP Extensions.
	```
	{
		"PHP_EXTENSIONS": ["mysql","mysqli","curl","gd","openssl"]
	}
	```
- c. Change config.php (applicaton/config/config.php)
	```
	// $config['base_url'] = 'https://codeigniter-bluemix.mybluemix.net';
	$config['base_url'] = 'YOUR_BASE_URL';
	```
