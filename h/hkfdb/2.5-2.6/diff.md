# Comparing `tmp/hkfdb-2.5.tar.gz` & `tmp/hkfdb-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkfdb-2.5.tar", last modified: Mon Apr  3 04:19:12 2023, max compression
+gzip compressed data, was "hkfdb-2.6.tar", last modified: Sun Apr 16 06:42:34 2023, max compression
```

## Comparing `hkfdb-2.5.tar` & `hkfdb-2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 04:19:12.366398 hkfdb-2.5/
--rw-rw-rw-   0        0        0    35149 2021-07-30 00:33:11.000000 hkfdb-2.5/LICENSE
--rw-rw-rw-   0        0        0     1651 2023-04-03 04:19:12.366398 hkfdb-2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-03-30 03:29:25.000000 hkfdb-2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 04:19:12.366398 hkfdb-2.5/hkfdb/
--rw-rw-rw-   0        0        0    90085 2023-04-03 04:17:54.000000 hkfdb-2.5/hkfdb/Database.py
--rw-rw-rw-   0        0        0       23 2021-09-12 13:30:45.000000 hkfdb-2.5/hkfdb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 04:19:12.366398 hkfdb-2.5/hkfdb.egg-info/
--rw-rw-rw-   0        0        0     1651 2023-04-03 04:19:12.000000 hkfdb-2.5/hkfdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-03 04:19:12.000000 hkfdb-2.5/hkfdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 04:19:12.000000 hkfdb-2.5/hkfdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-03 04:19:12.000000 hkfdb-2.5/hkfdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-03 04:19:12.000000 hkfdb-2.5/hkfdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 04:19:12.366398 hkfdb-2.5/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-04-03 04:17:18.000000 hkfdb-2.5/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-16 06:42:34.531413 hkfdb-2.6/
+-rw-rw-rw-   0 cmw        (501) staff       (20)    35149 2021-07-30 00:33:11.000000 hkfdb-2.6/LICENSE
+-rw-r--r--   0 cmw        (501) staff       (20)     1618 2023-04-16 06:42:34.531223 hkfdb-2.6/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1243 2023-03-30 03:29:25.000000 hkfdb-2.6/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-16 06:42:34.530286 hkfdb-2.6/hkfdb/
+-rw-r--r--   0 cmw        (501) staff       (20)    90392 2023-04-16 06:32:33.000000 hkfdb-2.6/hkfdb/Database.py
+-rw-rw-rw-   0 cmw        (501) staff       (20)       23 2021-09-12 13:30:45.000000 hkfdb-2.6/hkfdb/__init__.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-16 06:42:34.531017 hkfdb-2.6/hkfdb.egg-info/
+-rw-rw-rw-   0 cmw        (501) staff       (20)     1618 2023-04-16 06:42:34.000000 hkfdb-2.6/hkfdb.egg-info/PKG-INFO
+-rw-rw-rw-   0 cmw        (501) staff       (20)      206 2023-04-16 06:42:34.000000 hkfdb-2.6/hkfdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        1 2023-04-16 06:42:34.000000 hkfdb-2.6/hkfdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)       44 2023-04-16 06:42:34.000000 hkfdb-2.6/hkfdb.egg-info/requires.txt
+-rw-rw-rw-   0 cmw        (501) staff       (20)        6 2023-04-16 06:42:34.000000 hkfdb-2.6/hkfdb.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-04-16 06:42:34.531465 hkfdb-2.6/setup.cfg
+-rw-rw-rw-   0 cmw        (501) staff       (20)      761 2023-04-16 06:42:27.000000 hkfdb-2.6/setup.py
```

### Comparing `hkfdb-2.5/LICENSE` & `hkfdb-2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hkfdb-2.5/PKG-INFO` & `hkfdb-2.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,74 @@
-Metadata-Version: 2.1
-Name: hkfdb
-Version: 2.5
-Summary: Hong Kong Finance Database.
-Home-page: https://www.hkfdb.net
-Author: Hong Kong Finance Database Team
-Author-email: info@hkfdb.net
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Hong Kong Finance Database
-
-To install the latest version:
-```
-pip install hkfdb
-```
-
-Before you start, please make sure you have done the following:
-* **subscribe** the data from our website
-* get the personal authToken 
-* create an client object from class Database
-* have fun!
-
-create client object with authToken and class Database:
-```
-import hkfdb
-
-authToken = 'personal_authToken'
-client = hkfdb.Database(authToken)
-```
-
-**Major Functions**
-
-Price Data:
-* get_hk_stock_ohlc() 
-* get_us_stock_ohlc()
-* get_hk_fut_ohlc()
-* get_hk_deri_daily_market_report()
-
-CCASS Data:
-* get_ccass_all_id()
-* get_ccass_by_code()
-* get_ccass_holding_rank()
-* get_ccass_by_id()
-* get_ccass_by_id_change()
-
-Index list:
-* get_spx_index_const()
-* get_hk_index_const()
-* get_hk_stock_plate_const()
-* get_all_hk_index_name()
-* get_all_hk_stock_plate_name()
-
-Earning Calendar:
-* get_us_earning_calendar_by_date()
-* get_us_earning_calendar_by_code()
-* get_hk_earning_calendar_by_code()
-* get_hk_earning_calendar_by_date()
-
-Other:
-* get_hk_market_cap_hist()
-* get_hk_ipo_hist()
-* get_north_water()
-* get_market_highlight()
-* get_hk_buyback_by_date()
-* get_hk_buyback_by_code()
-* get_basic_hk_stock_info()
+Metadata-Version: 2.1
+Name: hkfdb
+Version: 2.6
+Summary: Hong Kong Finance Database.
+Home-page: https://www.hkfdb.net
+Author: Hong Kong Finance Database Team
+Author-email: info@hkfdb.net
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hong Kong Finance Database
+
+To install the latest version:
+```
+pip install hkfdb
+```
+
+Before you start, please make sure you have done the following:
+* **subscribe** the data from our website
+* get the personal authToken 
+* create an client object from class Database
+* have fun!
+
+create client object with authToken and class Database:
+```
+import hkfdb
+
+authToken = 'personal_authToken'
+client = hkfdb.Database(authToken)
+```
+
+**Major Functions**
+
+Price Data:
+* get_hk_stock_ohlc() 
+* get_us_stock_ohlc()
+* get_hk_fut_ohlc()
+* get_hk_deri_daily_market_report()
+
+CCASS Data:
+* get_ccass_all_id()
+* get_ccass_by_code()
+* get_ccass_holding_rank()
+* get_ccass_by_id()
+* get_ccass_by_id_change()
+
+Index list:
+* get_spx_index_const()
+* get_hk_index_const()
+* get_hk_stock_plate_const()
+* get_all_hk_index_name()
+* get_all_hk_stock_plate_name()
+
+Earning Calendar:
+* get_us_earning_calendar_by_date()
+* get_us_earning_calendar_by_code()
+* get_hk_earning_calendar_by_code()
+* get_hk_earning_calendar_by_date()
+
+Other:
+* get_hk_market_cap_hist()
+* get_hk_ipo_hist()
+* get_north_water()
+* get_market_highlight()
+* get_hk_buyback_by_date()
+* get_hk_buyback_by_code()
+* get_basic_hk_stock_info()
+
+
```

### Comparing `hkfdb-2.5/README.md` & `hkfdb-2.6/README.md`

 * *Files identical despite different names*

### Comparing `hkfdb-2.5/hkfdb/Database.py` & `hkfdb-2.6/hkfdb/Database.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,33 +199,38 @@
         else:
             err_msg = 'Error in: '
             for error in check_bool_dict:
                 if check_bool_dict[error] == False:
                     err_msg += error + ','
             print(err_msg)
 
