## ProxyCheckTool
ProxyCheckTool is a Python script designed to test the validity of proxy servers. It checks proxies for connectivity, categorizes them based on their type, and saves valid ones into specific files.


![لقطة الشاشة 2024-07-23 042442](https://github.com/user-attachments/assets/a623125f-239f-4040-95bc-413405431258)



Getting Started
To get started with ProxyCheckTool, follow these steps:

Clone the Repository:

```
git clone https://github.com/H-crowe/ProxyCheckTool.git
cd ProxyCheckTool
```

Create a virtual environment (optional but recommended) and install dependencies:

```
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
pip install -r requirements.txt
```
# requirements

```
requests
fake_useragent
colorama
pyfiglet
```



put the ip list in proxy.txt in the root directory. Proxies can be with or without protocol prefixes (e.g., http://192.168.1.1:8080 or 192.168.1.1:8080).

Run the script: python app.py

The script will test each proxy, and save valid proxies into the following files:

http-valid.txt for HTTP proxies
socks4-valid.txt for SOCKS4 proxies
socks5-valid.txt for SOCKS5 proxies

## Code Explanation: 

1- Welcome Message: The script starts by printing a stylized welcome message and ASCII art logo.

2- Proxy Reading: Reads proxies from proxy.txt, normalizes them by removing protocol prefixes, and prepares them for testing.

3- Proxy Testing: Tests each proxy for connectivity and saves valid proxies to corresponding files.

4- Multithreading: Utilizes ThreadPoolExecutor to test proxies concurrently, enhancing performance.


## Contributing
Contributions are welcome! If you'd like to contribute to the project, please follow these steps:

Fork the repository and create a new branch.
Make your changes and test them locally.
Submit a pull request detailing your changes and improvements.

## Contact
If you have questions or need assistance, feel free to contact Telegram @cr0wel
