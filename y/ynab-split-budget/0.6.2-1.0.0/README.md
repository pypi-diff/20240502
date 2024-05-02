# Comparing `tmp/ynab_split_budget-0.6.2.tar.gz` & `tmp/ynab_split_budget-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab_split_budget-0.6.2.tar", max compression
+gzip compressed data, was "ynab_split_budget-1.0.0.tar", max compression
```

## Comparing `ynab_split_budget-0.6.2.tar` & `ynab_split_budget-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0    35148 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/LICENSE
--rw-r--r--   0        0        0     4983 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/README.md
--rw-r--r--   0        0        0      810 2024-02-28 10:35:14.147175 ynab_split_budget-0.6.2/pyproject.toml
--rw-r--r--   0        0        0       61 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/__init__.py
--rw-r--r--   0        0        0     1865 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/__main__.py
--rw-r--r--   0        0        0     5611 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/client.py
--rw-r--r--   0        0        0      239 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/fileloader.py
--rw-r--r--   0        0        0        0 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/models/__init__.py
--rw-r--r--   0        0        0      194 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/models/account.py
--rw-r--r--   0        0        0      105 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/models/category.py
--rw-r--r--   0        0        0      247 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/models/exception.py
--rw-r--r--   0        0        0      803 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/models/splittransaction.py
--rw-r--r--   0        0        0      503 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/models/transaction.py
--rw-r--r--   0        0        0      185 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/models/user.py
--rw-r--r--   0        0        0     2403 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/syncrepository.py
--rw-r--r--   0        0        0     3556 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/transactionbuilder.py
--rw-r--r--   0        0        0     1100 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/userloader.py
--rw-r--r--   0        0        0     2813 2024-02-28 10:34:57.535161 ynab_split_budget-0.6.2/ynabsplitbudget/ynabsplitbudget.py
--rw-r--r--   0        0        0     5729 1970-01-01 00:00:00.000000 ynab_split_budget-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5110 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/README.md
+-rw-r--r--   0        0        0      842 2024-05-02 06:32:08.895079 ynab_split_budget-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/__init__.py
+-rw-r--r--   0        0        0     2449 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/__main__.py
+-rw-r--r--   0        0        0     2215 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/adjusters.py
+-rw-r--r--   0        0        0     4230 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/client.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/models/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/models/account.py
+-rw-r--r--   0        0        0      105 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/models/category.py
+-rw-r--r--   0        0        0      247 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/models/exception.py
+-rw-r--r--   0        0        0      503 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/models/transaction.py
+-rw-r--r--   0        0        0     1741 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/models/user.py
+-rw-r--r--   0        0        0      945 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/splitparser.py
+-rw-r--r--   0        0        0     2634 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/syncrepository.py
+-rw-r--r--   0        0        0     2216 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/transactionbuilder.py
+-rw-r--r--   0        0        0     5325 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/ynabsplitbudget.py
+-rw-r--r--   0        0        0     5929 1970-01-01 00:00:00.000000 ynab_split_budget-1.0.0/PKG-INFO
```

### Comparing `ynab_split_budget-0.6.2/LICENSE` & `ynab_split_budget-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab_split_budget-0.6.2/README.md` & `ynab_split_budget-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # ynab-split-budget
 
 [![GitHub Release](https://img.shields.io/github/release/dnbasta/ynab-split-budget?style=flat)]() 
 [![Github Release](https://img.shields.io/maintenance/yes/2100)]()
+[![Monthly downloads](https://img.shields.io/pypi/dm/ynab-split-budget)]()
 
 This library enables cost sharing across two YNAB budgets. It requires two dedicated accounts in each budget to which
 each budget owner can transfer amounts from their own budget. Each transfer is considered as its opposite in the other 
 account.
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/dnbasta)
 
@@ -14,106 +15,90 @@
 2. Create a personal access token for both budgets as described [here](https://api.ynab.com/)
 
 ## Install library from PyPI
 
 ```bash
 pip install ynab-split-budget
 ```
+## Usage
+### 1. Create a transaction
+Create a transaction in the budget and add a specific flag color for the splits. The 
+transaction needs to be cleared in order to be considered by this library. By default, the transaction will be split 
+in half, but you can specify a different split by adding `@x%` for percentage or `@x` for specific amount in the memo 
+of the transaction. The amount you specify in this split will be transferred to your sharing account. You can also 
+create a plain transfer to the shared account which will be completely allocated to the partner account.
+
+### 2. Initialize library
+Initialize the library by creating two `User` instances and pass them as user and partner to the constructor of the 
+main class. For the flag_color set the value used marking the transaction earlier. Possible color values are `red`, 
+`orange`, `yellow`, `green`, `blue` and `purple`. The id of the budget and of the account can be found going to 
+https://app.ynab.com/ and opening the target account by clicking on the name on the left hand side menu. The URL does 
+now contain both IDs `https://app.ynab.com/<budget_id>/accounts/<account_id>`. 
+The `User` object can be optionally initialized from a YAML file using the `from_yaml()` classmethod.
+```py
+from ynabsplitbudget import YnabSplitBudget, User
 
-## Create config
-Create a config `dict` with the below structure. 
+user = User(name='<name>', token='<token>', budget_id='<budget_id>', 
+            account_id='<account_id', flag_color='<flag_color>')
+
+partner = User(name='<name>', token='<token>', budget_id='<budget_id>', 
+               account_id='<account_id', flag_color='<flag_color>')
+
+split_budget = YnabSplitBudget(user=user, partner=partner)
+```
+### 3. Split transactions
+Call the `split()` method of the instance. It will split flagged transactions in the budget into a subtransaction with
+the original category and a transfer to the split account. By default, the transfer transactions will show up as 
+uncleared in the split account. The optional `clear` parameter allows to automatically clear the transactions in 
+the split account. The function returns the updated transactions after applying the split.
 ```py
-CONFIG = {
-    '<user_name>': {
-        'budget': '<budget_id>',
-        'account': '<account_id>',
-        'token': '<ynab_token>',
-        'flag': '<color>'},
-    '<partner_name>': {
-        'budget': '<budget_id>',
-        'account': '<account_id>',
-        'token': '<ynab_token>',
-        'flag': '<color>'}
-}
-```
-You can find the ID of the budget and of the account if you go to https://app.ynab.com/ and open the target account by
-clicking on the name on the left hand side menu. The URL does now contain both IDs 
-`https://app.ynab.com/<budget_id>/accounts/<account_id>`
-Possible colors for the flag value are `red`, `orange`, `yellow`, `green`, `blue` and `purple`
-
-Alternatively you can save the config in a yaml file with the below structure and provide the path to the library 
-when initializing
-```yaml
-<user_name>:
-  token: <ynab_token>
-  budget: <budget_id>
-  account: <account_id>
-  flag: <color>
-<partner_name>:
-  token: <ynab_token>
-  budget: <budget_id>
-  account: <account_id>
-  flag: <color>
+split_budget.split()
 ```
 
-## Usage
-### 1. Create a transaction
-Create a transaction in your budget and add the defined color flag. Only cleared transactions will be considered. 
-By default, the transaction will be split in half, but you can specify a different split by adding
-`@x%` for percentage or `@x` for specific amount in the memo of the transaction. The amount you specify
-in this split will be transferred to your sharing account. You can also create a plain transfer to the shared account 
-which will be completely allocated to the partner account.
-### 2. Initialize and run the split functionality
-
-```py
-from ynabsplitbudget import YnabSplitBudget
-
-# initialize from config dict
-ynab_split_budget = YnabSplitBudget(config=CONFIG, user='<user_name>')
-# or alternatively from yaml
-ynab_split_budget = YnabSplitBudget.from_yaml(path='path/to/config.yaml', user='<user_name')
-
-ynab_split_budget.split_transactions()
-```
-### 3. Clear the newly split transaction
-Using the YNAB web interface go to your split account and clear the newly split transaction over there. 
-This can currently not be automated as YNAB API can't clear split transactions at this point in time.
-### 4. Run the insert functionality
-By default the library will compare and insert transactions of the last 30 days. If you would like to do it for a
-different timeframe you can provide a `since` argument to the function with a value from `datetime.date`
+### 4. Push new splits to partner split account
+Calling the `push()` function will insert new transactions from user split account into split account of partner to keep
+both accounts in sync. By default, the function will compare and insert transactions of the last 30 days. Optionally it 
+takes a `since` parameter in the form of `datetime.date` to set a timeframe different from 30 days. 
+
 ```py
-ynab_split_budget.insert_complements()
+split_budget.push()
 ```
 ## Advanced Usage
 ### Check Balances
-Additionally you can check if the cleared balances in both accounts match. If they don't match you will get back a
-`BalancesDontMatch` Error which also gives you the two values of the balances.
+The `raise_on_balances_off()` function compares the cleared balances in both split accounts. If they don't match it 
+will raise a `BalancesDontMatch` error which includes the values of the balances.
 ```py
-ynab_split_budget.raise_on_balances_off()
+split_budget.raise_on_balances_off()
 ```
 ### Delete Orphaned Complements
-If you delete a transaction in your share account you can use this function to delete the respective complement on your
-partners shared account. It does return a list with the deleted transactions. By default the library will compare 
-transactions of the last 30 days. If you would like to do it for a different timeframe you can provide a `since` 
-argument to the function with a value from `datetime.date`
-```py
-ynab_split_budget.delete_orphaned_complements()
+The `delete_orphans()` function deletes orphaned transactions in the partner split account, which don't have a 
+corresponding transaction in the user split account any more. It does return a list with the deleted transactions. 
+By default, the function compares transactions of the last 30 days. Optionally it takes a `since` parameter in the 
+form of `datetime.date` to set a timeframe different from 30 days.
+```py
+split_budget.delete_orphans()
+```
+### Reconcile split account
+The `reconcile()` function allows to reconcile the split account. It does check if the balances match before reconciling
+and will an `BalancesDontMatch` error if they don't.
+```py 
+split_budget.reconcile()
 ```
+
 ### Show Logs
-The library logs information about the result of the methods on the 'INFO' level. If you want to see these logs import
-the logging module and set in to the level `INFO`. You can also access the logger for advanced configuration via the  
-`logger` attribute of your `YnabSplitBudget`instance.
+The library logs information about the result of the methods at the 'INFO' level. The logs can be made visible by 
+importing the logging module and set it to the level `INFO`. The logger itself can also be accessed via the `logger` 
+attribute of the instance.
 ```py
 import logging
 
 logging.basicConfig(level='INFO')
 ```
-### Run via bash commands
-You can run this package also from bash with the following commands
+### Run via bash
+You can run this library also from bash with the following basic structure
 ```bash
-$ python -m ynabsplitbudget -c <path/config.yaml#user_name> -s | --split-transactions
-$ python -m ynabsplitbudget -c <path/config.yaml#user_name> -i | --insert-complements [-d | --since-date "YYYY-mm-dd"]
-$ python -m ynabsplitbudget -c <path/config.yaml#user_name> -b | --check-balances
+$ python -m ynabsplitbudget -u <path/user.yaml> -p <path/partner.yaml> --split
+```
+For a complete list of available bash options please use
+```bash
+$ python -m ynabsplitbudget -h | -- help
 ```
-## Development
-
-Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

### Comparing `ynab_split_budget-0.6.2/pyproject.toml` & `ynab_split_budget-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry-core.masonry.api"
 
 [tool.poetry]
 name = "ynab-split-budget"
-version = "0.6.2"
+version = "1.0.0"
 authors = ["Daniel Basta <ynab@basta.info>"]
 description = "Library to split and share You Need A Budget (YNAB) transactions between two budgets"
 readme = "README.md"
 license = 'MIT'
 packages = [{include = 'ynabsplitbudget'}]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = '>=3.8'
-pyyaml = '>=6.0'
-requests = '>=2.28'
+python = '^3.8'
+pyyaml = '^6.0'
+requests = '^2.28'
+ynab-transaction-adjuster= '^2.0.0'
 
 [tool.poetry.group.dev.dependencies]
-pytest = ">=8.0.0"
+pytest = "^8.0.0"
 
 [poetry.urls]
 "Homepage" = "https://github.com/dnbasta/ynab-split-budget"
 "Bug Tracker" = "https://github.com/dnbasta/ynab-split-budget/issues"
```

### Comparing `ynab_split_budget-0.6.2/ynabsplitbudget/client.py` & `ynab_split_budget-1.0.0/ynabsplitbudget/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,154 +1,106 @@
 from dataclasses import dataclass
 from datetime import date, datetime
 from typing import List, Union
 
 import requests
 from requests import HTTPError
 
-from ynabsplitbudget.models.splittransaction import SplitTransaction
-from ynabsplitbudget.transactionbuilder import TransactionBuilder, SplitTransactionBuilder
-from ynabsplitbudget.models.exception import BudgetNotFound, AccountNotFound
 from ynabsplitbudget.models.account import Account
+from ynabsplitbudget.models.exception import BudgetNotFound, AccountNotFound
+from ynabsplitbudget.transactionbuilder import TransactionBuilder
 from ynabsplitbudget.models.transaction import RootTransaction, LookupTransaction, ComplementTransaction
-from ynabsplitbudget.models.user import User
 
 YNAB_BASE_URL = 'https://api.ynab.com/v1/'
 
 
-class ClientMixin:
-	_token: str
-
-	def _header(self):
-		return {'Authorization': f'Bearer {self._token}'}
-
-	def _get(self, url: str, params: dict = None) -> dict:
-		r = requests.get(url, params=params, headers=self._header())
-		r.raise_for_status()
-		return r.json()['data']
-
-
-class BaseClient(ClientMixin):
+@dataclass
+class Client:
 
-	def __init__(self, token: str, user_name: str):
-		self._token = token
-		self._user_name = user_name
+	def __init__(self, user_name: str, budget_id: str, account_id: str, token: str):
+		self.session = requests.Session()
+		self.session.headers.update({'Authorization': f'Bearer {token}'})
+		self.user_name = user_name
+		self.budget_id = budget_id
+		self.account_id = account_id
+		self.transaction_builder = TransactionBuilder(account_id=self.account_id)
 
 	def fetch_account(self, budget_id: str, account_id: str) -> Account:
-		url = f'{YNAB_BASE_URL}budgets?include_accounts=true'
-		data_dict = self._get(url)
+		r = self.session.get(f'{YNAB_BASE_URL}budgets', params=dict(include_accounts=True))
+		r.raise_for_status()
+		data_dict = r.json()['data']
 
 		try:
 			budget = next(b for b in data_dict['budgets'] if b['id'] == budget_id)
 		except StopIteration:
-			raise BudgetNotFound(f"No budget with id '{budget_id} found for {self._user_name}'")
+			raise BudgetNotFound(f"No budget with id '{budget_id} found for {self.user_name}'")
 
 		try:
 			account = next(a for a in budget['accounts'] if a['id'] == account_id and a['deleted'] is False)
 		except StopIteration:
 			raise AccountNotFound(f"No Account with id '{account_id}' fund in budget '{budget['name']} "
-								  f"for user {self._user_name}'")
+								  f"for user {self.user_name}'")
 
 		return Account(budget_id=budget_id,
 					   budget_name=budget['name'],
 					   account_id=account_id,
 					   account_name=account['name'],
 					   transfer_payee_id=account['transfer_payee_id'],
 					   currency=budget['currency_format']['iso_code'])
 
-
-@dataclass
-class SyncClient(ClientMixin):
-
-	def __init__(self, user: User):
-		self._token = user.token
-		self.user = user
-		self.transaction_builder = TransactionBuilder(user=user)
-
 	def fetch_roots(self, since: date) -> List[RootTransaction]:
-		url = (f'{YNAB_BASE_URL}budgets/{self.user.account.budget_id}/accounts/'
-			   f'{self.user.account.account_id}/transactions')
-
-		transactions_dicts = self._get(url, params={'since_date': datetime.strftime(since, '%Y-%m-%d')})['transactions']
+		url = f'{YNAB_BASE_URL}budgets/{self.budget_id}/accounts/{self.account_id}/transactions'
+		r = self.session.get(url, params={'since_date': datetime.strftime(since, '%Y-%m-%d')})
+		r.raise_for_status()
+		transactions_dicts = r.json()['data']['transactions']
 		transactions_filtered = [t for t in transactions_dicts if not t['cleared'] == 'uncleared'
 							  and t['deleted'] is False
 							  and (t['import_id'] is None or 's||' not in t['import_id'])
 							  and t['payee_name'] != 'Reconciliation Balance Adjustment']
 		transactions = [self.transaction_builder.build_root(t_dict=t) for t in transactions_filtered]
 		return transactions
 
 	def fetch_lookup(self, since: date) -> List[Union[RootTransaction, LookupTransaction, ComplementTransaction]]:
-		url = f'{YNAB_BASE_URL}budgets/{self.user.account.budget_id}/transactions'
-		data_dict = self._get(url, params={'since_date': datetime.strftime(since, '%Y-%m-%d')})
-		transactions = [self.transaction_builder.build(t_dict=t) for t in data_dict['transactions']]
+		url = f'{YNAB_BASE_URL}budgets/{self.budget_id}/transactions'
+		r = self.session.get(url, params={'since_date': datetime.strftime(since, '%Y-%m-%d')})
+		r.raise_for_status()
+		data_dict = r.json()['data']['transactions']
+		transactions = [self.transaction_builder.build(t_dict=t) for t in data_dict]
 		return transactions
 
-	def insert_complement(self, t: RootTransaction):
+	def insert_complement(self, t: RootTransaction) -> ComplementTransaction:
 		iteration = 0
-		try_again = True
-		while try_again:
+		while True:
 			try:
-				self._insert(t, iteration=iteration)
-				try_again = False
+				return self._insert(t, iteration=iteration)
 			except HTTPError as e:
 				if e.response.status_code == 409:
 					iteration += 1
 
-	def _insert(self, t: RootTransaction, iteration: int):
-		url = f'{YNAB_BASE_URL}budgets/{self.user.account.budget_id}/transactions'
+	def _insert(self, t: RootTransaction, iteration: int) -> ComplementTransaction:
+		url = f'{YNAB_BASE_URL}budgets/{self.budget_id}/transactions'
 		data = {'transaction': {
-			"account_id": self.user.account.account_id,
+			"account_id": self.account_id,
 			"date": t.transaction_date.strftime("%Y-%m-%d"),
 			"amount": - t.amount,
 			"payee_name": t.payee_name,
 			"memo": t.memo,
 			"cleared": 'cleared',
 			"approved": False,
 			"import_id": f's||{t.share_id}||{iteration}'
 		}}
-		r = requests.post(url, json=data, headers=self._header())
+		r = self.session.post(url, json=data)
 		r.raise_for_status()
+		complement = self.transaction_builder.build_complement(r.json()['data']['transaction'])
+		return complement
 
 	def fetch_balance(self) -> int:
-		url = f'{YNAB_BASE_URL}budgets/{self.user.account.budget_id}/accounts/{self.user.account.account_id}'
-		data_dict = self._get(url)
-		return data_dict['account']['cleared_balance']
-
-	def delete_complement(self, transaction_id: str) -> None:
-		url = f'{YNAB_BASE_URL}budgets/{self.user.account.budget_id}/transactions/{transaction_id}'
-		r = requests.delete(url, headers=self._header())
+		url = f'{YNAB_BASE_URL}budgets/{self.budget_id}/accounts/{self.account_id}'
+		r = self.session.get(url)
 		r.raise_for_status()
+		balance = r.json()['data']['account']['cleared_balance']
+		return balance
 
-
-class SplitClient(ClientMixin):
-
-	def __init__(self, user: User):
-		self._token = user.token
-		self.user = user
-
-	def fetch_new_to_split(self) -> List[SplitTransaction]:
-		url = f'{YNAB_BASE_URL}budgets/{self.user.account.budget_id}/transactions'
-
-		data_dict = self._get(url)
-		transactions_dicts = [t for t in data_dict['transactions'] if not t['cleared'] == 'uncleared'
-							  and t['deleted'] is False and len(t['subtransactions']) == 0]
-		stb = SplitTransactionBuilder()
-		flag_splits = [stb.build(t) for t in transactions_dicts if t['flag_color'] == self.user.flag]
-
-		return [s for s in flag_splits if s is not None]
-
-	def insert_split(self, t: SplitTransaction):
-		data = {'transaction': {
-			"subtransactions": [{"amount": int(round(t.split_amount)),
-								 "payee_id": self.user.account.transfer_payee_id,
-								 "memo": t.memo,
-								 "cleared": "cleared"
-								},
-								{"amount": int(t.amount - round(t.split_amount)),
-								 "category_id": t.category.id,
-								 "cleared": "cleared"
-								 }]
-		}}
-		url = f'{YNAB_BASE_URL}budgets/{self.user.account.budget_id}/transactions/{t.id}'
-
-		r = requests.put(url, json=data, headers=self._header())
+	def delete_complement(self, transaction_id: str) -> None:
+		url = f'{YNAB_BASE_URL}budgets/{self.budget_id}/transactions/{transaction_id}'
+		r = self.session.delete(url)
 		r.raise_for_status()
```

### Comparing `ynab_split_budget-0.6.2/ynabsplitbudget/syncrepository.py` & `ynab_split_budget-1.0.0/ynabsplitbudget/syncrepository.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from datetime import date
 from typing import List, Union
 
-from ynabsplitbudget.client import SyncClient
+from ynabsplitbudget.client import Client
 from ynabsplitbudget.models.transaction import RootTransaction, ComplementTransaction, LookupTransaction
 from ynabsplitbudget.models.user import User
 
 
 class SyncRepository:
 
 	def __init__(self, user: User, partner: User):
-		self._user_client = SyncClient(user)
-		self._partner_client = SyncClient(partner)
+		self._user_client = Client(token=user.token, budget_id=user.budget_id, account_id=user.account_id,
+								   user_name=user.name)
+		self._partner_client = Client(token=partner.token, budget_id=partner.budget_id, account_id=partner.account_id,
+									  user_name=partner.name)
 
 	def fetch_roots_wo_complement(self, since: date) -> List[RootTransaction]:
 		roots = self._user_client.fetch_roots(since=since)
 		pl = [t for t in self._partner_client.fetch_lookup(since) if isinstance(t, ComplementTransaction)]
 		roots_wo_complement = [t for t in roots if t.share_id not in [lo.share_id for lo in pl]]
 		transactions_replaced_payee = self.replace_payee(transactions=roots_wo_complement,
 															 lookup_date=since)
 		return transactions_replaced_payee
 
-	def insert_complements(self, transactions: List[RootTransaction]):
-		[self._partner_client.insert_complement(t) for t in transactions]
+	def insert_complements(self, transactions: List[RootTransaction]) -> List[ComplementTransaction]:
+		return [self._partner_client.insert_complement(t) for t in transactions]
 
 	def replace_payee(self, transactions: List[RootTransaction], lookup_date: date) -> List[RootTransaction]:
 		ul = self._user_client.fetch_lookup(lookup_date)
 		pr = PayeeReplacer(lookup=ul)
 		transactions_replaced = [pr.replace(t) for t in transactions]
 		return transactions_replaced
```

### Comparing `ynab_split_budget-0.6.2/PKG-INFO` & `ynab_split_budget-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.1
 Name: ynab-split-budget
-Version: 0.6.2
+Version: 1.0.0
 Summary: Library to split and share You Need A Budget (YNAB) transactions between two budgets
 License: MIT
 Author: Daniel Basta
 Author-email: ynab@basta.info
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pyyaml (>=6.0)
-Requires-Dist: requests (>=2.28)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.28,<3.0)
+Requires-Dist: ynab-transaction-adjuster (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ynab-split-budget
 
 [![GitHub Release](https://img.shields.io/github/release/dnbasta/ynab-split-budget?style=flat)]() 
 [![Github Release](https://img.shields.io/maintenance/yes/2100)]()
+[![Monthly downloads](https://img.shields.io/pypi/dm/ynab-split-budget)]()
 
 This library enables cost sharing across two YNAB budgets. It requires two dedicated accounts in each budget to which
 each budget owner can transfer amounts from their own budget. Each transfer is considered as its opposite in the other 
 account.
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/dnbasta)
 
@@ -34,107 +36,91 @@
 2. Create a personal access token for both budgets as described [here](https://api.ynab.com/)
 
 ## Install library from PyPI
 
 ```bash
 pip install ynab-split-budget
 ```
+## Usage
+### 1. Create a transaction
+Create a transaction in the budget and add a specific flag color for the splits. The 
+transaction needs to be cleared in order to be considered by this library. By default, the transaction will be split 
+in half, but you can specify a different split by adding `@x%` for percentage or `@x` for specific amount in the memo 
+of the transaction. The amount you specify in this split will be transferred to your sharing account. You can also 
+create a plain transfer to the shared account which will be completely allocated to the partner account.
+
+### 2. Initialize library
+Initialize the library by creating two `User` instances and pass them as user and partner to the constructor of the 
+main class. For the flag_color set the value used marking the transaction earlier. Possible color values are `red`, 
+`orange`, `yellow`, `green`, `blue` and `purple`. The id of the budget and of the account can be found going to 
+https://app.ynab.com/ and opening the target account by clicking on the name on the left hand side menu. The URL does 
+now contain both IDs `https://app.ynab.com/<budget_id>/accounts/<account_id>`. 
+The `User` object can be optionally initialized from a YAML file using the `from_yaml()` classmethod.
+```py
+from ynabsplitbudget import YnabSplitBudget, User
 
-## Create config
-Create a config `dict` with the below structure. 
+user = User(name='<name>', token='<token>', budget_id='<budget_id>', 
+            account_id='<account_id', flag_color='<flag_color>')
+
+partner = User(name='<name>', token='<token>', budget_id='<budget_id>', 
+               account_id='<account_id', flag_color='<flag_color>')
+
+split_budget = YnabSplitBudget(user=user, partner=partner)
+```
+### 3. Split transactions
+Call the `split()` method of the instance. It will split flagged transactions in the budget into a subtransaction with
+the original category and a transfer to the split account. By default, the transfer transactions will show up as 
+uncleared in the split account. The optional `clear` parameter allows to automatically clear the transactions in 
+the split account. The function returns the updated transactions after applying the split.
 ```py
-CONFIG = {
-    '<user_name>': {
-        'budget': '<budget_id>',
-        'account': '<account_id>',
-        'token': '<ynab_token>',
-        'flag': '<color>'},
-    '<partner_name>': {
-        'budget': '<budget_id>',
-        'account': '<account_id>',
-        'token': '<ynab_token>',
-        'flag': '<color>'}
-}
-```
-You can find the ID of the budget and of the account if you go to https://app.ynab.com/ and open the target account by
-clicking on the name on the left hand side menu. The URL does now contain both IDs 
-`https://app.ynab.com/<budget_id>/accounts/<account_id>`
-Possible colors for the flag value are `red`, `orange`, `yellow`, `green`, `blue` and `purple`
-
-Alternatively you can save the config in a yaml file with the below structure and provide the path to the library 
-when initializing
-```yaml
-<user_name>:
-  token: <ynab_token>
-  budget: <budget_id>
-  account: <account_id>
-  flag: <color>
-<partner_name>:
-  token: <ynab_token>
-  budget: <budget_id>
-  account: <account_id>
-  flag: <color>
+split_budget.split()
 ```
 
-## Usage
-### 1. Create a transaction
-Create a transaction in your budget and add the defined color flag. Only cleared transactions will be considered. 
-By default, the transaction will be split in half, but you can specify a different split by adding
-`@x%` for percentage or `@x` for specific amount in the memo of the transaction. The amount you specify
-in this split will be transferred to your sharing account. You can also create a plain transfer to the shared account 
-which will be completely allocated to the partner account.
-### 2. Initialize and run the split functionality
-
-```py
-from ynabsplitbudget import YnabSplitBudget
-
-# initialize from config dict
-ynab_split_budget = YnabSplitBudget(config=CONFIG, user='<user_name>')
-# or alternatively from yaml
-ynab_split_budget = YnabSplitBudget.from_yaml(path='path/to/config.yaml', user='<user_name')
-
-ynab_split_budget.split_transactions()
-```
-### 3. Clear the newly split transaction
-Using the YNAB web interface go to your split account and clear the newly split transaction over there. 
-This can currently not be automated as YNAB API can't clear split transactions at this point in time.
-### 4. Run the insert functionality
-By default the library will compare and insert transactions of the last 30 days. If you would like to do it for a
-different timeframe you can provide a `since` argument to the function with a value from `datetime.date`
+### 4. Push new splits to partner split account
+Calling the `push()` function will insert new transactions from user split account into split account of partner to keep
+both accounts in sync. By default, the function will compare and insert transactions of the last 30 days. Optionally it 
+takes a `since` parameter in the form of `datetime.date` to set a timeframe different from 30 days. 
+
 ```py
-ynab_split_budget.insert_complements()
+split_budget.push()
 ```
 ## Advanced Usage
 ### Check Balances
-Additionally you can check if the cleared balances in both accounts match. If they don't match you will get back a
-`BalancesDontMatch` Error which also gives you the two values of the balances.
+The `raise_on_balances_off()` function compares the cleared balances in both split accounts. If they don't match it 
+will raise a `BalancesDontMatch` error which includes the values of the balances.
 ```py
-ynab_split_budget.raise_on_balances_off()
+split_budget.raise_on_balances_off()
 ```
 ### Delete Orphaned Complements
-If you delete a transaction in your share account you can use this function to delete the respective complement on your
-partners shared account. It does return a list with the deleted transactions. By default the library will compare 
-transactions of the last 30 days. If you would like to do it for a different timeframe you can provide a `since` 
-argument to the function with a value from `datetime.date`
-```py
-ynab_split_budget.delete_orphaned_complements()
+The `delete_orphans()` function deletes orphaned transactions in the partner split account, which don't have a 
+corresponding transaction in the user split account any more. It does return a list with the deleted transactions. 
+By default, the function compares transactions of the last 30 days. Optionally it takes a `since` parameter in the 
+form of `datetime.date` to set a timeframe different from 30 days.
+```py
+split_budget.delete_orphans()
+```
+### Reconcile split account
+The `reconcile()` function allows to reconcile the split account. It does check if the balances match before reconciling
+and will an `BalancesDontMatch` error if they don't.
+```py 
+split_budget.reconcile()
 ```
+
 ### Show Logs
-The library logs information about the result of the methods on the 'INFO' level. If you want to see these logs import
-the logging module and set in to the level `INFO`. You can also access the logger for advanced configuration via the  
-`logger` attribute of your `YnabSplitBudget`instance.
+The library logs information about the result of the methods at the 'INFO' level. The logs can be made visible by 
+importing the logging module and set it to the level `INFO`. The logger itself can also be accessed via the `logger` 
+attribute of the instance.
 ```py
 import logging
 
 logging.basicConfig(level='INFO')
 ```
-### Run via bash commands
-You can run this package also from bash with the following commands
+### Run via bash
+You can run this library also from bash with the following basic structure
 ```bash
-$ python -m ynabsplitbudget -c <path/config.yaml#user_name> -s | --split-transactions
-$ python -m ynabsplitbudget -c <path/config.yaml#user_name> -i | --insert-complements [-d | --since-date "YYYY-mm-dd"]
-$ python -m ynabsplitbudget -c <path/config.yaml#user_name> -b | --check-balances
+$ python -m ynabsplitbudget -u <path/user.yaml> -p <path/partner.yaml> --split
+```
+For a complete list of available bash options please use
+```bash
+$ python -m ynabsplitbudget -h | -- help
 ```
-## Development
-
-Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
```