-    def get_hk_fut_ohlc(self, index, start_date, end_date, freq, rolling_day, rolling_time = 0, rth_only=False):
-        
+    def get_hk_fut_ohlc(self, index, start_date, end_date, freq, rolling_day, rolling_time=0, rth_only=False):
+
         check_bool_dict = self.check_hk_fut_ohlc_args(index, freq, start_date, end_date, rolling_day, rolling_time)
 
         if False not in list(check_bool_dict.values()):
 
             if freq == '1D':
                 rolling_time = 0
                 if rth_only == True:
                     freq = freq + '_rth'
                 elif rth_only == False:
                     freq = freq + '_all'
 
             start_date_dt = datetime.datetime.strptime(str(start_date), '%Y%m%d').date()
             end_date_dt = datetime.datetime.strptime(str(end_date), '%Y%m%d').date()
 
-            start_date_year = start_date_dt.year if start_date_dt.month > 1 else start_date_dt.year - 1
+            if start_date_dt.month > 1:
+                start_date_year = start_date_dt.year
+            else:
+                start_date_year = start_date_dt.year - 1
+                start_date_dt = start_date_dt - relativedelta(months=1)
+
             end_date_year = end_date_dt.year if end_date_dt.month < 11 else end_date_dt.year + 1
-            
+
             holiday_dict = get_hk_holiday_and_expiry_date(start_date_year, end_date_year, 'datetime')
             expiry_date_list = holiday_dict['expiry_date']
 
             expiry_date_dict = {}
             for expiry_date in expiry_date_list:
                 expiry_year_month_str = str(expiry_date.year - 2000) + str(expiry_date.month).zfill(2)
                 expiry_date_dict[expiry_year_month_str] = expiry_date
