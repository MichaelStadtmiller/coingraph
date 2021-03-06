# Coingraph

[![Version](https://img.shields.io/badge/version-0.1.0-brightgreen.svg)](https://github.com/derogab/coingraph)
[![Release](https://img.shields.io/badge/release-beta-lightgrey.svg)](https://github.com/derogab/coingraph)
[![GitHub stars](https://img.shields.io/github/stars/derogab/coingraph.svg)](https://github.com/derogab/coingraph/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/derogab/coingraph.svg)](https://github.com/derogab/coingraph/network)
[![GitHub issues](https://img.shields.io/github/issues/derogab/coingraph.svg)](https://github.com/derogab/coingraph/issues)
[![Donate](https://img.shields.io/badge/donate-paypal-blue.svg)](https://paypal.me/derogab)

Coingraph is a **real-time graph for cryptocurrencies**.
Powered by Python, MySQL and Cryptonator.

![Coingraph Screenshot](screenshot.png)

**Dependencies**
```shell
# Install dependencies
sudo apt-get install python python3 libmysqlclient-dev

# Install python dependencies
pip install json requests sys time tornado MySQL-python
```

**Download**

```shell
git clone https://github.com/derogab/coingraph
cd coingraph
python webserver.py
```

**Configuration**

Edit `webserver.py` and `getdata.py` to customize your mysql database connection.

**Cronjob**

Insert a cronjob. You can edit your cronjob list from the terminal command `crontab -e`. 
```
*/1 * * * * /usr/bin/python ~/coingraph/getdata.py
```

**Usage**

Open `http://localhost:8080` in your browser to view real-time graphs.

**Donate**

If this project helps you reduce your development time please considering [giving me a cup of coffee](https://www.paypal.me/derogab) :) 
