Discord-Account-Generator
Proof of concept of how the creation of Discord accounts can be automated without the need to type/click buttons on browser.

About
A script that automates creating discord accounts. It shows how accounts can be created automatically without the user typing unless there is a captcha (h-Captcha just needs to be clicked) . It automatically verifies your Discord account via email for you and automatically saves login info in login.txt in email:password:token format. This is used for educational purposes only.
__________________________________________________________________________

Features
Auto scrape email
Random username from list
Random password
Random date
Auto-email-verify
Automatically get Discord token and other login info
Proxy support
Multi-threading
Preview
Picture

__________________________________________________________________________

Usage
You can customize usernames by editing the usernames in discord_usernames.txt.
Run the file and use normal mode if you are a inexperienced with proxies and theading.
Get Python
If you dont have python installed, download python 3.7.6 and make sure you click on the 'ADD TO PATH' option during the installation.

Run via Python
install the required modules
pip install selenium
pip install undetected-chromedriver
pip install colorama
pip install bs4
pip install lxml
pip install requests
To run the script..
python discordgenerator.py
Proxy support
__________________________________________________________________________

If you want to use proxies, simply paste the proxies in config/proxies.txt. If you want to stop using proxies, just remove all the proxies from the .txt file. The script automatically checks for proxies on startup. HTTP proxies are only supported as of now. If the proxies are not alive, the script will throw a WebDriver error.
Threading mode
Uses multiple chrome windows
Only run this when you have proxies or else one of you Chrome windows will get rate limited.
Do put more than 6 threads unless you think your PC can handle it. I recommend using 2-3 threads.
No Threading
This only uses one chrome window.
