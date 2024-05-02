# Comparing `tmp/glook-1.1.6b1-py3-none-any.whl.zip` & `tmp/glook-1.1.7b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 55468 bytes, number of entries: 18
+Zip file size: 55038 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat     3200 b- defN 24-Apr-24 16:04 glook/GLook.py
 -rw-rw-rw-  2.0 fat       51 b- defN 24-Mar-25 17:39 glook/__init__.py
 -rw-rw-rw-  2.0 fat      339 b- defN 24-Mar-25 18:24 glook/cli.py
 -rw-rw-rw-  2.0 fat    25002 b- defN 24-Apr-10 10:33 glook/pages/10_Unsupervised_learning.py
 -rw-rw-rw-  2.0 fat    96985 b- defN 24-Apr-27 21:03 glook/pages/11_Custom_Model_Training.py
 -rw-rw-rw-  2.0 fat     6157 b- defN 24-Apr-28 06:49 glook/pages/1_General_Data_Insights.py
--rw-rw-rw-  2.0 fat    19725 b- defN 24-Apr-27 19:10 glook/pages/2_Univariate_Analysis.py
+-rw-rw-rw-  2.0 fat    19800 b- defN 24-Apr-29 17:44 glook/pages/2_Univariate_Analysis.py
 -rw-rw-rw-  2.0 fat     7813 b- defN 24-Apr-24 16:05 glook/pages/3_Bivariate_Analysis.py
 -rw-rw-rw-  2.0 fat     7707 b- defN 24-Apr-28 06:03 glook/pages/4_Trivariate_Analysis.py
--rw-rw-rw-  2.0 fat   112037 b- defN 24-Apr-29 14:17 glook/pages/5_Pre_Processing.py
+-rw-rw-rw-  2.0 fat   111718 b- defN 24-Apr-29 17:46 glook/pages/5_Pre_Processing.py
 -rw-rw-rw-  2.0 fat     3315 b- defN 24-Apr-27 20:41 glook/pages/6_Split_Data.py
 -rw-rw-rw-  2.0 fat     4588 b- defN 24-Apr-11 19:05 glook/pages/7_Dimensionality_Reduction.py
 -rw-rw-rw-  2.0 fat    59951 b- defN 24-Apr-27 20:43 glook/pages/8_Supervised_Learning.py
--rw-rw-rw-  2.0 fat     7241 b- defN 24-Apr-29 14:40 glook-1.1.6b1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 14:40 glook-1.1.6b1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-29 14:40 glook-1.1.6b1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-29 14:40 glook-1.1.6b1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1537 b- defN 24-Apr-29 14:40 glook-1.1.6b1.dist-info/RECORD
-18 files, 355784 bytes uncompressed, 52940 bytes compressed:  85.1%
+-rw-rw-rw-  2.0 fat     7241 b- defN 24-Apr-29 17:51 glook-1.1.7b1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 17:51 glook-1.1.7b1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       38 b- defN 24-Apr-29 17:51 glook-1.1.7b1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-29 17:51 glook-1.1.7b1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1537 b- defN 24-Apr-29 17:51 glook-1.1.7b1.dist-info/RECORD
+18 files, 355540 bytes uncompressed, 52510 bytes compressed:  85.2%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: glook/pages/7_Dimensionality_Reduction.py
 Comment: 
 
 Filename: glook/pages/8_Supervised_Learning.py
 Comment: 
 
-Filename: glook-1.1.6b1.dist-info/METADATA
+Filename: glook-1.1.7b1.dist-info/METADATA
 Comment: 
 
-Filename: glook-1.1.6b1.dist-info/WHEEL
+Filename: glook-1.1.7b1.dist-info/WHEEL
 Comment: 
 
-Filename: glook-1.1.6b1.dist-info/entry_points.txt
+Filename: glook-1.1.7b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: glook-1.1.6b1.dist-info/top_level.txt
+Filename: glook-1.1.7b1.dist-info/top_level.txt
 Comment: 
 
-Filename: glook-1.1.6b1.dist-info/RECORD
+Filename: glook-1.1.7b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## glook/pages/2_Univariate_Analysis.py

