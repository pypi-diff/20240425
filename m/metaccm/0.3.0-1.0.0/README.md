# Comparing `tmp/metaccm-0.3.0-py3-none-any.whl.zip` & `tmp/metaccm-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,12 @@
-Zip file size: 5633 bytes, number of entries: 6
+Zip file size: 9977 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-18 10:45 metaccm/__init__.py
--rw-rw-rw-  2.0 fat    12571 b- defN 24-Apr-19 07:06 metaccm/metaccm.py
--rw-rw-rw-  2.0 fat      493 b- defN 24-Apr-19 07:09 metaccm-0.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-19 07:09 metaccm-0.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-19 07:09 metaccm-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      445 b- defN 24-Apr-19 07:09 metaccm-0.3.0.dist-info/RECORD
-6 files, 13609 bytes uncompressed, 4825 bytes compressed:  64.5%
+-rw-rw-rw-  2.0 fat      325 b- defN 24-Apr-25 02:14 metaccm/diffStatistics.py
+-rw-rw-rw-  2.0 fat    12998 b- defN 24-Apr-25 01:59 metaccm/metaccm.py
+-rw-rw-rw-  2.0 fat     4158 b- defN 24-Apr-24 06:25 metaccm/metaccmpro.py
+-rw-rw-rw-  2.0 fat     2335 b- defN 24-Apr-24 02:47 metaccm/weightCalculate.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 24-Apr-25 02:17 metaccm-1.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      573 b- defN 24-Apr-25 02:17 metaccm-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 02:17 metaccm-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-25 02:17 metaccm-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      775 b- defN 24-Apr-25 02:17 metaccm-1.0.0.dist-info/RECORD
+10 files, 22351 bytes uncompressed, 8659 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -1,19 +1,31 @@
 Filename: metaccm/__init__.py
 Comment: 
 
+Filename: metaccm/diffStatistics.py
+Comment: 
+
 Filename: metaccm/metaccm.py
 Comment: 
 
-Filename: metaccm-0.3.0.dist-info/METADATA
+Filename: metaccm/metaccmpro.py
+Comment: 
+
+Filename: metaccm/weightCalculate.py
+Comment: 
+
+Filename: metaccm-1.0.0.dist-info/LICENSE
+Comment: 
+
+Filename: metaccm-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: metaccm-0.3.0.dist-info/WHEEL
+Filename: metaccm-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: metaccm-0.3.0.dist-info/top_level.txt
+Filename: metaccm-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: metaccm-0.3.0.dist-info/RECORD
+Filename: metaccm-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## metaccm/metaccm.py

