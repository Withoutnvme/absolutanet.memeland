[![Telegram channel](https://img.shields.io/endpoint?url=https://runkit.io/damiankrawczyk/telegram-badge/branches/master?url=https://t.me/n4z4v0d)](https://t.me/n4z4v0d)
[![PyPI supported Python versions](https://img.shields.io/pypi/pyversions/better-automation.svg)](https://www.python.org/downloads/release/python-3116/)
[![works badge](https://cdn.jsdelivr.net/gh/nikku/works-on-my-machine@v0.2.0/badge.svg)](https://github.com/nikku/works-on-my-machine)  


![alt text](https://i.imgur.com/1yX3NAx.png)
Version 3.11.6 of Python
config.py
SITE_KEY - SITEKEY for solving Twitter captcha when unfreezing an account, do not change
SITE_URL - SITEURL for Twitter account unfreezing, do not change
FIRSTCAPTCHA_API_KEY - API KEY from https://1stcaptcha.com/ (make sure to top up the balance)
CHANGE_PROXY_URL - Link for changing IP when using mobile proxies with link change
REPEATS_ATTEMPTS - Number of attempts to repeat the script execution in case of errors
SOLVE_CAPTCHA_ATTEMPTS - Number of attempts to solve the captcha
UNAUTHORIZED_ATTEMPTS - Number of attempts to retry actions in case of Unauthorized errors
SLEEP_BETWEEN_TASKS - Sleep time between task execution (e.g., 1, 5, 10 // range, e.g., 1-5, 5-7, 2-6)
SLEEP_AFTER_PROXY_CHANGING - Sleep time after changing the Proxy
GM_PHRASES_LIST - List of phrases for commenting on GM posts

accounts.txt
Fill in the auth_token's of the accounts, each on a new line

private_keys.txt
Private keys from wallets to link to accounts (if desired, link your own wallets. You can leave the file empty - the software will register wallets and link them to accounts automatically)

proxies.txt
List of proxies (you can insert a single mobile proxy, the software will randomly select from the file). Format - type://user:pass@ip:port // type://ip:port

log files
empty_attempts.txt - a file with account tokens for which retry attempts have been exhausted (see config.py -> REPATS_COUNT)
registered.txt - file of successfully registered accounts
suspended_accounts.txt - file of account tokens blocked on Twitter
account_too_new.txt - File of account tokens that do not meet the parameters
unauthorized_accounts.txt - File of account tokens with Unauthorized error
forbidden_accounts.txt - File of account tokens with Forbidden error
http_exceptions.txt - File of account tokens with HTTP Exception error
unexpected_errors.txt - File of account tokens with unexpected errors

errors
Q: SSL: CERTIFICATE_VERIFY_FAILED
A: MAC: open /Applications/Python\ 3.11/Install\ Certificates.command

DONATE (any EVM) - 0xbE7F99B30051b52B489381e939665C0eA9f4f3A6