```diff
@@ -193,15 +193,15 @@
 		# st.subheader(f"Number of duplicates: :green[{num_duplicates}]")
 		# st.subheader(f"Memory usage: :green[{memory_usage:.1f} KB]")
 		# st.subheader(f"Number of features: :green[{num_features}]")
 		# st.subheader(f"Number of categorical features: :green[{num_categorical}]")
 		# st.subheader(f"Number of numerical features: :green[{num_numerical}]")
 		
 		# Display insights for each column
-		st.title("1️⃣ Univariate Analysis")
+		st.title("1️⃣ Univariate Analysis")                                                                  # PROBLEM
 		# st.header(":green[Column Insights:]⤵️")
 		# html_content = ""
 		for idx, column in enumerate(df.columns):
 			# st.subheader(f':green[**Column {idx + 1}:** {column}]')
 			# subh = f""":green[Column {idx + 1}: {column}]"""
 			# st.subheader(subh)
 			# subh = f"**Column {idx + 1}:** `{column}`"
```

## glook/pages/5_Pre_Processing.py

```diff
@@ -2292,155 +2292,156 @@
 					joblib.dump(pipeline7, f)
 				st.session_state.df = modified_df
 				st.rerun()
 
 	elif preprocessing_action == 'Create Dummy Variables':
 		encoding_method = st.selectbox('Select encoding method', [
 			'One-Hot Encoding', 'Label Encoding'])
-		opt = st.toggle('drop_first')
+		
 		if st.button('Apply', on_click=callback
 			) or st.session_state.button_clicked:
+			opt = st.toggle('drop_first')
 			modified_df = df.copy()
 			modified_df = create_dummy_variables(modified_df, encoding_method, opt)
-			st.write('Modified DataFrame:')
+			# st.write('Modified DataFrame:')                                                   # PROBLEM
 			print(480)
 			st.write(modified_df)
 			print(481)
 			try:
 				print(110000)
 				if modified_df[selected_column].dtype == 'object':
 					print(210000)
-				# 	col1, col2 = st.columns(2)
-				# 	with col1:
-				# 		unique_values = modified_df[selected_column].nunique()
-				# 		st.write(
-				# 			f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
-				# 			)
-				# 		print(482)
-				# 		st.write(
-				# 			f'  - Number of Unique Values: :green[{unique_values}]'
-				# 			)
-				# 		print(483)
-				# 		if unique_values <= 20:
-				# 			st.write(
-				# 				f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]"
-				# 				)
-				# 			print(484)
-				# 		else:
-				# 			st.write(f'  - Top 20 Unique Values:')
-				# 			print(485)
-				# 			st.write(
-				# 				f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]"
-				# 				)
-				# 			print(486)
-				# 	with col2:
-				# 		plt.figure(figsize=(10, 6))
-				# 		print(487)
-				# 		try:
-				# 			sns.countplot(x=limit_unique_values(modified_df
-				# 				[selected_column]), data=modified_df, color
-				# 				='green')
-				# 			print(488)
-				# 		except:
-				# 			sns.countplot(x=modified_df[selected_column],
-				# 				data=modified_df, color='green')
-				# 			print(489)
-				# 		plt.xticks(rotation=45)
-				# 		print(490)
-				# 		st.pyplot()
-				# 		print(491)
-				# 		plt.close()
-				# 		print(492)
-				# 	with st.expander('More Info'):
-				# 		tab1, tab2 = st.tabs(['Insights', 'Donut chart'])
-				# 		with tab1:
-				# 			col7, col8, col9 = st.columns(3)
-				# 			with col7:
-				# 				st.write('## Insights')
-				# 				print(493)
-				# 				approximate_distinct_count = modified_df[
-				# 					selected_column].nunique()
-				# 				approximate_unique_percent = (
-				# 					approximate_distinct_count / len(
-				# 					modified_df) * 100)
-				# 				missing = modified_df[selected_column].isna(
-				# 					).sum()
-				# 				missing_percent = missing / len(modified_df
-				# 					) * 100
-				# 				memory_size = modified_df[selected_column
-				# 					].memory_usage(deep=True)
-				# 				st.write(
-				# 					f'Approximate Distinct Count: :green[{approximate_distinct_count}]'
-				# 					)
-				# 				print(494)
-				# 				st.write(
-				# 					f'Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]'
-				# 					)
-				# 				print(495)
-				# 				st.write(f'Missing: :green[{missing}]')
-				# 				print(496)
-				# 				st.write(
-				# 					f'Missing (%): :green[{missing_percent:.2f}%]'
-				# 					)
-				# 				print(497)
-				# 				st.write(f'Memory Size: :green[{memory_size}]')
-				# 				print(498)
-				# 			with col8:
-				# 				st.write('## Mode')
-				# 				print(499)
-				# 				mode = modified_df[selected_column].mode(
-				# 					).iloc[0]
-				# 				st.write(f'Mode: :green[{mode}]')
-				# 				print(500)
-				# 			with col9:
-				# 				st.write('## First 5 Sample Rows')
-				# 				print(501)
-				# 				st.write(modified_df[selected_column].head())
-				# 				print(502)
-				# 		with tab2:
-				# 			data = limit_unique_values(modified_df[
-				# 				selected_column]).value_counts().reset_index()
-				# 			data.columns = [selected_column, 'count']
-				# 			fig = px.pie(data, values='count', names=
-				# 				selected_column, hole=0.5)
-				# 			fig.update_traces(textposition='inside',
-				# 				textinfo='percent+label')
-				# 			print(503)
-				# 			fig.update_layout(legend=dict(orientation='h',
-				# 				yanchor='bottom', y=1.02, xanchor='right', x=1)
-				# 				)
-				# 			print(504)
-				# 			st.plotly_chart(fig)
-				# 			print(505)
+					col1, col2 = st.columns(2)
+					with col1:
+						unique_values = modified_df[selected_column].nunique()
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+						print(482)
+						st.write(
+							f'  - Number of Unique Values: :green[{unique_values}]'
+							)
+						print(483)
+						if unique_values <= 20:
+							st.write(
+								f"  - Unique Values: :green[{', '.join(map(str, modified_df[selected_column].unique()))}]"
+								)
+							print(484)
+						else:
+							st.write(f'  - Top 20 Unique Values:')
+							print(485)
+							st.write(
+								f":green[{', '.join(map(str, modified_df[selected_column].value_counts().head(20).index))}]"
+								)
+							print(486)
+					with col2:
+						plt.figure(figsize=(10, 6))
+						print(487)
+						try:
+							sns.countplot(x=limit_unique_values(modified_df
+								[selected_column]), data=modified_df, color
+								='green')
+							print(488)
+						except:
+							sns.countplot(x=modified_df[selected_column],
+								data=modified_df, color='green')
+							print(489)
+						plt.xticks(rotation=45)
+						print(490)
+						st.pyplot()
+						print(491)
+						plt.close()
+						print(492)
+					with st.expander('More Info'):
+						tab1, tab2 = st.tabs(['Insights', 'Donut chart'])
+						with tab1:
+							col7, col8, col9 = st.columns(3)
+							with col7:
+								st.write('## Insights')
+								print(493)
+								approximate_distinct_count = modified_df[
+									selected_column].nunique()
+								approximate_unique_percent = (
+									approximate_distinct_count / len(
+									modified_df) * 100)
+								missing = modified_df[selected_column].isna(
+									).sum()
+								missing_percent = missing / len(modified_df
+									) * 100
+								memory_size = modified_df[selected_column
+									].memory_usage(deep=True)
+								st.write(
+									f'Approximate Distinct Count: :green[{approximate_distinct_count}]'
+									)
+								print(494)
+								st.write(
+									f'Approximate Unique (%): :green[{approximate_unique_percent:.2f}%]'
+									)
+								print(495)
+								st.write(f'Missing: :green[{missing}]')
+								print(496)
+								st.write(
+									f'Missing (%): :green[{missing_percent:.2f}%]'
+									)
+								print(497)
+								st.write(f'Memory Size: :green[{memory_size}]')
+								print(498)
+							with col8:
+								st.write('## Mode')
+								print(499)
+								mode = modified_df[selected_column].mode(
+									).iloc[0]
+								st.write(f'Mode: :green[{mode}]')
+								print(500)
+							with col9:
+								st.write('## First 5 Sample Rows')
+								print(501)
+								st.write(modified_df[selected_column].head())
+								print(502)
+						with tab2:
+							data = limit_unique_values(modified_df[
+								selected_column]).value_counts().reset_index()
+							data.columns = [selected_column, 'count']
+							fig = px.pie(data, values='count', names=
+								selected_column, hole=0.5)
+							fig.update_traces(textposition='inside',
+								textinfo='percent+label')
+							print(503)
+							fig.update_layout(legend=dict(orientation='h',
+								yanchor='bottom', y=1.02, xanchor='right', x=1)
+								)
+							print(504)
+							st.plotly_chart(fig)
+							print(505)
 				elif pd.api.types.is_numeric_dtype(modified_df[selected_column]
 					):
 					print(10000)
 					modified_df.to_csv("heha.csv")
 					col3, col4 = st.columns(2)
-				# 	with col3:
-				# 		st.write(
-				# 			f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
-				# 			)
-				# # 		print(506)
-				# 		st.write(
-				# 			f'  - Mean: :green[{modified_df[selected_column].mean()}]'
-				# 			)
-				# 		print(507)
-				# 		st.write(
-				# 			f'  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]'
-				# 			)
-				# 		print(508)
-				# 		st.write(
-				# 			f'  - Min Value: :green[{modified_df[selected_column].min()}]'
-				# 			)
-				# 		print(509)
-				# 		st.write(
-				# 			f'  - Max Value: :green[{modified_df[selected_column].max()}]'
-				# 			)
-				# 		print(510)
+					with col3:
+						st.write(
+							f'  - Data Type: :green[{modified_df[selected_column].dtype}]'
+							)
+				# 		print(506)
+						st.write(
+							f'  - Mean: :green[{modified_df[selected_column].mean()}]'
+							)
+						print(507)
+						st.write(
+							f'  - Standard Deviation: :green[{modified_df[selected_column].std():.3}]'
+							)
+						print(508)
+						st.write(
+							f'  - Min Value: :green[{modified_df[selected_column].min()}]'
+							)
+						print(509)
+						st.write(
+							f'  - Max Value: :green[{modified_df[selected_column].max()}]'
+							)
+						print(510)
 					with col4:
 						plt.figure(figsize=(10, 6))
 						print(511)
 						sns.histplot(modified_df[selected_column], kde=True,
 							color='green')
 						print(512)
 						st.pyplot()
@@ -2448,73 +2449,73 @@
 						plt.close()
 						print(514)
 					with st.expander('More Info'):
 						tab1, tab2, tab3 = st.tabs(['Insights', 'Box plot', 'QQ plot'])
 						with tab1:
 							col4, col5, col6 = st.columns(3)
 							with col4:
-								# st.write('#### Basic Statistics')
+								st.write('#### Basic Statistics')
 								print(515)
-								# insights = calculate_insights(modified_df[selected_column])
-								# basic_stats = {key: value for key, value in
-								# 	insights.items() if key in ['Mean',
-								# 	'Median', 'Mode', 'Standard deviation',
-								# 	'Variance', 'Kurtosis', 'Skewness']}
-								# for key, value in basic_stats.items():
-									# st.write(f'**{key}:** :green[{value:.3f}]')
-									# print(516)
-								# st.write(
-								# 	f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]"
-								# 	)
-								# print(517)
-								# st.write(
-								# 	f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]"
-								# 	)
-								# print(518)
-								# st.write(
-								# 	f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]"
-								# 	)
+								insights = calculate_insights(modified_df[selected_column])
+								basic_stats = {key: value for key, value in
+									insights.items() if key in ['Mean',
+									'Median', 'Mode', 'Standard deviation',
+									'Variance', 'Kurtosis', 'Skewness']}
+								for key, value in basic_stats.items():
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(516)
+								st.write(
+									f"**Memory size:** :green[{insights.get('Memory size', 'N/A'):.3f}]"
+									)
+								print(517)
+								st.write(
+									f"**Range:** :green[{insights.get('Range', 'N/A'):.3f}]"
+									)
+								print(518)
+								st.write(
+									f"**Interquartile range:** :green[{insights.get('Interquartile range', 'N/A'):.3f}]"
+									)
 								print(519)
 							with col5:
 								st.write('#### Percentiles')
 								print(520)
-								# descriptive_stats = insights.get(
-								# 	'Descriptive statistics')
-								# if descriptive_stats is not None:
-								# 	percentiles = descriptive_stats.loc[[
-								# 		'min', '25%', '50%', '75%', 'max']]
-								# 	if '5%' in descriptive_stats.index:
-								# 		percentiles['5%'] = descriptive_stats['5%']
-								# 	if '95%' in descriptive_stats.index:
-								# 		percentiles['95%'] = descriptive_stats[
-								# 			'95%']
-								# 	st.write(percentiles)
-									# print(521)
+								descriptive_stats = insights.get(
+									'Descriptive statistics')
+								if descriptive_stats is not None:
+									percentiles = descriptive_stats.loc[[
+										'min', '25%', '50%', '75%', 'max']]
+									if '5%' in descriptive_stats.index:
+										percentiles['5%'] = descriptive_stats['5%']
+									if '95%' in descriptive_stats.index:
+										percentiles['95%'] = descriptive_stats[
+											'95%']
+									st.write(percentiles)
+									print(521)
 							with col6:
 								st.write('#### Additional Statistics')
-								# print(522)
-								# additional_stats = {key: value for key,
-								# 	value in insights.items() if key in [
-								# 	'Distinct', 'Distinct (%)', 'Missing',
-								# 	'Missing (%)', 'Zeros', 'Zeros (%)',
-								# 	'Negative', 'Negative (%)']}
-								# for key, value in additional_stats.items():
-								# # 	st.write(f'**{key}:** :green[{value:.3f}]')
-									# print(523)
-								# st.write(
-								# 	f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]"
-								# 	)
-								# print(524)
-								# st.write(
-								# 	f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]"
-								# 	)
-								# print(525)
-								# st.write(
-								# 	f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]"
-								# 	)
+								print(522)
+								additional_stats = {key: value for key,
+									value in insights.items() if key in [
+									'Distinct', 'Distinct (%)', 'Missing',
+									'Missing (%)', 'Zeros', 'Zeros (%)',
+									'Negative', 'Negative (%)']}
+								for key, value in additional_stats.items():
+									st.write(f'**{key}:** :green[{value:.3f}]')
+									print(523)
+								st.write(
+									f"**Coefficient of variation (CV):** :green[{insights.get('Coefficient of variation (CV)', 'N/A'):.3f}]"
+									)
+								print(524)
+								st.write(
+									f"**Median Absolute Deviation (MAD):** :green[{insights.get('Median Absolute Deviation (MAD)', 'N/A'):.3f}]"
+									)
+								print(525)
+								st.write(
+									f"**Sum:** :green[{insights.get('Sum', 'N/A'):.3f}]"
+									)
 								print(526)
 						with tab2:
 							fig = px.box(modified_df, y=selected_column)
 							st.plotly_chart(fig)
 							print(527)
 						with tab3:
 							plt.figure(figsize=(10, 6))
@@ -2545,15 +2546,15 @@
 								{'title': 'Theoretical Quantiles',
 								'zeroline': False}, 'yaxis': {'title':
 								'Sample Quantiles'}, 'showlegend': False,
 								'width': 800, 'height': 700})
 							print(532)
 							st.plotly_chart(fig)
 							print(533)
-					st.write('---')
+					# st.write('---')
 					print(534)
 				else:
 					st.write('DataFrame not found.')
 					print(535)
 				st.write('``')
 				print(536)
 			except ZeroDivisionError:
@@ -3381,15 +3382,14 @@
 					"select": select
 				}
 
 				# Save the pipeline to a serialized object
 				with open("column_unique_value_replacement.pkl", "wb") as f:
 					joblib.dump(pipeline12, f)
 				st.session_state.df = modified_df
-				modified_df.to_csv("heha.csv")
 				st.rerun()
 				print(729)
 except Exception as e:
 	print('e:=_', e)
 	print(730)
 	st.error(e)
 	print(731)
```

