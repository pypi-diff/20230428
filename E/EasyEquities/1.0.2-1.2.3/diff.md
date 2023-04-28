# Comparing `tmp/EasyEquities-1.0.2.tar.gz` & `tmp/EasyEquities-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyEquities-1.0.2.tar", last modified: Mon Jul 26 09:41:17 2021, max compression
+gzip compressed data, was "EasyEquities-1.2.3.tar", last modified: Fri Apr 28 11:31:02 2023, max compression
```

## Comparing `EasyEquities-1.0.2.tar` & `EasyEquities-1.2.3.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxrwx   0        0        0        0 2021-07-26 09:41:17.497871 EasyEquities-1.0.2/
-drwxrwxrwx   0        0        0        0 2021-07-26 09:41:17.497871 EasyEquities-1.0.2/EasyEquities/
--rw-rw-rw-   0        0        0       15 2021-07-25 15:30:16.473000 EasyEquities-1.0.2/EasyEquities/__init__.py
--rw-rw-rw-   0        0        0     8119 2021-07-26 09:26:45.391864 EasyEquities-1.0.2/EasyEquities/broker.py
--rw-rw-rw-   0        0        0      699 2021-07-26 09:41:17.498869 EasyEquities-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       40 2021-07-25 15:15:29.960742 EasyEquities-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1707 2021-07-26 09:41:13.797456 EasyEquities-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 11:31:02.498335 EasyEquities-1.2.3/
+drwxrwxrwx   0        0        0        0 2023-04-28 11:31:02.483374 EasyEquities-1.2.3/EasyEquities/
+-rw-rw-rw-   0        0        0       15 2023-04-28 09:44:31.000000 EasyEquities-1.2.3/EasyEquities/__init__.py
+-rw-rw-rw-   0        0        0    12249 2023-04-28 09:53:09.000000 EasyEquities-1.2.3/EasyEquities/broker.py
+drwxrwxrwx   0        0        0        0 2023-04-28 11:31:02.497336 EasyEquities-1.2.3/EasyEquities.egg-info/
+-rw-rw-rw-   0        0        0     2972 2023-04-28 11:31:02.000000 EasyEquities-1.2.3/EasyEquities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-28 11:31:02.000000 EasyEquities-1.2.3/EasyEquities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 11:31:02.000000 EasyEquities-1.2.3/EasyEquities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-28 11:31:02.000000 EasyEquities-1.2.3/EasyEquities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-28 11:31:02.000000 EasyEquities-1.2.3/EasyEquities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2023-04-28 09:48:11.000000 EasyEquities-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2972 2023-04-28 11:31:02.498335 EasyEquities-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2222 2023-04-28 11:21:25.000000 EasyEquities-1.2.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-28 11:31:02.500329 EasyEquities-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1998 2023-04-28 11:30:24.000000 EasyEquities-1.2.3/setup.py
```

### Comparing `EasyEquities-1.0.2/EasyEquities/broker.py` & `EasyEquities-1.2.3/EasyEquities/broker.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,178 +1,269 @@
 import base64
 import sys
 import traceback
 import configparser
 import time
 import re
-from requests.api import options
+
+import pandas as pd
 
 from selenium import webdriver
+from selenium.webdriver import FirefoxOptions
 from selenium.webdriver.common import keys
 from selenium.webdriver.common.by import By
+from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.firefox.options import Options
-from urllib3.packages.six import b
+from selenium.webdriver.firefox.service import Service
+
+
 from webdriver_manager.firefox import GeckoDriverManager
+
+from shutil import which
+
+from urllib3.packages.six import b
 from bs4 import BeautifulSoup
 
 class EasyEquities:
-    timeout = 3
+    timeout = 2.5
     driver = None
     account = None
     options = None
 
     def __init__(self) -> None:
         pass
 
     def __init__(self, username, password, account = 'DEMO') -> None:
+        self.options = FirefoxOptions()
+        
         self.Username = username
         self.Password = password
         if account == 'DEMO':
-            self.account = 'slick-slide04'
+            self.account = 'Demo ZAR'
         if account == 'ZAR':
-            self.account = 'slick-slide00'
-        self.options = Options()
-
+            self.account = 'EasyEquities ZAR'
 
     def open(self):