@@ -238,15 +243,17 @@
                 year_month = i_date.strftime('%y%m')
                 expiry_date = expiry_date_dict[year_month]
                 if i_date > expiry_date:
                     year_month = (i_date + relativedelta(months=1)).strftime('%y%m')
                 if year_month not in year_month_involved_list:
                     year_month_involved_list.append(year_month)
 
-            year_month_involved_list.append((datetime.datetime.strptime(year_month_involved_list[-1], '%y%m') + relativedelta(months=1)).strftime('%y%m'))
+            year_month_involved_list.append(
+                (datetime.datetime.strptime(year_month_involved_list[-1], '%y%m') + relativedelta(months=1)).strftime(
+                    '%y%m'))
             year_month_involved_list_str = json.dumps(str(year_month_involved_list))
 
             year_month_involved_list_str = year_month_involved_list_str.replace('[', '')
             year_month_involved_list_str = year_month_involved_list_str.replace(']', '')
             year_month_involved_list_str = year_month_involved_list_str.replace('\'', '')
             year_month_involved_list_str = year_month_involved_list_str.replace(',', '')
             year_month_involved_list_str = year_month_involved_list_str.replace(' ', '_')
@@ -262,15 +269,14 @@
             rolling_day_str = 'rolling_day=' + str(rolling_day)
             rolling_time_str = 'rolling_time=' + str(rolling_time)
             year_month_involved_list_str = 'year_month_involved_list=' + year_month_involved_list_str
             link_str = link_url + index_str + '&' + freq_str + '&' + rolling_day_str + '&' + rolling_time_str + '&' + year_month_involved_list_str + '&' \
                        + token_str + '&' + database_str + '&' \
                        + start_date_str + '&' + end_date_str
 
-
             response = requests.get(link_str)
             response_ok = response_check(response)
             if response_ok == True:
 
                 result_list = json.loads(json.loads(response.content).replace("'", "\""))
 
                 df_list = []
@@ -287,41 +293,44 @@
                         df = pd.concat(sub_df_list)
                         df = df.reset_index(drop=True)
                         temp_date_list = list(df['date'].unique())
                         temp_date_list.sort()
 
                         date_list = []
                         for temp_date in temp_date_list:
-                            if datetime.datetime.strptime(str(temp_date),'%Y%m%d').weekday() < 5:
+                            if datetime.datetime.strptime(str(temp_date), '%Y%m%d').weekday() < 5:
                                 date_list.append(temp_date)
 
                         front_year_month = str(date_list[0])[2:6]
                         back_year_month = str(date_list[-1])[2:6]
                         front_expiry_date = int(expiry_date_dict[front_year_month].strftime('%Y%m%d'))
                         back_expiry_date = int(expiry_date_dict[back_year_month].strftime('%Y%m%d'))
-
                         for i in range(len(date_list)):
                             date_item = date_list[i]
 
                             if i + rolling_day <= len(date_list) - 1:
+                                print(i, date_list[i + rolling_day], front_expiry_date)
                                 if date_list[i + rolling_day] == front_expiry_date:
                                     front_cut_off_date = date_item
                                 elif date_list[i + rolling_day] == back_expiry_date:
                                     back_cut_off_date = date_item
                                     break
                             else:
                                 back_cut_off_date = max(date_list)
 
-                        if df.loc[0,'expiry_date'] == '20130530':
+                        if df.loc[0, 'expiry_date'] == '20130530':
                             front_cut_off_date = 20130501
 
-                        if (back_cut_off_date != end_date) or (back_cut_off_date == end_date and back_cut_off_date not in expiry_date_list):
+                        if (back_cut_off_date != end_date) or (
+                                back_cut_off_date == end_date and back_cut_off_date not in expiry_date_list):
                             if '1D' not in freq:
-                                df = df[(df['date'] > front_cut_off_date) | ((df['date'] == front_cut_off_date) & (df['time'] >= rolling_time))]
-                                df = df[(df['date'] < back_cut_off_date) | ((df['date'] == back_cut_off_date) & (df['time'] < rolling_time))]
+                                df = df[(df['date'] > front_cut_off_date) | (
+                                            (df['date'] == front_cut_off_date) & (df['time'] >= rolling_time))]
+                                df = df[(df['date'] < back_cut_off_date) | (
+                                            (df['date'] == back_cut_off_date) & (df['time'] < rolling_time))]
                             else:
                                 df = df[(df['date'] > front_cut_off_date) | (df['date'] == front_cut_off_date)]
                                 df = df[(df['date'] < back_cut_off_date) | (df['date'] == back_cut_off_date)]
 
                         df = df[df['date'] >= start_date]
                         df = df[df['date'] <= end_date]
                         df['date'] = df['date'].astype(str)
@@ -350,15 +359,15 @@
                             if len(date_time_intersect) > 0:
                                 date_time_intersect_list.append(date_time_intersect[0])
                             df_list.append(df)
 
                         date_time_list_list += date_time_list
 
                 if '1D' not in freq:
-                    cols = ['datetime', 'date', 'time', 'open', 'high', 'low', 'close', 'volume', 'expiry_date','RTH']
+                    cols = ['datetime', 'date', 'time', 'open', 'high', 'low', 'close', 'volume', 'expiry_date', 'RTH']
                 else:
                     cols = ['datetime', 'date', 'open', 'high', 'low', 'close', 'volume', 'expiry_date']
                 df = pd.concat(df_list)
 
                 if '1D' not in freq:
                     df['datetime'] = pd.to_datetime(df['datetime'], format='%Y%m%d %H%M%S')
                     df['RTH'] = df['RTH'].astype(bool)
@@ -370,34 +379,34 @@
                     drop_index_list = []
                     df = df.reset_index()
                     for date_time_intersect in date_time_intersect_list:
                         check_drop_index_row = df[df['date'] == date_time_intersect]
                         if len(check_drop_index_row) > 1:
                             index_0 = check_drop_index_row.index[0]
                             index_1 = check_drop_index_row.index[1]
-                            expiry_date_0 = df.loc[index_0,'expiry_date']
-                            expiry_date_1 = df.loc[index_1,'expiry_date']
+                            expiry_date_0 = df.loc[index_0, 'expiry_date']
+                            expiry_date_1 = df.loc[index_1, 'expiry_date']
                             if expiry_date_0 > expiry_date_1:
                                 drop_index_list.append(index_0)
                             elif expiry_date_0 < expiry_date_1:
                                 drop_index_list.append(index_1)
                     if len(drop_index_list) > 0:
                         df = df.drop(drop_index_list, axis=0)
                     df = df.drop('index', axis=1)
 
                 df = df.set_index(keys='datetime')
                 df = df.sort_index(ascending=True)
 
                 if '1D' not in freq and rth_only == True:
                     df = df[df['RTH'] == True]
 
-                #df = df.drop_duplicates(keep='last')
+                # df = df.drop_duplicates(keep='last')
 
                 return df
-    
+
         else:
             err_msg = 'Error in: '
             for error in check_bool_dict:
                 if check_bool_dict[error] == False:
                     err_msg += error + ','
             print(err_msg)
 