## Comparing `glook-1.1.6b1.dist-info/METADATA` & `glook-1.1.7b1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glook
-Version: 1.1.6b1
+Version: 1.1.7b1
 Summary: Auto EDA.
 Home-page: https://github.com/gaurang157/glook
 Author: Gaurang Ingle
 Author-email: gaurang.ingle@gmail.com
 Maintainer: Gaurang Ingle, Sharat Chandra Manikonda
 Maintainer-email: manikondasharat@gmail.com
 License: MIT
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: glook Version: 1.1.6b1 Summary: Auto EDA. Home-
+Metadata-Version: 2.1 Name: glook Version: 1.1.7b1 Summary: Auto EDA. Home-
 page: https://github.com/gaurang157/glook Author: Gaurang Ingle Author-email:
 gaurang.ingle@gmail.com Maintainer: Gaurang Ingle, Sharat Chandra Manikonda
 Maintainer-email: manikondasharat@gmail.com License: MIT Project-URL: Bug
 Reports, https://github.com/gaurang157/glook/issues Project-URL: Source, https:
 //github.com/gaurang157/glook Project-URL: Documentation, https://github.com/
 gaurang157/glook/blob/main/README.md Project-URL: Say Thanks!, https://
 github.com/gaurang157/glook/issues/new?assignees=&labels=&template=thanks.yml