-        self.options.headless = True
-        self.driver = webdriver.Firefox(
-            options = self.options,
-            executable_path=GeckoDriverManager().install())
+        self.options.add_argument('--headless')
+        self.driver = webdriver.Firefox(options=self.options, service=Service(GeckoDriverManager().install()))
         self.driver_wait = WebDriverWait(self.driver, 90)
         self.login(self.Username, self.Password)
 
     def close(self):
         time.sleep(self.timeout)
+        self.logout()
         self.driver.close()
         
     def login(self, username, password):
-        self.driver.get('https://platform.easyequities.io/Account/SignIn')
-        self.driver_wait.until(EC.presence_of_element_located((By.ID, "login-mobile")))
-        self.driver.find_element_by_id('user-identifier-input').send_keys(username)
-        self.driver.find_element_by_id('Password').send_keys(password)
-        self.driver.find_element_by_id('login-mobile').click()
-
-    def balance(self):  
-        self.open()      
-        self.driver_wait.until(EC.presence_of_element_located(
-            (By.ID, "important-documents")))
+        self.driver.get('https://identity.openeasy.io/Account/Login')
+        self.driver_wait.until(EC.presence_of_element_located((By.ID, "SignIn")))
+        self.driver.find_element(By.ID, 'user-identifier-input').send_keys(username)
+        self.driver.find_element(By.ID,  'Password').send_keys(password)
+        self.driver.find_element(By.ID, 'SignIn').click()
+
+        time.sleep(self.timeout)
+        if self.driver.current_url == 'https://identity.openeasy.io/Grants':
+            self.driver.get('https://platform.easyequities.io/')
+
+    def logout(self):
+        self.driver.get('https://identity.openeasy.io/Account/Logout')
+        self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "btn-primary")))
+        self.driver.find_elements(By.CLASS_NAME, "btn-primary")[1].click()
+
+    def balance(self) -> dict:  
+        self.open()  
+        Balance = {}
+
         self.driver.get('https://platform.easyequities.io/AccountOverview')
         time.sleep(self.timeout)
-        self.driver.find_elements_by_xpath(
-            "//div[ @aria-describedby='{0}']".format(self.account))[0].click()
-        self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "funds-to-invest")))
-        balance = self.driver.find_elements_by_xpath("//div[ @aria-describedby='{0}']".format(self.account))[0]
-        balance = balance.text.split('\n')[-1][1:].replace(' ', '')
+        self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "slick-track")))
+        self.driver.find_elements(By.XPATH, "//*[text()='{0}']".format(self.account))[0].click()
         
+        self.driver_wait.until(EC.presence_of_element_located((By.ID, "account-distribution")))
+        time.sleep(self.timeout)
+        balance = self.driver.find_element(By.ID, "asset-class-display")
+        balance = pd.read_html(balance.get_attribute('innerHTML'))
+
+        for item in balance:
+            for i, row in item.iterrows():
+                Balance[row[0]] = str(row[3])[1:].replace(' ', '')
+
+        self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "asset-summary-heading")))
+        Summary = self.driver.find_elements(By.CLASS_NAME,  'asset-summary-heading')
+        Balance['Value'] = Summary[0].text.replace('R', '').replace(' ', '')
+        Balance['Movement'] = Summary[1].text.replace('R', '').replace(' ', '')
+        Balance['Status'] = Summary[2].text[:-1].replace(' ', '')
+
         self.close()
 
-        return balance
+        return Balance
+
+    def holdings(self, tickers = True) -> list:
+        self.open() 
 
-    def holdings(self, tickers = True):
-        self.open()        
         Holdings = []
 
-        self.driver_wait.until(EC.presence_of_element_located((By.ID, "important-documents")))
         self.driver.get('https://platform.easyequities.io/AccountOverview')  
-        self.driver.find_element_by_xpath("//div[@aria-describedby='{0}']".format(self.account)).click()
+        time.sleep(self.timeout)
+        self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "slick-track")))
+        self.driver.find_elements(By.XPATH, "//*[text()='{0}']".format(self.account))[0].click()
+        time.sleep(self.timeout)
         self.driver_wait.until(EC.presence_of_element_located((By.ID, "loadHoldings")))
-        self.driver.find_element_by_id('loadHoldings').click()
+        self.driver.find_element(By.ID, "loadHoldings").click()
+
+        try:
+            self.driver_wait.until(EC.presence_of_element_located((By.ID, "no-holdings-message")))
+            element = self.driver.find_element(By.ID, "no-holdings-message")
+            if element is not None:
+                self.close()
+                return Holdings
+        except:
+            pass
+
+        time.sleep(self.timeout)
         self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "holding-table-body")))