@@ -1178,29 +1187,30 @@
             df['volume'] = df['volume'].str.replace('.0','', regex=False)
             df['turnover'] = df['turnover'].str.replace('.0','', regex=False)
             df['market_capital'] = df['market_capital'].str.replace('.0','', regex=False)
 
             df = df.sort_values(by='code')
 
             df['market_capital'] = df['market_capital'].astype('int64')
-            df['is_stop_trading'] = df['is_stop_trading'].map({'1': True, '0': False})
+            df['is_stop_trading'] = df['is_stop_trading'].map({'True': True, 'False': False})
+            df = df.rename(columns={'is_stop_trading':'stop_trading'})
 
             float_col_list = ['price','PE','EPS','dividend']
             int_col_list = ['volume','turnover']
             for col in float_col_list:
                 df[col] = df[col].str.replace('-', '', regex=False)
                 df[col] = df[col].str.replace('.000', '', regex=False)
                 df[col] = df[col].str.replace(',', '', regex=False)
                 df[col] = df[col].astype(float)
 
             for col in int_col_list:
                 df[col] = df[col].astype('int64')
             df['lot_size'] = df['lot_size'].astype(int)
 
-            df = df[['code','stock_name','price','PE','EPS','dividend','volume','turnover','share_issued','lot_size','market_capital','ipo_date','year_end_date', 'is_stop_trading','category']]
+            df = df[['code','stock_name','price','PE','EPS','dividend','volume','turnover','share_issued','lot_size','market_capital','ipo_date','year_end_date', 'stop_trading','category']]
             return df
 
     def get_hk_ipo_hist(self):
 
         link_url = 'http://www.hkfdb.net/data_api?'
         token_str = 'token=' + str(self.authToken)
         database_str = 'database=' + 'hk_ipo_hist'
@@ -1423,34 +1433,33 @@
 
             response = requests.get(link_str)
             response_ok = response_check(response)
             if response_ok == True:
 
                 result_list = json.loads(json.loads(response.content).replace("'", "\""))
 
-                columns = ['cbbc_code', 'cbbc_name', 'date', 'num_of_cbbc_bought', 'avg_price_per_cbbc_bought',
-                           'num_of_cbbc_sold', 'avg_price_per_cbbc_sold', 'num_of_cbbc_in_mkt', 'pct_of_issued_in_mkt',
-                           'total_issued_size', 'currency', 'day_high', 'day_low', 'close_price', 'volume', 'turnover',
-                           'issuer', 'underlying', 'bull_bear', 'cbbc_type', 'cbbc_category', 'listing_date',
-                           'last_trading_date', 'maturity_date', 'mce', 'strike_or_call_currency', 'strike_level',
-                           'call_level', 'entitlement_ratio', 'delisting_date']
+                columns = ['unique_id', 'cbbc_code', 'cbbc_name', 'date', 'num_of_cbbc_bought',
+                           'avg_price_per_cbbc_bought',
+                           'num_of_cbbc_sold', 'avg_price_per_cbbc_sold', 'num_of_cbbc_in_mkt', 'total_issued_size',
+                           'currency', 'issuer', 'underlying', 'bull_bear', 'listing_date', 'strike_or_call_currency',
+                           'strike_level', 'call_level', 'entitlement_ratio']
 
                 df_list = []
                 for result in result_list:
                     for item, content in result.items():
                         if type(content) is list:
                             df = pd.DataFrame(content, columns=columns)
-                            df['date'] = df['date'] / 1000000000
-                            df['date'] = pd.to_datetime(df['date'], unit='s')
+                            df['date'] = pd.to_datetime(df['date'], format='%Y%m%d')
+                            df['listing_date'] = pd.to_datetime(df['listing_date'], format='%Y%m%d')
                             df_list.append(df)
 
                 df = pd.concat(df_list)
-                df = df.sort_values('date')
-                df = df.reset_index()
-                df = df.drop('index', axis=1)
+                df = df.sort_values('unique_id')
+                df = df.set_index('unique_id')
+                # df = df.drop('index', axis=1)
 
                 return df
 
         else:
             err_msg = 'Error in: '
             for error in check_bool_dict:
                 if check_bool_dict[error] == False:
