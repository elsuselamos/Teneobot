# Teneo

For those who don't want to stay active 24/7

# Features
- [x] Multiple accounts
- [x] Proxy support (HTTP protocol only)

# How to Use

1. Make sure Python and Git are installed on your computer.

2. Clone this repository
   
   ```
   git clone https://github.com/elsuselamos/Teneobot
   ```

3. Navigate to the teneoxd folder
   
   ```
   cd Teneobot
   ```

4. Optional step: Create a virtual environment
   
   Windows
   ```
   python/py -m venv env
   ```
   Linux
   ```
   python3 -m venv env
   ```
   Then activate the virtual environment
   Windows
   ```
   env\scripts\activate
   ```
   Linux
   ```
   source env/bin/activate
   ```

5. Install required libraries
   ```
   pip install -r requirements.txt
   ```

6. Enter your account access tokens in the `data.txt` file
   
   [How to Get Account Access Token](#How-to-Get-Access-Token)

7. Edit `config.json` if you want to change the configuration. Here's a table explaining the `config.json` contents:
   
   | key           | description                           | value         |
   | ------------- | ------------------------------------- | ------------- |
   | ping_interval | wait time/delay between pings         | must be number|
   | max_retry     | maximum retry attempts when error occurs | must be number|

8. If you want to use proxies, add your proxies to the `proxies.txt` file. The proxy format should be as follows:
   
   With authentication:
   `protocol://user:password@host:port`
   example:
   `http://admin:admin@127.0.0.1:8000`
   Without authentication:
   `protocol://host:port`
   example:
   `http://127.0.0.1:8000`
9. After completing all steps, simply run `main.py`
    ```
    python main.py
    ```

# How to Get Access Token
1. Go to the Teneo dashboard page use code to register: trb8O
   
   [https://dashboard.teneo.pro/](https://dashboard.teneo.pro/)

2. Open DevTools by pressing F11/F12 or right-click -> Inspect Element

3. Go to the Console tab

4. Type `allow pasting` to enable pasting JavaScript code

5. Paste the following JavaScript code into the console
   ```
   copy(localStorage.getItem('accessToken'))
   ```

6. Then paste (Ctrl + V) as the JavaScript code above has copied the access token to your device's clipboard. If the access token doesn't appear or nothing appears when pasting, something went wrong with your actions.

7. Paste the access token into the `data.txt` file



# Thank you
