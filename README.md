This script should be used for authorized penetration testing and/or educational purposes only.
Any misuse of this software will not be the responsibility of the author. Use it at your own networks and/or with the network owner's permission.

## Usage

````bash
git clone https://github.com/e1abrador/SpringCorePoC.sh
cd SpringCorePoC.sh
chmod 777 SpringCorePoC.sh
./SpringCorePoC file_with_urls
````

![alt text](https://github.com/e1abrador/SpringCorePoC.sh/blob/master/springCorePoC.png)

Note: bash script does not filter for http response body, in case that the web app shows 404 error page with status code 200, will show as vulnerable. Nuclei script does filter that and should't show false positives.                    
Note: Please, don't delete headers file, if you delete it, bash script won't work!

To use it at nuclei, run:

````bash
cat file_with_urls | nuclei -t SpringCorePoC.yaml
````
![alt text](https://github.com/e1abrador/SpringCorePoC.sh/blob/master/SpringCorePoC_nuclei.png)

<h1>Support</h1>

If you like this script and it saves you time, money or just brings you happy feelings, please show your support through sponsorship! Click the little sponsor button in the header and sponsor for as little as $1 per month :)

Or buy me a coffee to keep me powered :)

<a href="https://www.buymeacoffee.com/e1abrador" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-black.png" alt="Buy Me A Coffee" width=300px> </a>