```

### Comparing `hkfdb-2.5/hkfdb.egg-info/PKG-INFO` & `hkfdb-2.6/hkfdb.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,74 @@
-Metadata-Version: 2.1
-Name: hkfdb
-Version: 2.5
-Summary: Hong Kong Finance Database.
-Home-page: https://www.hkfdb.net
-Author: Hong Kong Finance Database Team
-Author-email: info@hkfdb.net
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Hong Kong Finance Database
-
-To install the latest version:
-```
-pip install hkfdb
-```
-
-Before you start, please make sure you have done the following:
-* **subscribe** the data from our website
-* get the personal authToken 
-* create an client object from class Database
-* have fun!
-
-create client object with authToken and class Database:
-```
-import hkfdb
-
-authToken = 'personal_authToken'
-client = hkfdb.Database(authToken)
-```
-
-**Major Functions**
-
-Price Data:
-* get_hk_stock_ohlc() 
-* get_us_stock_ohlc()
-* get_hk_fut_ohlc()
-* get_hk_deri_daily_market_report()
-
-CCASS Data:
-* get_ccass_all_id()
-* get_ccass_by_code()
-* get_ccass_holding_rank()
-* get_ccass_by_id()
-* get_ccass_by_id_change()
-
-Index list:
-* get_spx_index_const()
-* get_hk_index_const()
-* get_hk_stock_plate_const()
-* get_all_hk_index_name()
-* get_all_hk_stock_plate_name()
-
-Earning Calendar:
-* get_us_earning_calendar_by_date()
-* get_us_earning_calendar_by_code()
-* get_hk_earning_calendar_by_code()
-* get_hk_earning_calendar_by_date()
-
-Other:
-* get_hk_market_cap_hist()
-* get_hk_ipo_hist()
-* get_north_water()
-* get_market_highlight()
-* get_hk_buyback_by_date()
-* get_hk_buyback_by_code()
-* get_basic_hk_stock_info()
+Metadata-Version: 2.1
+Name: hkfdb
+Version: 2.6
+Summary: Hong Kong Finance Database.
+Home-page: https://www.hkfdb.net
+Author: Hong Kong Finance Database Team
+Author-email: info@hkfdb.net
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Hong Kong Finance Database
+
+To install the latest version:
+```
+pip install hkfdb
+```
+
+Before you start, please make sure you have done the following:
+* **subscribe** the data from our website
+* get the personal authToken 
+* create an client object from class Database
+* have fun!
+
+create client object with authToken and class Database:
+```
+import hkfdb
+
+authToken = 'personal_authToken'
+client = hkfdb.Database(authToken)
+```
+
+**Major Functions**
+
+Price Data:
+* get_hk_stock_ohlc() 
+* get_us_stock_ohlc()
+* get_hk_fut_ohlc()
+* get_hk_deri_daily_market_report()
+
+CCASS Data:
+* get_ccass_all_id()
+* get_ccass_by_code()
+* get_ccass_holding_rank()
+* get_ccass_by_id()
+* get_ccass_by_id_change()
+
+Index list:
+* get_spx_index_const()
+* get_hk_index_const()
+* get_hk_stock_plate_const()
+* get_all_hk_index_name()
+* get_all_hk_stock_plate_name()
+
+Earning Calendar:
+* get_us_earning_calendar_by_date()
+* get_us_earning_calendar_by_code()
+* get_hk_earning_calendar_by_code()
+* get_hk_earning_calendar_by_date()
+
+Other:
+* get_hk_market_cap_hist()
+* get_hk_ipo_hist()
+* get_north_water()
+* get_market_highlight()
+* get_hk_buyback_by_date()
+* get_hk_buyback_by_code()
+* get_basic_hk_stock_info()
+
+
```

### Comparing `hkfdb-2.5/setup.py` & `hkfdb-2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hkfdb",
-    version="2.5",
+    version="2.6",
     author="Hong Kong Finance Database Team",
     author_email="info@hkfdb.net",
     description="Hong Kong Finance Database.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.hkfdb.net",
     packages=setuptools.find_packages(),
```