-        holdings_data = self.driver.find_element_by_class_name('holding-table-body')
-        ticker_info = holdings_data.get_attribute('innerHTML')
-        
-        soup = BeautifulSoup(ticker_info, 'lxml')
-        ticker_table = soup.findAll('div', attrs={"class": "table-display"})
-        if(tickers):
-            for link in soup.findAll('a', href=True, text=True, attrs={"class": "btn"}):
-                ticker = link['href'].split('.')[-1]
-                if ticker not in Holdings:
-                    Holdings.append(ticker)
-        else:
-            for ticker in ticker_table:  
-                ticker = str("".join([ll.strip() for ll in ticker.text.splitlines() if ll.strip()]))            
-                regex =  r'([R]\d+\.?\d*)'
-                ticker = re.split(regex, ticker)
-                if ticker is not None:
-                    try:
-                        Holdings.append((ticker[0], ticker[1]))
-                    except:
-                        continue
+        holdings_table = self.driver.find_element(By.CLASS_NAME, 'holding-table-body')
+        tickers_data = holdings_table.find_elements(By.CLASS_NAME, 'content-box')
 
+        for ticker in tickers_data:
+            image = ticker.find_element(By.TAG_NAME, 'img').get_attribute('src')
+            holding = str(image).split('.')[-2].upper()
+            purchase = str(ticker.find_element(By.CLASS_NAME, 'purchase-value-cell').text)[1:].replace(' ', '')
+            current = str(ticker.find_element(By.CLASS_NAME, 'current-value-cell').text)[1:].replace(' ', '')
+            movement = str(ticker.find_element(By.CLASS_NAME, 'pnl-cell').text)
+
+            Holdings.append({'Holding': holding,
+                'Purchase': purchase,
+                'Current': current,
+                'Image': image,
+                'Movement': movement})
+            
         self.close()
 
         return Holdings
 
-    def buy(self, ticker, shares = 1, amount = None):
-        self.open()
+    def buy(self, ticker, shares = 1, amount = None, instruction = 'OPEN', limit = True, price = None):
+        try:
+            self.open()
+            self.driver.get('https://platform.easyequities.io/ValueAllocation/Buy?contractCode=EQU.ZA.{0}'.format(ticker.upper()))
+            self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "slick-track")))
+            self.driver.find_elements(By.XPATH, "//*[text()='{0}']".format(self.account))[0].click()   
+
+            self.driver_wait.until(EC.invisibility_of_element_located((By.CLASS_NAME, "value-allocations__snapshot-price-request-loader")))
+            self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "flex-container")))
+            if amount == None:
+                self.driver.find_element(By.ID, 'js-number-of-shares').send_keys(keys.Keys.CONTROL, 'a')
+                self.driver.find_element(By.ID, 'js-number-of-shares').send_keys(keys.Keys.BACKSPACE)
+                self.driver.find_element(By.ID, 'js-number-of-shares').send_keys(shares)
+                self.driver.find_element(By.ID, 'js-number-of-shares').send_keys(keys.Keys.ENTER)
+                
+            else:
+                self.driver.find_element(By.ID, 'js-value-amount').send_keys(keys.Keys.CONTROL, 'a')
+                self.driver.find_element(By.ID, 'js-value-amount').send_keys(keys.Keys.BACKSPACE)
+                self.driver.find_element(By.ID, 'js-value-amount').send_keys(amount)        
+                self.driver.find_element(By.ID, 'js-value-amount').send_keys(keys.Keys.ENTER)
+            
+            self.driver_wait.until(EC.invisibility_of_element_located((By.CLASS_NAME, "value-allocations__snapshot-price-request-loader")))
+            self.driver_wait.until(EC.presence_of_element_located((By.ID, "netAmountDueDisplay")))
+
+            if instruction != 'OPEN':
+                self.driver.find_element(By.IDE, 'advanced-btn').click()
+                if price != None:
+                    self.driver.find_element(By.ID, 'OrderPrice').send_keys(keys.Keys.CONTROL, 'a')
+                    self.driver.find_element(By.ID, 'OrderPrice').send_keys(keys.Keys.BACKSPACE)
+                    self.driver.find_element(By.ID, 'OrderPrice').send_keys(price)
+                    self.driver.find_element(By.ID, 'OrderPrice').send_keys(keys.Keys.ENTER)
+
+            if limit == True:
+                try:    
+                    self.driver.find_elements(By.CLASS_NAME, 'btnTradeOrderType js-order-type-btn')[1].click()
+                except:
+                    pass
 