```

## Comparing `glook-1.1.6b1.dist-info/RECORD` & `glook-1.1.7b1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 glook/GLook.py,sha256=qNCnTY0f4myhVXkZHf1mMgpN4yfHCaVXq4uz4uC85_s,3200
 glook/__init__.py,sha256=8NahmY4XQHJYMnFDvkZnHpjVBHwxrYrnDFlTTuyXbB0,51
 glook/cli.py,sha256=zBVCZyNNyRj_Zy4Tdnbrb1TrgRhEqAEEdZbk_vrLmi4,339
 glook/pages/10_Unsupervised_learning.py,sha256=_RAtRgR8asoxaIsu-KlITcFlVOV0nRHZl1qWT33OU4k,25002
 glook/pages/11_Custom_Model_Training.py,sha256=4FtzOYYLxySsy7tgV2m6B8IHVaO9KOCVJ1GVHqgmCbs,96985
 glook/pages/1_General_Data_Insights.py,sha256=MTFJNDNfE6k7dBBeWMlN-dfromzX4oKEWWClmSTHc9w,6157
-glook/pages/2_Univariate_Analysis.py,sha256=eGA6zjAwmlMNDIqm1dN-eq_4EVOW1ispoq8BL3o2ypU,19725
+glook/pages/2_Univariate_Analysis.py,sha256=bb_6YzkC7i8WMCmnRQhMlQ6Sci4XVc_HLMP8g2cTXzw,19800
 glook/pages/3_Bivariate_Analysis.py,sha256=_eUSH35csf_Uljg9HvW7szmfXjrgNwrsVJA0gLMDNEA,7813
 glook/pages/4_Trivariate_Analysis.py,sha256=lChxNbGt1nyga-Zf69oL7hUH-z_xLJPq1o0b-pjrtTw,7707