```diff
@@ -24,46 +24,55 @@
           '\t', '     |         |         | \  / |     ', '\n',
           '\t', '     \         \         |  \/  |     ', '\n',
           '\t', '      \_____    \_____   |      |     ', '\n')
     print('\t', " Meta-CCM 2024-04", '\n')
 
 
 def process_nominal(vector):
+    # 确保数组中的元素为字符串类型
+    vector = vector.astype(str)
+
     return vector
 
 
 def process_scale(vector):
     var_vector = vector.reshape(-1, 1)  # 将向量转换为二维数组
     # 使用最大最小标准化将数值映射到 0-1 之间
     scaler = MinMaxScaler()
     normalized_vector = scaler.fit_transform(var_vector)
     # 将标准化后的向量再转换回一维数组
     normalized_vector = normalized_vector.flatten()
 
+    normalized_vector = normalized_vector.astype(float)
+
     return normalized_vector
 
 
 def process_ordinal(vector):
     var_vector = vector.reshape(-1, 1)  # 将向量转换为二维数组
     # 使用最大最小标准化将数值映射到 0-1 之间
     scaler = MinMaxScaler()
     normalized_vector = scaler.fit_transform(var_vector)
     # 将标准化后的向量再转换回一维数组
     normalized_vector = normalized_vector.flatten()
 
+    normalized_vector = normalized_vector.astype(float)
+
     return normalized_vector
 
 
 def process_binary(vector):
     # 使用 LabelEncoder 将字符串类型转换为数字类型
     label_encoder = LabelEncoder()
     encoded_vector = label_encoder.fit_transform(vector)
     # 将第一个类别映射为 0，第二个类别映射为 1
     normalized_vector = encoded_vector - encoded_vector.min()
 
+    normalized_vector = normalized_vector.astype(int)
+
     return normalized_vector
 
 
 # 定义一个字典，将不同类型的操作关联起来
 process_dict = {
     'nominal': process_nominal,
     'scale': process_scale,
@@ -178,15 +187,15 @@
 # sampleID='sampleID'
 # label='label'
 # matchVars=confoundVars
 # weight=weightVars
 # RequireDiffVar=RequireDiffVar
 
 # help(matchingVars)
-def matchingVars(data: pd.DataFrame, label: str, matchVars: list[str], weight: list[float], RequireDiffVar: list[str]):
+def matchingVars(data: pd.DataFrame, label: str, matchVars: list[str], weight: list[float], RequireDiffVar: list[str] = []):
     """
     This is a function to realize the matching algorithm, which matches positive and negative samples according to
     specific criteria.
     Here’s a breakdown of the steps involved:
 
     1) Initialize the pairID and matchType variables.
     2) Loop through the positive samples (pos_var) until either the positive or negative sample list is empty.
@@ -216,44 +225,48 @@
     negative samples that are different from positive samples. It could be used to ensure diversity in the matched pairs.
     :return: (DataFrame) This function is expected to return a balanced dataset with pairs of positive and negative
     samples that meet the specified criteria. The pairs are matched based on the matching score calculated using the
     matchVars and weights.
     """
 
     logo()
-
+    random.seed(2024)
     # 保存匹配样本对的数据框
     matched_pos = pd.DataFrame() # 阳性样本池
     matched_neg = pd.DataFrame() # 阴性样本池
     pos_var = data[data[label] == 1]
     neg_var = data[data[label] == 0]
     # pos_var = pos_var.reset_index(drop=True)
     # neg_var = neg_var.reset_index(drop=True)
 
     pairID = 0 # 初始化
-    matchType = 'matchingVars'
+    matchType = 'metaccm'
 
     for i in range(len(pos_var)):
         if len(pos_var) == 0 or len(neg_var) == 0:
             break
         # 选择一个阳性样本
         pos_sample = pos_var.sample()
         neg_samples = neg_var.copy()
 
-        # 1) 查看限定条件 RequireDiffVar，选择与阳性样本 RequireDiffVar 不一样的阴性样本
-        for difVar in RequireDiffVar:
-            # print(difVar)
-            # 将 neg_samples[difVar] 和 pos_sample[difVar] 的值转换为集合
-            # neg_set = set(neg_samples[difVar])
-            pos_set = set(pos_sample[difVar])
-            # 找出 neg_samples[difVar] 中不在 pos_sample[difVar] 中的值的位置
-            indices = [j for j, val in enumerate(neg_samples[difVar]) if val not in pos_set]
-            # 根据 indices 列表提取出符合条件的行
-            # iloc方法是根据行的位置（整数位置）来进行选择，而不是根据行的索引（标签）来选择。
-            neg_samples = neg_samples.iloc[indices]
+        if RequireDiffVar == [] or len(RequireDiffVar) == 0 :
+            continue
+        else:
+            # 1) 查看限定条件 RequireDiffVar，选择与阳性样本 RequireDiffVar 不一样的阴性样本
+            for difVar in RequireDiffVar:
+                # print(difVar)
+                # 将 neg_samples[difVar] 和 pos_sample[difVar] 的值转换为集合
+                # neg_set = set(neg_samples[difVar])
+                pos_set = set(pos_sample[difVar])
+                # 找出 neg_samples[difVar] 中不在 pos_sample[difVar] 中的值的位置
+                indices = [j for j, val in enumerate(neg_samples[difVar]) if val not in pos_set]
+                # 根据 indices 列表提取出符合条件的行
+                # iloc方法是根据行的位置（整数位置）来进行选择，而不是根据行的索引（标签）来选择。
+                neg_samples = neg_samples.iloc[indices]
+
         if len(neg_samples) == 0:
             # 没有符合条件的阴性样本，从样本池中移除当前阳性样本
             pos_var = pos_var.drop(pos_sample.index)
             continue
 
         # 2) 在阴性样本中选取与阳性样本 match score 最小（最相近）的样本
         score = matchingScore(neg_samples[matchVars], pos_sample[matchVars], weight)
```