-        self.driver_wait.until(EC.presence_of_element_located((By.ID, "important-documents")))
-        self.driver.get('https://platform.easyequities.io/Equity')  
-        time.sleep(self.timeout)
-        self.driver.find_elements_by_xpath("//div[ @aria-describedby='{0}']".format(self.account))[0].click()
-        time.sleep(self.timeout-2)
-        self.driver.find_element_by_id('InstrumentSearchString').send_keys(ticker)
-        time.sleep(self.timeout-2)
-        self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "hoverBorder")))
-        self.driver.get('https://platform.easyequities.io/ValueAllocation/Buy?contractCode=EQU.ZA.{0}'.format(ticker.upper()))
-        time.sleep(self.timeout-2)
-
-        self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "tab-pane")))
-        if amount == None:
-            self.driver.find_element_by_id('js-number-of-shares').send_keys(keys.Keys.CONTROL, 'a')
-            self.driver.find_element_by_id('js-number-of-shares').send_keys(keys.Keys.BACKSPACE)
-            self.driver.find_element_by_id('js-number-of-shares').send_keys(shares)
-            time.sleep(self.timeout)
-            self.driver.find_element_by_class_name('flex-container').click()
-        else:
-            self.driver.find_element_by_id('js-value-amount').send_keys(keys.Keys.CONTROL, 'a')
-            self.driver.find_element_by_id('js-value-amount').send_keys(keys.Keys.BACKSPACE)
-            self.driver.find_element_by_id('js-value-amount').send_keys(amount)        
             time.sleep(self.timeout)
-            self.driver.find_element_by_class_name('flex-container').click()
+            self.driver.find_element(By.CLASS_NAME, 'trade-action-container__right-action-button').click()
 
-        time.sleep(self.timeout)
-        self.driver_wait.until(EC.presence_of_element_located((By.ID, "netAmountDueDisplay")))
-        self.driver.find_element_by_class_name('trade-action-container__right-action-button').click()
-
-        self.close()
+            self.close()
 
+            return True
+        except Exception:
+            traceback.print_exc()
+            self.close()
+            return False
 
     def sell(self, ticker, amount=None, percentage=100):
-        self.open()
-
-        self.driver_wait.until(EC.presence_of_element_located(
-            (By.ID, "important-documents")))
-        self.driver.get('https://platform.easyequities.io/AccountOverview')
-        time.sleep(self.timeout)
-        self.driver.find_elements_by_xpath(
-            "//div[@aria-describedby='{0}']".format(self.account))[0].click()
-        time.sleep(self.timeout-2)
-        self.driver.get('https://platform.easyequities.io/ValueAllocation/Sell?contractCode=EQU.ZA.{0}'.format(ticker.upper()))
-        time.sleep(self.timeout-2)
+        try:
+            self.open()
+            self.driver.get('https://platform.easyequities.io/ValueAllocation/Sell?contractCode=EQU.ZA.{0}'.format(ticker.upper()))
+            self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "slick-track")))
+            self.driver.find_elements(By.XPATH, "//*[text()='{0}']".format(self.account))[0].click()
+
+            self.driver_wait.until(EC.invisibility_of_element_located((By.CLASS_NAME, "value-allocations__snapshot-price-request-loader")))
+            self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "flex-container")))
+            element = self.driver.find_element(By.CLASS_NAME, 'flex-container')
+            if element is not None:                
+                if amount == None:
+                    self.driver.find_element(By.ID, 'js-percentage-to-sell').send_keys(keys.Keys.CONTROL, 'a')
+                    self.driver.find_element(By.ID, 'js-percentage-to-sell').send_keys(keys.Keys.BACKSPACE)
+                    self.driver.find_element(By.ID, 'js-percentage-to-sell').send_keys(percentage)
+                    self.driver.find_element(By.ID, 'js-percentage-to-sell').send_keys(keys.Keys.ENTER)
+                else:   
+                    self.driver.find_element(By.ID, 'js-value-amount').send_keys(keys.Keys.CONTROL, 'a')
+                    self.driver.find_element(By.ID, 'js-value-amount').send_keys(keys.Keys.BACKSPACE)
+                    self.driver.find_element(By.ID, 'js-value-amount').send_keys(amount)
+                    self.driver.find_element(By.ID, 'js-value-amount').send_keys(keys.Keys.ENTER)
+                
+                self.driver_wait.until(EC.invisibility_of_element_located((By.CLASS_NAME, "value-allocations__snapshot-price-request-loader")))
+                self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "value-allocations__trade-button")))
+                self.driver.find_element(By.CLASS_NAME, "value-allocations__trade-button").click()
+
+                self.close()
+                return True
+
+            self.driver_wait.until(EC.presence_of_element_located((By.CLASS_NAME, "validation-summary-errors")))
+            element = self.driver.find_element(By.CLASS_NAME, "validation-summary-errors")
+            if element is not None:
+                self.close()
+                return False    
+        except:
+            traceback.print_exc()
+            self.close()
+            return False
+            
+
+if __name__ == '__main__':
+    username = None
+    password = None
+
+    from yahoo_fin import stock_info as si
+    import yfinance as yf
+
+    try:
+        username = ['Username']
+        password = ['Password']
+    except Exception as e:
+        print("ERROR:\t{0}".format(e))
+        sys.exit(1)
+    finally:
+        easy_equities = EasyEquities(username,  password, account='ZAR')
+
+        print(easy_equities.holdings())
+        for ticker in easy_equities.holdings():
+            if easy_equities.sell(ticker.get('Holding')) == True:
+                print(f"Sold {ticker.get('Holding')}")
+            else:
+                print(f"Failed to sell {ticker.get('Holding')}")
+            exit()
+    
+        if easy_equities.buy('CPI', shares = 1) == True:
+            print(f"Bought")
+        else:
+            print(f"Failed to buy")
         