-glook/pages/5_Pre_Processing.py,sha256=usaMfyFrgKcYVK_wfxuTDY7825tyo384matx087qj9I,112037
+glook/pages/5_Pre_Processing.py,sha256=2gW0m8o6QK2H69zOG1FDk0J-wCcrAXrc29HeOgtB5wg,111718
 glook/pages/6_Split_Data.py,sha256=y-3Qo16H5vZeADRxKR8oSs8PViSm89O-iCstK-YPhSs,3315
 glook/pages/7_Dimensionality_Reduction.py,sha256=Eq9Et3k7Q-MsS7e5EYiI6P4Vat5P9VBTCziM6KdidIo,4588
 glook/pages/8_Supervised_Learning.py,sha256=Bg3qK4w8RRfWhpMzaYeTwPgfzeBO4PgO7rkgB9wzuCQ,59951
-glook-1.1.6b1.dist-info/METADATA,sha256=TFhxkNQ-fJfx1Hckvn9CfGmziX843Xw_3070bab1u_8,7241
-glook-1.1.6b1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-glook-1.1.6b1.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
-glook-1.1.6b1.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
-glook-1.1.6b1.dist-info/RECORD,,
+glook-1.1.7b1.dist-info/METADATA,sha256=F5RMMxomhJm53mW0szIxqsm9IlEnOvAUd8wB8Z0OWDc,7241
+glook-1.1.7b1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+glook-1.1.7b1.dist-info/entry_points.txt,sha256=7q8WVzTgIl4vX4wJgctmfdJckoB5yPtI0p3hqAQSiFA,38
+glook-1.1.7b1.dist-info/top_level.txt,sha256=2wtpfrIqw9VT_LFDxpI77DArLrUaNjWxyClToM3P9WE,6
+glook-1.1.7b1.dist-info/RECORD,,
```