-        if amount == None:
-            self.driver.find_element_by_id('js-percentage-to-sell').send_keys(keys.Keys.CONTROL, 'a')
-            self.driver.find_element_by_id('js-percentage-to-sell').send_keys(keys.Keys.BACKSPACE)
-            self.driver.find_element_by_id('js-percentage-to-sell').send_keys(percentage)
-            time.sleep(self.timeout)
-            self.driver.find_element_by_class_name('value-allocations__enter-value-container').click()
-        else:   
-            self.driver.find_element_by_id('js-value-amount').send_keys(keys.Keys.CONTROL, 'a')
-            self.driver.find_element_by_id('js-value-amount').send_keys(keys.Keys.BACKSPACE)
-            self.driver.find_element_by_id('js-value-amount').send_keys(amount)
-            time.sleep(self.timeout)
-            self.driver.find_element_by_class_name('value-allocations__enter-value-container').click()
-
-        time.sleep(self.timeout)
-        self.driver_wait.until(EC.presence_of_element_located(
-            (By.CLASS_NAME, "chartjs-render-monitor")))
-        self.driver.find_element_by_class_name(
-            'value-allocations__trade-button').click()
-
-        self.close()
-
+        if easy_equities.sell('CPI') == True:
+            print(f"Sold")
+        else:
+            print(f"Failed to sell")
 
+        print(easy_equities.balance())
```

### Comparing `EasyEquities-1.0.2/setup.py` & `EasyEquities-1.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 from distutils.core import setup
+
+# read the contents of your README file
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setup(
   name = 'EasyEquities',         # How you named your package folder (MyLib)
   packages = ['EasyEquities'],   # Chose the same as "name"
-  version = '1.0.2',      # Start with a small number and increase it with every change you make
+  version = '1.2.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'EasyEquities active scraper to issue trading instructions',   # Give a short description about your library
   author = 'Kloniphani Maxakadzi',                   # Type in your name
   author_email = 'Kloniphani@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/kloniphani/EasyEquities',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/kloniphani/EasyEquities/archive/refs/tags/v1.0.2.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/kloniphani/EasyEquities/archive/refs/tags/v1.2.3.tar.gz',    # I explain this later on
   keywords = ['South Africa', 'Trading', 'EasyEQuities'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'validators',
           'beautifulsoup4',
           'selenium',
           'urllib3',
           'webdriver_manager',
@@ -20,8 +26,11 @@
   classifiers=[
     'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
   ],
+  python_requires = ">=3.6",
+  long_description=long_description,
+  long_description_content_type='text/markdown'
 )
```

