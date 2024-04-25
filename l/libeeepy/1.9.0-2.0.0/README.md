# Comparing `tmp/libeeepy-1.9.0-py3-none-any.whl.zip` & `tmp/libeeepy-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 12175 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      114 b- defN 22-Jan-06 01:45 libeeepy/__init__.py
--rw-rw-rw-  2.0 fat    53726 b- defN 22-Jan-06 01:43 libeeepy/calculateaccuracy.py
--rw-rw-rw-  2.0 fat     6448 b- defN 21-Dec-30 03:41 libeeepy/dataprocessing.py
--rw-rw-rw-  2.0 fat     5054 b- defN 21-Dec-30 03:41 libeeepy/operatemysql.py
--rw-rw-rw-  2.0 fat      465 b- defN 22-Jan-06 01:46 libeeepy-1.9.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 22-Jan-06 01:46 libeeepy-1.9.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 22-Jan-06 01:46 libeeepy-1.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      627 b- defN 22-Jan-06 01:46 libeeepy-1.9.0.dist-info/RECORD
-8 files, 66540 bytes uncompressed, 11083 bytes compressed:  83.3%
+Zip file size: 16073 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      114 b- defN 24-Apr-25 06:40 libeeepy/__init__.py
+-rw-rw-rw-  2.0 fat   111845 b- defN 23-Dec-04 05:54 libeeepy/calculateaccuracy.py
+-rw-rw-rw-  2.0 fat     6448 b- defN 22-May-17 03:45 libeeepy/dataprocessing.py
+-rw-rw-rw-  2.0 fat     5054 b- defN 22-May-17 03:45 libeeepy/operatemysql.py
+-rw-rw-rw-  2.0 fat      464 b- defN 24-Apr-25 06:43 libeeepy-2.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-25 06:43 libeeepy-2.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-25 06:42 libeeepy-2.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      628 b- defN 24-Apr-25 06:43 libeeepy-2.0.0.dist-info/RECORD
+8 files, 124654 bytes uncompressed, 14981 bytes compressed:  88.0%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: libeeepy/dataprocessing.py
 Comment: 
 
 Filename: libeeepy/operatemysql.py
 Comment: 
 
-Filename: libeeepy-1.9.0.dist-info/METADATA
+Filename: libeeepy-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: libeeepy-1.9.0.dist-info/WHEEL
+Filename: libeeepy-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: libeeepy-1.9.0.dist-info/top_level.txt
+Filename: libeeepy-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: libeeepy-1.9.0.dist-info/RECORD
+Filename: libeeepy-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libeeepy/__init__.py

```diff
@@ -1,4 +1,4 @@
 from .operatemysql import *
 from .dataprocessing import *
 from .calculateaccuracy import *
-__version__ = "v1.9.0"
+__version__ = "v2.0.0"
```

## libeeepy/calculateaccuracy.py

```diff
@@ -6,52 +6,88 @@
             |calculate_MSE：          计算 MSE
             |calculate_harmonic:      计算调和平均准确率
             |calculate_huabei:        计算华北短期准确率
             |calculate_huazhong_wind: 计算华中风电短期准确率
             |calculate_huazhong_solar:计算华中光伏短期准确率
             |calculate_sichuan_wind:  计算四川风电短期准确率
             |calculate_sichuan_solar: 计算四川光伏短期准确率
+            |calculate_nanfang_wind_2022: 计算南网2022版风电短期准确率 乔锋 2023年5月31日
+            |calculate_nanfang_solar_2022: 计算南网2022版光伏短期准确率 乔锋 2023年5月31日
             |calculate_nanfang_wind:  计算南方风电短期准确率
             |calculate_nanfang_solar: 计算南方光伏短期准确率
             |calculate_shanxi_wind:   计算山西风电短期准确率
             |calculate_shanxi_solar:  计算山西光伏短期准确率
             |calculate_shandong_wind: 计算山东风电短期准确率
             |calculate_shandong_solar:计算山东光伏短期准确率
             |calculate_fujian_wind:   计算福建风电短期准确率
             |calculate_anhui_wind:    计算安徽风电短期准确率
             |calculate_anhui_solar:   计算安徽光伏短期准确率
-            |calculate_zhejiang_wind: 计算浙江风电短期准确率
-            |calculate_zhejiang_solar:计算浙江光伏短期准确率
+            |calculate_zhejiang_wind: 计算浙江风电短期准确率  2022年3月18日
+            |calculate_zhejiang_solar:计算浙江光伏短期准确率  2022年3月18日
             |calculate_dongbei_wind:  计算东北风电短期准确率
             |calculate_dongbei_solar: 计算东北光伏短期准确率
             |calculate_shanxi_2021_wind: 计算山西2021版风电短期准确率
             |calculate_shanxi_2021_solar: 计算山西2021版光伏短期准确率
+            |calculate_xibei_wind_2022: 计算陕西2022版风电短期准确率
+            |calculate_xibei_solar_2022: 计算陕西2022版光伏短期准确率
+            |calculate_xinjiang_wind_2022: 计算新疆2022版风电短期准确率
+            |calculate_xinjiang_solar_2022: 计算新疆2022版风电短期准确率
+            |calculate_xibei_wind_2023: 计算陕西2023版风电短期准确率
+            |calculate_xibei_solar_2023: 计算陕西2023版光伏短期准确率
+            |calculate_xinjiang_wind_2023: 计算新疆2023版风电短期准确率
+            |calculate_xinjiang_solar_2023: 计算新疆2023版风电短期准确率
+            |calculate_harmonic_2023:      计算2023版调和平均准确率
+
+
             --------------------------------------
-@ author:   sun-shu-bei
+@ author:   sun-shu-bei song-mei-yang
 @ date:     2020-07-22
-@ vision：  v1.6.0
+@ update:   2023-05-31
+@ vision：  v1.11.0
 @ update:
             1. 时间格式处兼容性      sun-shu-bei  2017-11-13
             2. 日mse时间格式排序     sun-shu-bei  2017-11-13
             3. pandas列名显示问题   sun-shu-bei  2017-11-15
             4. 简化时间格式         sun-shu-bei  2018-01-04
             5. 添加调和平均准确率    sun-shu-bei  2018-01-31
             6. 添加合格率计算        zhang-qi     2018-03-29
             7. 增加Python3版本的支持 sun-shu-bei  2020-07-22
             8. 修改调和平均数        song-mei-yang 2020-12-11
             9. 增加华北、华中、南方、东北、山西、山东、福建、安徽、浙江、四川
             等各省两个细则函数       song-mei-yang 2020-12-11
             10 增加山西2021版双细则考核函数 song-mei-yang 2021-12-09
+            11 根据均方根误差计算不达标天数时将原标准20% 改为 15% song-mei-yang 2022-01-17
+            12 新增西北区域柔性考核  song-mei-yang 2022-03-10
+            13 浙江两个细则 数据预处理 bug修复 song-mei-yang 2022-03-18
+            14 新增南方电网2022版风光两个细则计算规则 qiaofeng 2023-05-31
+            15 新增西北电网2023版风光两个细则计算规则 song-mei-yang 2023-12-01
+
  """
 import numpy
 import datetime
 import pandas
 import calendar
 
 
+
+def check(date_time=None,power_real=None,power_forecast=None):
+    if len(str(date_time))==19:
+        return str(date_time)
+    else:
+        print(date_time)
+    if str(power_real).isdigit():
+        return float(power_real)
+    else:
+        print(power_real)
+    if str(power_forecast).isdigit:
+        return float(power_forecast)
+    else:
+        print(power_forecast)
+
+
 class CalculateAccuracy:
 
     def __init__(self, date_time, power_real, power_forecast, capacity):
 
         self.date_time = date_time
         self.power_real = power_real
         self.power_forecast = power_forecast
@@ -118,15 +154,15 @@
 
         for b_loop in range(len(error_day)):
             bd = datetime.datetime.strptime(error_day[b_loop], '%Y-%m-%d')
             yy_mm = bd.strftime('%Y-%m')
             ym_list.append(yy_mm)
             error_list.append(error_value[b_loop])
 
-            if error_value[b_loop] > 20:
+            if error_value[b_loop] > 15:
                 count_day.append(1)
             else:
                 count_day.append(0)
 
         df_month = pandas.DataFrame({'date': ym_list, 'MSE': error_list, 'day_mark': count_day})
         MSE = df_month['MSE'].groupby(df_month['date']).mean()
         off_grade = df_month['day_mark'].groupby(df_month['date']).sum()
@@ -166,14 +202,83 @@
         harmonic_score = numpy.where(harmonic < 0.75, 100 * (0.75 - harmonic) * self.capacity * 0.015 * 0.1, 0)
         date_ymd = harmonic.index
         # 输出成DataFrame格式
         df_score = pandas.DataFrame({'date': date_ymd, 'day_harmonic': numpy.array(harmonic), 'day_pen_score': numpy.array(harmonic_score)})
 
         return df_score
 
+    def calculate_harmonic_2023(self):
+        '''
+        输入为实际功率及第*小时超短期预测功率 输入numpy.array格式
+        输出为DataFrame格式的第*小时重点时刻调和平均数准确率 + 其它时刻调和平均数准确率
+        由于输入第*小时不确定 故暂不输出对应的考核分数
+
+        2023年11月08日西北能监局关于印发西北区域两个细则 附件1并网运行管理实施细则 
+        超短期预测曲线第1、2、3、4小时调和平均数准确率
+        风电第1小时80% 第2小时75% 第3小时70% 第4小时65%
+        光伏第1小时85% 第2小时80% 第3小时75% 第4小时70%
+        
+        重点时段为：用电高峰时段 + 新能源大发时段  
+        重点时段每减少1%按照全场装机容量*0.0015分/万千瓦
+        其它时段每减少1%按照全场装机容量*0.0003分/万千瓦
+        西北（除新疆外）新能源大发时段为 10:00-16:00
+        西北（除新疆外）用  电高峰时段为 06:00-09:00  17:00-22:00
+
+        新疆新能源大发时段为: 11:00-17:00
+        新疆用  电高峰时段为: 07:00-10:00  18:00-23:00
+        FBI WARNING : 
+            pr和pf均在装机容量的3%以为时 该点不计入误差计算
+            确保输入超短期第*小时预测数据
+            返回的超短期第*小时准确率
+    
+        '''
+        # 创建DataFrame
+        # df_score = pandas.DataFrame([], columns=['date','harmonic', 'harmonic_score'])
+        df_data = pandas.DataFrame([],columns=['time', 'power_real', 'power_forecast'])
+        df_data['time'] = self.date_time
+        df_data['power_real'] = self.power_real
+        df_data['power_forecast'] = self.power_forecast
+        # 计算调和平均准确率
+        dfs_time = df_data['time']
+        power_real = df_data['power_real']
+        power_forecast = df_data['power_forecast']
+        ymd = dfs_time.str[0:10]  # 选取 yyyy-mm-dd
+        df_hour = dfs_time.str[11:16] # 选取 hh-mm
+        # 实际和预测均在装机容量的3%以内时 不计入误差计算
+        n_index = numpy.where(numpy.logical_or(power_real >= self.capacity * 0.03, power_forecast >= self.capacity * 0.03))
+        power_real = power_real[n_index[0]]
+        power_forecast = power_forecast[n_index[0]]
+        ymd = ymd[n_index[0]]
+        df_hour = df_hour[n_index[0]]
+
+        df_clean = pandas.DataFrame([],columns=['ymd','hour', 'power_real', 'power_forecast'])
+        df_clean['ymd'] = ymd
+        df_clean['hour'] = df_hour
+        df_clean['power_real'] = power_real
+        df_clean['power_forecast'] = power_forecast
+
+        # 高峰时段计算调和平均数准确率
+
+
+        bias_item = abs((power_real / (power_real + power_forecast)) - 0.5)  # 偏差项计算
+        abs_error = abs(power_real - power_forecast)  # 实际功率与预测功率之差
+        multi_item = bias_item * abs_error
+        sum_item = multi_item.groupby(ymd).sum()
+        sum_error = abs_error.groupby(ymd).sum()  # 96个点的差值求和计算
+        harmonic = 1 - 2 * sum_item / sum_error
+        harmonic_score = numpy.where(harmonic < 0.75, 100 * (0.75 - harmonic) * self.capacity * 0.015 * 0.1, 0)
+        date_ymd = harmonic.index
+        # 输出成DataFrame格式
+        df_score = pandas.DataFrame({'date': date_ymd, 'day_harmonic': numpy.array(harmonic), 'day_pen_score': numpy.array(harmonic_score)})
+
+        return df_score
+
+
+
+
     def calculate_huabei(self):
         '''
             北京、天津、河北、冀北、内蒙古两个细则考核 输入numpy.array格式
             返回每日短期准确率
             返回每日短期考核电量
             FBI WARING :   
                 准确率公式多适用于冀北 冀南风光项目
@@ -417,48 +522,151 @@
         penalty_mwh = numpy.array(penalty_mwh)  # 转为数组
 
         # 转DataFrame格式
         df_penalty = pandas.DataFrame({'date': date_ymd,'day_acc': 1-mae, 'day_pen_mwh': penalty_mwh})
 
         return df_penalty
 
+    def calculate_nanfang_wind_2022(self):
+        '''
+        按照国家能源局南方监管局 南方能监市场2022第91号文 （适用对象广东、广西、云南、贵州、海南、深圳）
+        南网考核1+7系统计算规则要求：当预测功率、可用功率、实际功率均小于装机10%，不纳入准确率计算；
+        注：1+7考核系统不纳入计算后导致准确率比纳入计算的准确率更低
+        rmse/pmi        pmi ≥ 0.2Cap
+        rmse/cap*0.2    pmi < 0.2Cap
+
+        input：
+            日期、实际功率、预测准确率、装机容量
+        return：
+            日期、准确率、考核电量
+        准确率计算及考核要求：
+            同一时刻，实际功率、预测功率都低于装机容量的10%的数据会被剔除，不参与准确率计算
+            当准确率计算结果小于0时，准确率按0执行
+            短期考核电量==（60%-准确率）* cap * 0.2
+            实际执行规则为 不使用(不足一个百分点的按一个百分点计)此规则,准确率直接相减计算
+        '''
+        df_nanfang_wind = pandas.DataFrame([], columns=['time', 'power_real', 'power_forecast'])
+        df_nanfang_wind['time'] = self.date_time
+        df_nanfang_wind['power_real'] = self.power_real
+        df_nanfang_wind['power_forecast'] = self.power_forecast
+        cap = self.capacity
+
+        dfs_time = df_nanfang_wind['time']
+        pr = df_nanfang_wind['power_real']
+        pf = df_nanfang_wind['power_forecast']
+        ymd = dfs_time.astype(str).str[0:10]
+
+        popstand = 0.1 * cap
+        # 预测功率小于0.1倍装机阈值时 等于0.1倍装机 ；此行不在用于指标计算中
+        # df_nanfang_wind['power_forecast'] = numpy.where(df_nanfang_wind['power_forecast'] < popstand, popstand,
+        #                                               df_nanfang_wind['power_forecast'])
+        df_nanfang_wind['popdata'] = numpy.where(
+            (df_nanfang_wind['power_real'] < popstand) & (df_nanfang_wind['power_forecast'] < popstand), 0, 1)
+        df_nanfang_wind = df_nanfang_wind[df_nanfang_wind['popdata'] == 1]
+        df_nanfang_wind['fm'] = df_nanfang_wind['power_real'].apply(lambda x: x if x > 0.2 * cap else 0.2 * cap)
+        fm = df_nanfang_wind['fm']
+
+        dfs_time = df_nanfang_wind['time']
+        pr = df_nanfang_wind['power_real']
+        pf = df_nanfang_wind['power_forecast']
+
+        error = abs(pr - pf)
+        offset = (error / fm) ** 2
+        acc = 1 - numpy.sqrt(offset.groupby(ymd).mean())
+        date_ymd=acc.index
+        acc = numpy.array(numpy.where(acc < 0, 0, acc))
+        penalty_mwh = numpy.array(numpy.where(acc < 0.6, (0.6 - acc) * cap * 0.2, 0))
+        df_penalty = pandas.DataFrame(
+            {'date': date_ymd, 'day_acc': acc, 'day_pen_mwh': penalty_mwh})
+
+        return df_penalty
+
+    def calculate_nanfang_solar_2022(self):
+        '''
+        按照国家能源局南方监管局 南方能监市场2022第91号文 （适用对象广东、广西、云南、贵州、海南、深圳）
+        南网考核1+7系统计算规则要求：当预测功率、可用功率、实际功率均小于装机10%，不纳入准确率计算；
+        注：1+7考核系统不纳入计算后导致准确率比纳入计算的准确率更低
+        rmse/pmi        pmi ≥ 0.2Cap
+        rmse/cap*0.2    pmi < 0.2Cap
+        
+        input：
+            日期、实际功率、预测准确率、装机容量
+        return：
+            日期、准确率、考核电量
+        准确率计算及考核要求：
+            同一时刻，实际功率、预测功率都低于装机容量的10%的数据会被剔除，不参与准确率计算
+            当准确率计算结果小于0时，准确率按0执行
+            短期考核电量==（65%-准确率）* cap
+            实际执行规则为 不使用(不足一个百分点的按一个百分点计)此规则,准确率直接相减计算
+        '''
+        df_nanfang_solar = pandas.DataFrame([], columns=['time', 'power_real', 'power_forecast'])
+        df_nanfang_solar['time'] = self.date_time
+        df_nanfang_solar['power_real'] = self.power_real
+        df_nanfang_solar['power_forecast'] = self.power_forecast
+        cap = self.capacity
+
+        dfs_time = df_nanfang_solar['time']
+        pr = df_nanfang_solar['power_real']
+        pf = df_nanfang_solar['power_forecast']
+        ymd = dfs_time.astype(str).str[0:10]  # 选取 yyyy-mm-dd
+
+        popstand = 0.1 * cap
+        df_nanfang_solar['popdata'] = numpy.where((df_nanfang_solar['power_real'] < popstand) & (df_nanfang_solar['power_forecast'] < popstand), 0, 1)
+        df_nanfang_solar = df_nanfang_solar[df_nanfang_solar['popdata'] == 1]
+        df_nanfang_solar['fm'] = df_nanfang_solar['power_real'].apply(lambda x: x if x > 0.2 * cap else 0.2 * cap)
+        fm = df_nanfang_solar['fm']
+
+
+        error = abs(pr - pf)
+        offset = (error / fm) ** 2
+        acc = 1 - numpy.sqrt(offset.groupby(ymd).mean())
+        date_ymd = acc.index
+        acc = numpy.array(numpy.where(acc < 0, 0, acc))
+        penalty_mwh = numpy.array(numpy.where(acc < 0.65, (0.65 - acc) * cap, 0))
+        df_penalty = pandas.DataFrame(
+            {'date': date_ymd, 'day_acc': acc, 'day_pen_mwh': penalty_mwh})
+
+        return df_penalty
+
     def calculate_nanfang_wind(self):
         '''
         南方两个细则考核 输入numpy.array格式
         适用于装机30MW以上风电项目（云南、贵州、广东、广西、海南、深圳）
         返回每日短期准确率 即 (1-rmse) 
         返回每日短期考核电量（MWH)
         '''
+
         df_nanfang_wind = pandas.DataFrame([], columns=['time', 'power_real', 'power_forecast'])
         df_nanfang_wind['time'] = self.date_time
         df_nanfang_wind['power_real'] = self.power_real
         df_nanfang_wind['power_forecast'] = self.power_forecast
         cap = self.capacity
 
         dfs_time = df_nanfang_wind['time']
         pr = df_nanfang_wind['power_real']
         pf = df_nanfang_wind['power_forecast']
-        ymd = dfs_time.str[0:10]  # 选取 yyyy-mm-dd
+        ymd = dfs_time.astype(str).str[0:10]
+
 
         # 计算均方根误差
         pr = numpy.where(pr < 0, 0, pr)  # 实际功率小于零时归零
         error = (pr - pf) * (pr - pf)  # （实际功率-预测功率）
         mse = error.groupby(ymd).mean()  # 标准差计算
         rmse = numpy.sqrt(mse) / float(cap)  # 均方根误差计算
-
         date_ymd = rmse.index
-        rmse = numpy.array(rmse)  # 转为数组
 
-        penalty_mwh = numpy.where(rmse > 0.25, (rmse - 0.25) * cap * 1, 0)  # 均方根误差考核分数计算
-        penalty_mwh = numpy.array(penalty_mwh)  # 转为数组
 
+        rmse = numpy.array(rmse)  # 转为数组
+        penalty_mwh = numpy.where(rmse > 0.2, (rmse - 0.2) * cap * 1, 0)  # 均方根误差考核分数计算
+        penalty_mwh = numpy.array(penalty_mwh)  # 转为数组
         # 转DataFrame格式
         df_penalty = pandas.DataFrame(
             {'date': date_ymd, 'day_acc': 1 - rmse, 'day_pen_mwh': penalty_mwh})
 
+
         return df_penalty
 
     def calculate_nanfang_solar(self):
         '''
         南方两个细则考核 输入numpy.array格式
         适用于装机30MW以上风电项目（云南、贵州、广东、广西、海南、深圳）
         返回每日短期准确率 即 (1-rmse) 
@@ -469,28 +677,27 @@
         df_nanfang_solar['power_real'] = self.power_real
         df_nanfang_solar['power_forecast'] = self.power_forecast
         cap = self.capacity
 
         dfs_time = df_nanfang_solar['time']
         pr = df_nanfang_solar['power_real']
         pf = df_nanfang_solar['power_forecast']
-        ymd = dfs_time.str[0:10]  # 选取 yyyy-mm-dd
+        ymd = dfs_time.astype(str).str[0:10]  # 选取 yyyy-mm-dd
 
         # 计算均方根误差
         pr = numpy.where(pr < 0, 0, pr)  # 实际功率小于零时归零
         error = (pr - pf) * (pr - pf)  # （实际功率-预测功率）
         mse = error.groupby(ymd).mean()  # 标准差计算
         rmse = numpy.sqrt(mse) / float(cap)  # 均方根误差计算
 
         date_ymd = rmse.index
         rmse = numpy.array(rmse)  # 转为数组
 
         penalty_mwh = numpy.where(rmse > 0.15, (rmse - 0.15) * cap * 1, 0)  # 均方根误差考核分数计算
         penalty_mwh = numpy.array(penalty_mwh)  # 转为数组
-
         # 转DataFrame格式
         df_penalty = pandas.DataFrame(
             {'date': date_ymd, 'day_acc': 1 - rmse, 'day_pen_mwh': penalty_mwh})
 
         return df_penalty
 
     def calculate_shanxi_wind(self):
@@ -764,14 +971,16 @@
         '''
         浙江风电两个细则考核 输入numpy.array格式
         适用于浙江风电项目
         由于准确率公式分母为实际功率（需考虑分母为零的异常情况）；
             需对实际功率数据预处理
             实际功率为零 预测功率为零 偏差率为0
             实际功率为零 预测功率不为零 偏差率为100%
+                2022年3月18日
+                实际功率不为零，预测功率不为零，偏差率大于100% 该时间点的偏差率为100%
             准确率小于零 归为零
         返回每日短期准确率 (1-rmse)、每日短期考核电量
         '''
         df_zhejiang = pandas.DataFrame([], columns=['time', 'power_real', 'power_forecast'])
         df_zhejiang['time'] = self.date_time
         df_zhejiang['power_real'] = self.power_real
         df_zhejiang['power_forecast'] = self.power_forecast
@@ -787,15 +996,17 @@
             (df_zhejiang['power_real'] == 0.0) & (df_zhejiang['power_forecast'] != 0.0), ['deviation']] = -99.0
         df_zhejiang['error'] = -99
         df_zhejiang.loc[(df_zhejiang['deviation'] == -99.0), ['error']] = 1.0  # 实际为零 预测非零时 偏差率为1
         df_zhejiang.loc[(df_zhejiang['deviation'] == 0.0), ['error']] = 0.0    # 实际为零 预测为零时 偏差率为0
         pr_pf_nonzero = df_zhejiang.loc[(df_zhejiang['deviation'] > 0.0), 'deviation']
         pr_nonzero = df_zhejiang.loc[(df_zhejiang['deviation'] > 0.0), 'power_real']
         df_zhejiang.loc[(df_zhejiang['deviation'] > 0.0), 'error'] = (pr_pf_nonzero/pr_nonzero) * (pr_pf_nonzero/pr_nonzero)
-
+        # 实际功率不为零 预测功率不为零 如果此时偏差率大于100%时 则偏差率为100%
+        df_zhejiang.loc[(df_zhejiang['error'] > 1), 'error'] = 1
+        # 计算标准差
         mse = df_zhejiang.error.groupby(ymd).mean()  # 标准差计算
         rmse = numpy.sqrt(mse)  # 均方根误差计算
         acc = 1 - rmse
         acc = acc.where(acc > 0,0)  # 准确率小于零 归为零；DataFrame.where cond is True, keep the original value
 
         #  DataFrame 转 array
         date_ymd = acc.index    # 每天准确率
@@ -812,14 +1023,16 @@
 
         浙江光伏两个细则考核 输入numpy.array格式
         适用于浙江光伏项目
         由于准确率公式分母为实际功率（需考虑分母为零的异常情况）；
             需对实际功率数据预处理
             实际功率为零 预测功率为零 偏差率为0
             实际功率为零 预测功率不为零 偏差率为100%
+            2022年3月18日
+                实际功率不为零，预测功率不为零，偏差率大于100% 该时间点的偏差率为100%
             准确率小于零 归为零
         返回每日短期准确率 (1-rmse)、每日短期考核电量
 
         '''
         df_zhejiang = pandas.DataFrame([], columns=['time', 'power_real', 'power_forecast'])
         df_zhejiang['time'] = self.date_time
         df_zhejiang['power_real'] = self.power_real
@@ -836,15 +1049,16 @@
             (df_zhejiang['power_real'] == 0.0) & (df_zhejiang['power_forecast'] != 0.0), ['deviation']] = -99.0
         df_zhejiang['error'] = -99
         df_zhejiang.loc[(df_zhejiang['deviation'] == -99.0), ['error']] = 1.0  # 实际为零 预测非零时 偏差率为1
         df_zhejiang.loc[(df_zhejiang['deviation'] == 0.0), ['error']] = 0.0    # 实际为零 预测非零时 偏差率为0
         pr_pf_nonzero = df_zhejiang.loc[(df_zhejiang['deviation'] > 0.0), 'deviation']
         pr_nonzero = df_zhejiang.loc[(df_zhejiang['deviation'] > 0.0), 'power_real']
         df_zhejiang.loc[(df_zhejiang['deviation'] > 0.0), 'error'] = (pr_pf_nonzero/pr_nonzero) * (pr_pf_nonzero/pr_nonzero)
-
+        # 实际功率不为零 预测功率不为零 如果此时偏差率大于100%时 则偏差率为100%
+        df_zhejiang.loc[(df_zhejiang['error'] > 1), 'error'] = 1
         mse = df_zhejiang.error.groupby(ymd).mean()  # 标准差计算
         rmse = numpy.sqrt(mse)  # 均方根误差计算
         acc = 1 - rmse
         acc = acc.where(acc > 0,0)  # 准确率小于零 归为零；DataFrame.where cond is True, keep the original value
 
         #  DataFrame 转 array
         date_ymd = acc.index    # 每天准确率
@@ -904,15 +1118,15 @@
         ym_pass = numpy.array(ym_pass)  # 转为数组
         # 计算月考核分
         penalty_acc_score = numpy.where(ym_acc < 0.75, (0.75 - ym_acc) * cap , 0)  # 每降低一个百分点，每10万千瓦扣1分
         penalty_pass_score = numpy.where(ym_pass < 0.8, (0.8 - ym_pass) * cap, 0)  # 每降低一个百分点，每10万千瓦扣1分
         df_month_penalty = pandas.DataFrame({'date': date_ym,'month_acc': ym_acc,'month_pass':ym_pass,
                                              'month_pen_acc':penalty_acc_score,'month_pen_pass':penalty_pass_score})
 
-        return df_month_penalty
+        return df_day_penalty,df_month_penalty
 
     def calculate_dongbei_solar(self):
         '''
         东北两个细则考核 输入numpy.array格式
         适用于光伏项目（蒙东、黑龙江、吉林、辽宁）
         返回每月短期准确率（调度要求月均大于85%）、每月合格率（调度要求月均大于80%）
         返回每月短期考核分、每月合格率考核分
@@ -959,15 +1173,15 @@
         ym_pass = numpy.array(ym_pass)  # 转为数组
         # 计算月考核分
         penalty_acc_score = numpy.where(ym_acc < 0.85, (0.85 - ym_acc) * cap, 0)  # 每降低一个百分点，每10万千瓦扣1分
         penalty_pass_score = numpy.where(ym_pass < 0.8, (0.8 - ym_pass) * cap, 0)  # 每降低一个百分点，每10万千瓦扣1分
         df_month_penalty = pandas.DataFrame({'date': date_ym, 'month_acc': ym_acc, 'month_pass': ym_pass,
                                              'month_pen_acc': penalty_acc_score, 'month_pen_pass': penalty_pass_score})
 
-        return df_month_penalty
+        return df_day_penalty, df_month_penalty
     
     def calculate_qualification(self):
         '''
         计算合格率
         '''
         len_loop = len(self.date_time)
         ymd_list = []
@@ -1166,8 +1380,855 @@
                 temp_pen = 0
             pen_new.append(temp_pen)
 
         df_penalty = pandas.DataFrame({'date': ymd_new, 'day_acc': acc_new, 'day_pen_mwh': pen_new, 'max_ae': ae_new, 'max_ae_pen_mwh': ae_pen_new})
 
         return df_penalty
 
+    def calculate_xibei_wind_2022(self):
+        '''
+
+        2021年12月22日西北能监局发布修订完善西北区域两个细则
+        适用风 风电预测曲线最大误差不超过25%
+        西北（除新疆外）新能源大发时段为 10:00-16:00
+        西北（除新疆外）用  电高峰时段为 06:00-09:00  17:00-22:00
+
+        新疆新能源大发时段为：11:00-17:00
+        新疆用  电高峰时段为：07:00-10:00  18:00-23:00
+
+        返回每日短期偏差积分电量
+        FBI WARING
+        '''
+        df_xibei = pandas.DataFrame([], columns=['time', 'power_real', 'power_forecast'])
+        df_xibei['time'] = self.date_time
+        df_xibei['power_real'] = self.power_real
+        df_xibei['power_forecast'] = self.power_forecast
+        df_xibei = df_xibei[df_xibei['power_real'] >= 0]
+        df_xibei = df_xibei[df_xibei['power_forecast'] >= 0]
+        series_time = df_xibei['time']
+        df_xibei['hour'] = series_time.str[11:16]
+        if len(df_xibei) > 0:
+            # 取列
+            dfs_time = df_xibei['time']
+            power_real = df_xibei['power_real']
+            power_forecast = df_xibei['power_forecast']
+            ymd = dfs_time.str[0:10]  # 选取 yyyy-mm-dd
+            df_hour = dfs_time.str[11:16]  # pandas series
+            cap = self.capacity
+            TSD = 0.25  # 风电日预测曲线最大误差0.25 ; 光伏日预测曲线最大误差0.2
+            # 特殊条件下
+            n_index1 = numpy.where(
+                numpy.logical_and(power_forecast == 0, power_real > cap * 0.03))
+            n_index2 = numpy.where(
+                numpy.logical_and(power_forecast == 0, power_real <= cap * 0.03))
+            n_index3 = numpy.where(
+                numpy.logical_and(power_forecast > cap * 0.03, power_real == 0))
+            n_index4 = numpy.where(
+                numpy.logical_and(power_forecast <= cap * 0.03, power_real == 0))
+            numpy.seterr(divide='ignore', invalid='ignore')
+            # 满足特殊条件
+            error_deviation = numpy.where(power_forecast > 0, (power_real - power_forecast) / power_forecast, 0)
+            error_deviation[n_index1[0]] = 1
+            error_deviation[n_index2[0]] = 0
+            error_deviation[n_index3[0]] = 1
+            error_deviation[n_index4[0]] = 0
+
+            # 偏差积分电量 计算时考虑了允许偏差25%，偏差变成26%就考核1% ；参考 TSD = |(pr-pf)/pf| ==> |pr-pf| = TSD*pf
+            power_deviation = numpy.where(
+                abs(error_deviation) > TSD,
+                abs(power_real - power_forecast) / 40 - power_forecast / 40 * TSD,
+                0)
+            # 2022西北新细则要求，新能源大发时段风电的偏差大于25%时 or 用电高峰时段的偏差时
+            df_xibei['error_deviation'] = error_deviation
+            df_xibei['power_deviation'] = power_deviation
+            df_xibei['score_deviation'] = power_deviation
+            for index, row in df_xibei.iterrows():
+                # 新能源大发时段
+                if '10:00' <= row.hour <= '16:00':
+                    if row.error_deviation > TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.4
+                    elif row.error_deviation < -TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.2
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0
+                # 新能源用电高峰时段
+                elif '06:00' <= row.hour <= '09:00' or '17:00' <= row.hour <= '22:00' :
+                    if row.error_deviation > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.2
+                    elif row.error_deviation < -TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.4
+                else:
+                    if abs(row.error_deviation) > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.2
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = 0
+
+        score_deviation = df_xibei['score_deviation']
+        power_deviation = df_xibei['power_deviation']
+        # date_month = pandas.Series(list(map(time2split_month, date_time)))
+        # date_day = pandas.Series(list(map(time2split_day, date_time)))
+        date_month = df_xibei['time'].str[0:7]
+        date_day = df_xibei['time'].str[0:10]
+        deviation_score = score_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        ym_list = []
+        ymd_list = []
+        for name, group in score_deviation.groupby(date_day):
+            bd = datetime.datetime.strptime(name, '%Y-%m-%d')
+            yy_mm_dd = bd.strftime('%Y-%m-%d')
+            ymd_list.append(yy_mm_dd)
+        day_penalties = pandas.DataFrame(
+            numpy.c_[ymd_list, deviation_power, deviation_score],
+            columns=['date', 'Deviation_energy', 'Deviation_score'])
+        deviation_score = score_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        ym_list = []
+        for name, group in score_deviation.groupby(date_month):
+            bd = datetime.datetime.strptime(name, '%Y-%m')
+            yy_mm = bd.strftime('%Y-%m')
+            ym_list.append(yy_mm)
+        month_penalties = pandas.DataFrame(
+            numpy.c_[ym_list, deviation_power, deviation_score],
+            columns=['month', 'Deviation_energy', 'Deviation_score'])
+
+        return day_penalties, month_penalties
+
+
+    def calculate_xibei_wind_2023(self):
+        '''
+
+        2023年11月08日西北能监局关于印发西北区域两个细则 附件1并网运行管理实施细则 
+
+        适用风 风电预测曲线最大误差不超过25%
+        西北（除新疆外）新能源大发时段为 10:00-16:00
+        西北（除新疆外）用  电高峰时段为 06:00-09:00  17:00-22:00
+
+        新疆新能源大发时段为: 11:00-17:00
+        新疆用  电高峰时段为: 07:00-10:00  18:00-23:00
+
+        返回每日短期偏差积分电量
+        FBI WARING
+        '''
+        df_xibei = pandas.DataFrame([], columns=['time', 'power_real', 'power_forecast'])
+        df_xibei['time'] = self.date_time
+        df_xibei['power_real'] = self.power_real
+        df_xibei['power_forecast'] = self.power_forecast
+        # 实际功率在[-5,cap] 都纳入计算
+        df_xibei = df_xibei[df_xibei['power_real'] >= -5]
+        df_xibei = df_xibei[df_xibei['power_forecast'] >= 0]
+        series_time = df_xibei['time']
+        df_xibei['hour'] = series_time.str[11:16]
+        if len(df_xibei) > 0:
+            # 取列
+            dfs_time = df_xibei['time']
+            power_real = df_xibei['power_real']
+            power_forecast = df_xibei['power_forecast']
+            ymd = dfs_time.str[0:10]  # 选取 yyyy-mm-dd
+            df_hour = dfs_time.str[11:16]  # pandas series
+            cap = self.capacity
+            TSD = 0.25  # 风电日预测曲线最大误差0.25 ; 光伏日预测曲线最大误差0.2
+            # 当实际功率和预测功率均在装机容量的3%以内 不予考核
+            n_index1 = numpy.where(
+                numpy.logical_and(power_forecast <= cap * 0.03, power_real <= cap * 0.03))
+            numpy.seterr(divide='ignore', invalid='ignore')
+            # 分母必须是abs(pr) 由于power_real存在[-3MW,0]的情况，故此时的E偏差为负值
+            error_deviation = numpy.where(power_real > -5, (power_real - power_forecast) / abs(power_real), 0)
+            error_deviation[n_index1[0]] = 0
+
+            # 偏差积分电量 计算时考虑了允许偏差25%，偏差变成26%就考核1% ；参考 TSD = |(pr-pf)/pr| ==> |pr-pf| = TSD*pr
+            power_deviation = numpy.where(
+                abs(error_deviation) > TSD,
+                abs(power_real - power_forecast) / 40 - power_real / 40 * TSD,
+                0)
+            # 2023西北新细则要求，新能源大发时段风电的偏差大于25%时 or 用电高峰时段的偏差时
+            df_xibei['error_deviation'] = error_deviation
+            df_xibei['power_deviation'] = power_deviation
+            df_xibei['score_deviation'] = power_deviation
+            for index, row in df_xibei.iterrows():
+                # 新能源大发时段
+                if '10:00' <= row.hour <= '16:00':
+                    if row.error_deviation > TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.1
+                    elif row.error_deviation < -TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.05
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0
+                # 用电高峰时段
+                elif '06:00' <= row.hour <= '09:00' or '17:00' <= row.hour <= '22:00' :
+                    if row.error_deviation > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.05
+                    elif row.error_deviation < -TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.15
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0
+                else:
+                    if abs(row.error_deviation) > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.05
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = 0
+
+        score_deviation = df_xibei['score_deviation']
+        power_deviation = df_xibei['power_deviation']
+        # date_month = pandas.Series(list(map(time2split_month, date_time)))
+        # date_day = pandas.Series(list(map(time2split_day, date_time)))
+        date_month = df_xibei['time'].str[0:7]
+        date_day = df_xibei['time'].str[0:10]
+        deviation_score = score_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        ym_list = []
+        ymd_list = []
+        for name, group in score_deviation.groupby(date_day):
+            bd = datetime.datetime.strptime(name, '%Y-%m-%d')
+            yy_mm_dd = bd.strftime('%Y-%m-%d')
+            ymd_list.append(yy_mm_dd)
+        day_penalties = pandas.DataFrame(
+            numpy.c_[ymd_list, deviation_power, deviation_score],
+            columns=['date', 'Deviation_energy', 'Deviation_score'])
+        deviation_score = score_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        ym_list = []
+        for name, group in score_deviation.groupby(date_month):
+            bd = datetime.datetime.strptime(name, '%Y-%m')
+            yy_mm = bd.strftime('%Y-%m')
+            ym_list.append(yy_mm)
+        month_penalties = pandas.DataFrame(
+            numpy.c_[ym_list, deviation_power, deviation_score],
+            columns=['month', 'Deviation_energy', 'Deviation_score'])
+
+        return day_penalties, month_penalties
+
+
+    def calculate_xinjiang_wind_2023(self):
+        '''
+
+        2023年11月08日西北能监局关于印发西北区域两个细则 附件1并网运行管理实施细则 
+
+        适用风 风电预测曲线最大误差不超过25%
+        西北（除新疆外）新能源大发时段为 10:00-16:00
+        西北（除新疆外）用  电高峰时段为 06:00-09:00  17:00-22:00
+
+        新疆新能源大发时段为: 11:00-17:00
+        新疆用  电高峰时段为: 07:00-10:00  18:00-23:00
+
+        返回每日短期偏差积分电量
+        FBI WARING
+        '''
+        df_xibei = pandas.DataFrame([], columns=['time', 'power_real', 'power_forecast'])
+        df_xibei['time'] = self.date_time
+        df_xibei['power_real'] = self.power_real
+        df_xibei['power_forecast'] = self.power_forecast
+        # 实际功率在[-5,cap] 都纳入计算
+        df_xibei = df_xibei[df_xibei['power_real'] >= -5]
+        df_xibei = df_xibei[df_xibei['power_forecast'] >= 0]
+        series_time = df_xibei['time']
+        df_xibei['hour'] = series_time.str[11:16]
+        if len(df_xibei) > 0:
+            # 取列
+            dfs_time = df_xibei['time']
+            power_real = df_xibei['power_real']
+            power_forecast = df_xibei['power_forecast']
+            ymd = dfs_time.str[0:10]  # 选取 yyyy-mm-dd
+            df_hour = dfs_time.str[11:16]  # pandas series
+            cap = self.capacity
+            TSD = 0.25  # 风电日预测曲线最大误差0.25 ; 光伏日预测曲线最大误差0.2
+            # 当实际功率和预测功率均在装机容量的3%以内 不予考核
+            n_index1 = numpy.where(
+                numpy.logical_and(power_forecast <= cap * 0.03, power_real <= cap * 0.03))
+            numpy.seterr(divide='ignore', invalid='ignore')
+            # 分母必须是abs(pr) 由于power_real存在[-3MW,0]的情况，故此时的E偏差为负值
+            error_deviation = numpy.where(power_real > -5, (power_real - power_forecast) / abs(power_real), 0)
+            error_deviation[n_index1[0]] = 0
+
+            # 偏差积分电量 计算时考虑了允许偏差25%，偏差变成26%就考核1% ；参考 TSD = |(pr-pf)/pr| ==> |pr-pf| = TSD*pr
+            power_deviation = numpy.where(
+                abs(error_deviation) > TSD,
+                abs(power_real - power_forecast) / 40 - power_real / 40 * TSD,
+                0)
+            # 2023西北新细则要求，新能源大发时段风电的偏差大于25%时 or 用电高峰时段的偏差时
+            df_xibei['error_deviation'] = error_deviation
+            df_xibei['power_deviation'] = power_deviation
+            df_xibei['score_deviation'] = power_deviation
+            for index, row in df_xibei.iterrows():
+                # 新能源大发时段
+                if '11:00' <= row.hour <= '17:00':
+                    if row.error_deviation > TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.1
+                    elif row.error_deviation < -TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.05
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0
+                # 用电高峰时段
+                elif '07:00' <= row.hour <= '10:00' or '18:00' <= row.hour <= '23:00' :
+                    if row.error_deviation > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.05
+                    elif row.error_deviation < -TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.15
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0
+                else:
+                    if abs(row.error_deviation) > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.05
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = 0
+
+        score_deviation = df_xibei['score_deviation']
+        power_deviation = df_xibei['power_deviation']
+        # date_month = pandas.Series(list(map(time2split_month, date_time)))
+        # date_day = pandas.Series(list(map(time2split_day, date_time)))
+        date_month = df_xibei['time'].str[0:7]
+        date_day = df_xibei['time'].str[0:10]
+        deviation_score = score_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        ym_list = []
+        ymd_list = []
+        for name, group in score_deviation.groupby(date_day):
+            bd = datetime.datetime.strptime(name, '%Y-%m-%d')
+            yy_mm_dd = bd.strftime('%Y-%m-%d')
+            ymd_list.append(yy_mm_dd)
+        day_penalties = pandas.DataFrame(
+            numpy.c_[ymd_list, deviation_power, deviation_score],
+            columns=['date', 'Deviation_energy', 'Deviation_score'])
+        deviation_score = score_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        ym_list = []
+        for name, group in score_deviation.groupby(date_month):
+            bd = datetime.datetime.strptime(name, '%Y-%m')
+            yy_mm = bd.strftime('%Y-%m')
+            ym_list.append(yy_mm)
+        month_penalties = pandas.DataFrame(
+            numpy.c_[ym_list, deviation_power, deviation_score],
+            columns=['month', 'Deviation_energy', 'Deviation_score'])
+
+        return day_penalties, month_penalties
+
+
+    def calculate_xibei_solar_2023(self):
+        '''
+
+        2023年11月08日西北能监局关于印发西北区域两个细则 附件1并网运行管理实施细则 
+        适用光伏预测曲线最大误差不超过20%
+        西北（除新疆外）新能源大发时段为 10:00-16:00
+        西北（除新疆外）用  电高峰时段为 06:00-09:00  17:00-22:00
+
+        新疆新能源大发时段为:11:00-17:00
+        新疆用  电高峰时段为:07:00-10:00  18:00-23:00
+
+        返回每日短期偏差积分电量
+        FBI WARING
+        '''
+        df_xibei = pandas.DataFrame([], columns=['time', 'power_real', 'power_forecast'])
+        df_xibei['time'] = self.date_time
+        df_xibei['power_real'] = self.power_real
+        df_xibei['power_forecast'] = self.power_forecast
+        # 实际功率在[-5,cap] 都纳入计算
+        df_xibei = df_xibei[df_xibei['power_real'] >= -5]
+        df_xibei = df_xibei[df_xibei['power_forecast'] >= 0]
+        series_time = df_xibei['time']
+        df_xibei['hour'] = series_time.str[11:16]
+        if len(df_xibei) > 0:
+            # 取列
+            dfs_time = df_xibei['time']
+            power_real = df_xibei['power_real']
+            power_forecast = df_xibei['power_forecast']
+            ymd = dfs_time.str[0:10]  # 选取 yyyy-mm-dd
+            df_hour = dfs_time.str[11:16]  # pandas series
+            cap = self.capacity
+            TSD = 0.2  # 风电日预测曲线最大误差0.25 ; 光伏日预测曲线最大误差0.2
+            # 当实际功率和预测功率均在装机容量的3%以内 不予考核
+            n_index1 = numpy.where(
+                numpy.logical_and(power_forecast <= cap * 0.03, power_real <= cap * 0.03))
+            numpy.seterr(divide='ignore', invalid='ignore')
+            # 分母必须是abs(pr) 由于power_real存在[-3MW,0]的情况，故此时的E偏差为负值
+            error_deviation = numpy.where(power_real > -5, (power_real - power_forecast) / abs(power_real), 0)
+            error_deviation[n_index1[0]] = 0
+            numpy.seterr(divide='ignore', invalid='ignore')
+            # 偏差积分电量 计算时考虑了允许偏差25%，偏差变成26%就考核1% ；参考 TSD = |(pr-pf)/pr| ==> |pr-pf| = TSD*pr
+            power_deviation = numpy.where(
+                abs(error_deviation) > TSD,
+                abs(power_real - power_forecast) / 40 - power_real / 40 * TSD,
+                0)
+            # 2023西北新细则要求，新能源大发时段风电的偏差大于25%时 or 用电高峰时段的偏差时
+            df_xibei['error_deviation'] = error_deviation
+            df_xibei['power_deviation'] = power_deviation
+            df_xibei['score_deviation'] = power_deviation
+            for index, row in df_xibei.iterrows():
+                # 新能源大发时段
+                if '10:00' <= row.hour <= '16:00':
+                    if row.error_deviation > TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.1
+                    elif row.error_deviation < -TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.05
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0
+                # 用电高峰时段
+                elif '06:00' <= row.hour <= '09:00' or '17:00' <= row.hour <= '22:00' :
+                    if row.error_deviation > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.05
+                    elif row.error_deviation < -TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.15
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0    
+                else:
+                    if abs(row.error_deviation) > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.05
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = 0
+
+        score_deviation = df_xibei['score_deviation']
+        power_deviation = df_xibei['power_deviation']
+        # date_month = pandas.Series(list(map(time2split_month, date_time)))
+        # date_day = pandas.Series(list(map(time2split_day, date_time)))
+        date_month = df_xibei['time'].str[0:7]
+        date_day = df_xibei['time'].str[0:10]
+        deviation_score = score_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        ym_list = []
+        ymd_list = []
+        for name, group in score_deviation.groupby(date_day):
+            bd = datetime.datetime.strptime(name, '%Y-%m-%d')
+            yy_mm_dd = bd.strftime('%Y-%m-%d')
+            ymd_list.append(yy_mm_dd)
+        day_penalties = pandas.DataFrame(
+            numpy.c_[ymd_list, deviation_power, deviation_score],
+            columns=['date', 'Deviation_energy', 'Deviation_score'])
+        deviation_score = score_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        ym_list = []
+        for name, group in score_deviation.groupby(date_month):
+            bd = datetime.datetime.strptime(name, '%Y-%m')
+            yy_mm = bd.strftime('%Y-%m')
+            ym_list.append(yy_mm)
+        month_penalties = pandas.DataFrame(
+            numpy.c_[ym_list, deviation_power, deviation_score],
+            columns=['month', 'Deviation_energy', 'Deviation_score'])
+
+        return day_penalties, month_penalties
+
+
+    def calculate_xinjiang_solar_2023(self):
+        '''
+
+        2023年11月08日西北能监局关于印发西北区域两个细则 附件1并网运行管理实施细则 
+        适用光伏预测曲线最大误差不超过20%
+        西北（除新疆外）新能源大发时段为 10:00-16:00
+        西北（除新疆外）用  电高峰时段为 06:00-09:00  17:00-22:00
+
+        新疆新能源大发时段为:11:00-17:00
+        新疆用  电高峰时段为:07:00-10:00  18:00-23:00
+
+        返回每日短期偏差积分电量
+        FBI WARING
+        '''
+        df_xibei = pandas.DataFrame([], columns=['time', 'power_real', 'power_forecast'])
+        df_xibei['time'] = self.date_time
+        df_xibei['power_real'] = self.power_real
+        df_xibei['power_forecast'] = self.power_forecast
+        # 实际功率在[-5,cap] 都纳入计算
+        df_xibei = df_xibei[df_xibei['power_real'] >= -5]
+        df_xibei = df_xibei[df_xibei['power_forecast'] >= 0]
+        series_time = df_xibei['time']
+        df_xibei['hour'] = series_time.str[11:16]
+        if len(df_xibei) > 0:
+            # 取列
+            dfs_time = df_xibei['time']
+            power_real = df_xibei['power_real']
+            power_forecast = df_xibei['power_forecast']
+            ymd = dfs_time.str[0:10]  # 选取 yyyy-mm-dd
+            df_hour = dfs_time.str[11:16]  # pandas series
+            cap = self.capacity
+            TSD = 0.2  # 风电日预测曲线最大误差0.25 ; 光伏日预测曲线最大误差0.2
+            # 当实际功率和预测功率均在装机容量的3%以内 不予考核
+            n_index1 = numpy.where(
+                numpy.logical_and(power_forecast <= cap * 0.03, power_real <= cap * 0.03))
+            numpy.seterr(divide='ignore', invalid='ignore')
+            # 分母必须是abs(pr) 由于power_real存在[-3MW,0]的情况，故此时的E偏差为负值
+            error_deviation = numpy.where(power_real > -5, (power_real - power_forecast) / abs(power_real), 0)
+            error_deviation[n_index1[0]] = 0
+            numpy.seterr(divide='ignore', invalid='ignore')
+            # 偏差积分电量 计算时考虑了允许偏差25%，偏差变成26%就考核1% ；参考 TSD = |(pr-pf)/pr| ==> |pr-pf| = TSD*pr
+            power_deviation = numpy.where(
+                abs(error_deviation) > TSD,
+                abs(power_real - power_forecast) / 40 - power_real / 40 * TSD,
+                0)
+            # 2023西北新细则要求，新能源大发时段风电的偏差大于25%时 or 用电高峰时段的偏差时
+            df_xibei['error_deviation'] = error_deviation
+            df_xibei['power_deviation'] = power_deviation
+            df_xibei['score_deviation'] = power_deviation
+            for index, row in df_xibei.iterrows():
+                # 新能源大发时段
+                if '11:00' <= row.hour <= '17:00':
+                    if row.error_deviation > TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.1
+                    elif row.error_deviation < -TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.05
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0
+                # 用电高峰时段
+                elif '07:00' <= row.hour <= '10:00' or '18:00' <= row.hour <= '23:00' :
+                    if row.error_deviation > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.05
+                    elif row.error_deviation < -TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.15
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0    
+                else:
+                    if abs(row.error_deviation) > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.05
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = 0
+
+        score_deviation = df_xibei['score_deviation']
+        power_deviation = df_xibei['power_deviation']
+        # date_month = pandas.Series(list(map(time2split_month, date_time)))
+        # date_day = pandas.Series(list(map(time2split_day, date_time)))
+        date_month = df_xibei['time'].str[0:7]
+        date_day = df_xibei['time'].str[0:10]
+        deviation_score = score_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        ym_list = []
+        ymd_list = []
+        for name, group in score_deviation.groupby(date_day):
+            bd = datetime.datetime.strptime(name, '%Y-%m-%d')
+            yy_mm_dd = bd.strftime('%Y-%m-%d')
+            ymd_list.append(yy_mm_dd)
+        day_penalties = pandas.DataFrame(
+            numpy.c_[ymd_list, deviation_power, deviation_score],
+            columns=['date', 'Deviation_energy', 'Deviation_score'])
+        deviation_score = score_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        ym_list = []
+        for name, group in score_deviation.groupby(date_month):
+            bd = datetime.datetime.strptime(name, '%Y-%m')
+            yy_mm = bd.strftime('%Y-%m')
+            ym_list.append(yy_mm)
+        month_penalties = pandas.DataFrame(
+            numpy.c_[ym_list, deviation_power, deviation_score],
+            columns=['month', 'Deviation_energy', 'Deviation_score'])
+
+        return day_penalties, month_penalties
+
+
+    def calculate_xibei_solar_2022(self):
+        '''
+
+        2021年12月22日西北能监局发布修订完善西北区域两个细则
+        适用光伏预测曲线最大误差不超过20%
+        西北（除新疆外）新能源大发时段为 10:00-16:00
+        西北（除新疆外）用  电高峰时段为 06:00-09:00  17:00-22:00
+
+        新疆新能源大发时段为：11:00-17:00
+        新疆用  电高峰时段为：07:00-10:00  18:00-23:00
+
+        返回每日短期偏差积分电量
+        FBI WARING
+        '''
+        df_xibei = pandas.DataFrame([], columns=['time', 'power_real', 'power_forecast'])
+        df_xibei['time'] = self.date_time
+        df_xibei['power_real'] = self.power_real
+        df_xibei['power_forecast'] = self.power_forecast
+        df_xibei = df_xibei[df_xibei['power_real'] >= 0]
+        df_xibei = df_xibei[df_xibei['power_forecast'] >= 0]
+        series_time = df_xibei['time']
+        df_xibei['hour'] = series_time.str[11:16]
+        if len(df_xibei) > 0:
+            # 取列
+            dfs_time = df_xibei['time']
+            power_real = df_xibei['power_real']
+            power_forecast = df_xibei['power_forecast']
+            ymd = dfs_time.str[0:10]  # 选取 yyyy-mm-dd
+            df_hour = dfs_time.str[11:16]  # pandas series
+            cap = self.capacity
+            TSD = 0.2  # 风电日预测曲线最大误差0.25 ; 光伏日预测曲线最大误差0.2
+            # 特殊条件下
+            n_index1 = numpy.where(
+                numpy.logical_and(power_forecast == 0, power_real > cap * 0.03))
+            n_index2 = numpy.where(
+                numpy.logical_and(power_forecast == 0, power_real <= cap * 0.03))
+            n_index3 = numpy.where(
+                numpy.logical_and(power_forecast > cap * 0.03, power_real == 0))
+            n_index4 = numpy.where(
+                numpy.logical_and(power_forecast <= cap * 0.03, power_real == 0))
+            numpy.seterr(divide='ignore', invalid='ignore')
+            # 满足特殊条件
+            error_deviation = numpy.where(power_forecast > 0, (power_real - power_forecast) / power_forecast, 0)
+            error_deviation[n_index1[0]] = 1
+            error_deviation[n_index2[0]] = 0
+            error_deviation[n_index3[0]] = 1
+            error_deviation[n_index4[0]] = 0
+
+            # 偏差积分电量 计算时考虑了允许偏差25%，偏差变成26%就考核1% ；参考 TSD = |(pr-pf)/pf| ==> |pr-pf| = TSD*pf
+            power_deviation = numpy.where(
+                abs(error_deviation) > TSD,
+                abs(power_real - power_forecast) / 40 - power_forecast / 40 * TSD,
+                0)
+            # 2022西北新细则要求，新能源大发时段风电的偏差大于25%时 or 用电高峰时段的偏差时
+            df_xibei['error_deviation'] = error_deviation
+            df_xibei['power_deviation'] = power_deviation
+            df_xibei['score_deviation'] = power_deviation
+            for index, row in df_xibei.iterrows():
+                # 新能源大发时段
+                if '10:00' <= row.hour <= '16:00':
+                    if row.error_deviation > TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.4
+                    elif row.error_deviation < -TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.2
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0
+                # 新能源用电高峰时段
+                elif '06:00' <= row.hour <= '09:00' or '17:00' <= row.hour <= '22:00' :
+                    if row.error_deviation > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.2
+                    elif row.error_deviation < -TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.4
+                else:
+                    if abs(row.error_deviation) > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.2
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = 0
+
+        score_deviation = df_xibei['score_deviation']
+        power_deviation = df_xibei['power_deviation']
+        # date_month = pandas.Series(list(map(time2split_month, date_time)))
+        # date_day = pandas.Series(list(map(time2split_day, date_time)))
+        date_month = df_xibei['time'].str[0:7]
+        date_day = df_xibei['time'].str[0:10]
+        deviation_score = score_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        ym_list = []
+        ymd_list = []
+        for name, group in score_deviation.groupby(date_day):
+            bd = datetime.datetime.strptime(name, '%Y-%m-%d')
+            yy_mm_dd = bd.strftime('%Y-%m-%d')
+            ymd_list.append(yy_mm_dd)
+        day_penalties = pandas.DataFrame(
+            numpy.c_[ymd_list, deviation_power, deviation_score],
+            columns=['date', 'Deviation_energy', 'Deviation_score'])
+        deviation_score = score_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        ym_list = []
+        for name, group in score_deviation.groupby(date_month):
+            bd = datetime.datetime.strptime(name, '%Y-%m')
+            yy_mm = bd.strftime('%Y-%m')
+            ym_list.append(yy_mm)
+        month_penalties = pandas.DataFrame(
+            numpy.c_[ym_list, deviation_power, deviation_score],
+            columns=['month', 'Deviation_energy', 'Deviation_score'])
+
+        return day_penalties, month_penalties
+
+
+    def calculate_xinjiang_wind_2022(self):
+        '''
+
+        2021年12月22日西北能监局发布修订完善西北区域两个细则
+        适用风 风电预测曲线最大误差不超过25%
+        西北（除新疆外）新能源大发时段为 10:00-16:00
+        西北（除新疆外）用  电高峰时段为 06:00-09:00  17:00-22:00
+
+        新疆新能源大发时段为：11:00-17:00
+        新疆用  电高峰时段为：07:00-10:00  18:00-23:00
+
+        返回每日短期偏差积分电量
+        FBI WARING
+        '''
+        df_xibei = pandas.DataFrame([], columns=['time', 'power_real', 'power_forecast'])
+        df_xibei['time'] = self.date_time
+        df_xibei['power_real'] = self.power_real
+        df_xibei['power_forecast'] = self.power_forecast
+        df_xibei = df_xibei[df_xibei['power_real'] >= 0]
+        df_xibei = df_xibei[df_xibei['power_forecast'] >= 0]
+        series_time = df_xibei['time']
+        df_xibei['hour'] = series_time.str[11:16]
+        if len(df_xibei) > 0:
+            # 取列
+            dfs_time = df_xibei['time']
+            power_real = df_xibei['power_real']
+            power_forecast = df_xibei['power_forecast']
+            ymd = dfs_time.str[0:10]  # 选取 yyyy-mm-dd
+            df_hour = dfs_time.str[11:16]  # pandas series
+            cap = self.capacity
+            TSD = 0.25  # 风电日预测曲线最大误差0.25 ; 光伏日预测曲线最大误差0.2
+            # 特殊条件下
+            n_index1 = numpy.where(
+                numpy.logical_and(power_forecast == 0, power_real > cap * 0.03))
+            n_index2 = numpy.where(
+                numpy.logical_and(power_forecast == 0, power_real <= cap * 0.03))
+            n_index3 = numpy.where(
+                numpy.logical_and(power_forecast > cap * 0.03, power_real == 0))
+            n_index4 = numpy.where(
+                numpy.logical_and(power_forecast <= cap * 0.03, power_real == 0))
+            numpy.seterr(divide='ignore', invalid='ignore')
+            # 满足特殊条件
+            error_deviation = numpy.where(power_forecast > 0, (power_real - power_forecast) / power_forecast, 0)
+            error_deviation[n_index1[0]] = 1
+            error_deviation[n_index2[0]] = 0
+            error_deviation[n_index3[0]] = 1
+            error_deviation[n_index4[0]] = 0
+
+            # 偏差积分电量 计算时考虑了允许偏差25%，偏差变成26%就考核1% ；参考 TSD = |(pr-pf)/pf| ==> |pr-pf| = TSD*pf
+            power_deviation = numpy.where(
+                abs(error_deviation) > TSD,
+                abs(power_real - power_forecast) / 40 - power_forecast / 40 * TSD,
+                0)
+            # 2022西北新细则要求，新能源大发时段风电的偏差大于25%时 or 用电高峰时段的偏差时
+            df_xibei['error_deviation'] = error_deviation
+            df_xibei['power_deviation'] = power_deviation
+            df_xibei['score_deviation'] = power_deviation
+            for index, row in df_xibei.iterrows():
+                # 新能源大发时段
+                if '11:00' <= row.hour <= '17:00':
+                    if row.error_deviation > TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.4
+                    elif row.error_deviation < -TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.2
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0
+                # 新能源用电高峰时段
+                elif '07:00' <= row.hour <= '10:00' or '18:00' <= row.hour <= '23:00' :
+                    if row.error_deviation > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.2
+                    elif row.error_deviation < -TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.4
+                else:
+                    if abs(row.error_deviation) > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.2
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = 0
+
+        score_deviation = df_xibei['score_deviation']
+        power_deviation = df_xibei['power_deviation']
+        # date_month = pandas.Series(list(map(time2split_month, date_time)))
+        # date_day = pandas.Series(list(map(time2split_day, date_time)))
+        date_month = df_xibei['time'].str[0:7]
+        date_day = df_xibei['time'].str[0:10]
+        deviation_score = score_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        ym_list = []
+        ymd_list = []
+        for name, group in score_deviation.groupby(date_day):
+            bd = datetime.datetime.strptime(name, '%Y-%m-%d')
+            yy_mm_dd = bd.strftime('%Y-%m-%d')
+            ymd_list.append(yy_mm_dd)
+        day_penalties = pandas.DataFrame(
+            numpy.c_[ymd_list, deviation_power, deviation_score],
+            columns=['date', 'Deviation_energy', 'Deviation_score'])
+        deviation_score = score_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        ym_list = []
+        for name, group in score_deviation.groupby(date_month):
+            bd = datetime.datetime.strptime(name, '%Y-%m')
+            yy_mm = bd.strftime('%Y-%m')
+            ym_list.append(yy_mm)
+        month_penalties = pandas.DataFrame(
+            numpy.c_[ym_list, deviation_power, deviation_score],
+            columns=['month', 'Deviation_energy', 'Deviation_score'])
+
+        return day_penalties, month_penalties
+
+
+    def calculate_xinjiang_solar_2022(self):
+        '''
+
+        2021年12月22日西北能监局发布修订完善西北区域两个细则
+        适用光伏预测曲线最大误差不超过20%
+        西北（除新疆外）新能源大发时段为 10:00-16:00
+        西北（除新疆外）用  电高峰时段为 06:00-09:00  17:00-22:00
+
+        新疆新能源大发时段为: 11:00-17:00
+        新疆用  电高峰时段为: 07:00-10:00  18:00-23:00
+
+        返回每日短期偏差积分电量
+        FBI WARING
+        '''
+        df_xibei = pandas.DataFrame([], columns=['time', 'power_real', 'power_forecast'])
+        df_xibei['time'] = self.date_time
+        df_xibei['power_real'] = self.power_real
+        df_xibei['power_forecast'] = self.power_forecast
+        df_xibei = df_xibei[df_xibei['power_real'] >= 0]
+        df_xibei = df_xibei[df_xibei['power_forecast'] >= 0]
+        series_time = df_xibei['time']
+        df_xibei['hour'] = series_time.str[11:16]
+        if len(df_xibei) > 0:
+            # 取列
+            dfs_time = df_xibei['time']
+            power_real = df_xibei['power_real']
+            power_forecast = df_xibei['power_forecast']
+            ymd = dfs_time.str[0:10]  # 选取 yyyy-mm-dd
+            df_hour = dfs_time.str[11:16]  # pandas series
+            cap = self.capacity
+            TSD = 0.2  # 风电日预测曲线最大误差0.25 ; 光伏日预测曲线最大误差0.2
+            # 特殊条件下
+            n_index1 = numpy.where(
+                numpy.logical_and(power_forecast == 0, power_real > cap * 0.03))
+            n_index2 = numpy.where(
+                numpy.logical_and(power_forecast == 0, power_real <= cap * 0.03))
+            n_index3 = numpy.where(
+                numpy.logical_and(power_forecast > cap * 0.03, power_real == 0))
+            n_index4 = numpy.where(
+                numpy.logical_and(power_forecast <= cap * 0.03, power_real == 0))
+            numpy.seterr(divide='ignore', invalid='ignore')
+            # 满足特殊条件
+            error_deviation = numpy.where(power_forecast > 0, (power_real - power_forecast) / power_forecast, 0)
+            error_deviation[n_index1[0]] = 1
+            error_deviation[n_index2[0]] = 0
+            error_deviation[n_index3[0]] = 1
+            error_deviation[n_index4[0]] = 0
+
+            # 偏差积分电量 计算时考虑了允许偏差25%，偏差变成26%就考核1% ；参考 TSD = |(pr-pf)/pf| ==> |pr-pf| = TSD*pf
+            power_deviation = numpy.where(
+                abs(error_deviation) > TSD,
+                abs(power_real - power_forecast) / 40 - power_forecast / 40 * TSD,
+                0)
+            # 2022西北新细则要求，新能源大发时段风电的偏差大于25%时 or 用电高峰时段的偏差时
+            df_xibei['error_deviation'] = error_deviation
+            df_xibei['power_deviation'] = power_deviation
+            df_xibei['score_deviation'] = power_deviation
+            for index, row in df_xibei.iterrows():
+                # 新能源大发时段
+                if '11:00' <= row.hour <= '17:00':
+                    if row.error_deviation > TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.4
+                    elif row.error_deviation < -TSD :
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.2
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0
+                # 新能源用电高峰时段
+                elif '07:00' <= row.hour <= '10:00' or '18:00' <= row.hour <= '23:00' :
+                    if row.error_deviation > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.2
+                    elif row.error_deviation < -TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation*0.4
+                else:
+                    if abs(row.error_deviation) > TSD:
+                        df_xibei.at[index, 'score_deviation'] = row.power_deviation * 0.2
+                    else:
+                        df_xibei.at[index, 'score_deviation'] = 0
+
+        score_deviation = df_xibei['score_deviation']
+        power_deviation = df_xibei['power_deviation']
+        # date_month = pandas.Series(list(map(time2split_month, date_time)))
+        # date_day = pandas.Series(list(map(time2split_day, date_time)))
+        date_month = df_xibei['time'].str[0:7]
+        date_day = df_xibei['time'].str[0:10]
+        deviation_score = score_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_day).sum()  # 偏差考核分数计算
+        ym_list = []
+        ymd_list = []
+        for name, group in score_deviation.groupby(date_day):
+            bd = datetime.datetime.strptime(name, '%Y-%m-%d')
+            yy_mm_dd = bd.strftime('%Y-%m-%d')
+            ymd_list.append(yy_mm_dd)
+        day_penalties = pandas.DataFrame(
+            numpy.c_[ymd_list, deviation_power, deviation_score],
+            columns=['date', 'Deviation_energy', 'Deviation_score'])
+        deviation_score = score_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        deviation_power = power_deviation.groupby(date_month).sum()  # 偏差考核分数计算
+        ym_list = []
+        for name, group in score_deviation.groupby(date_month):
+            bd = datetime.datetime.strptime(name, '%Y-%m')
+            yy_mm = bd.strftime('%Y-%m')
+            ym_list.append(yy_mm)
+        month_penalties = pandas.DataFrame(
+            numpy.c_[ym_list, deviation_power, deviation_score],
+            columns=['month', 'Deviation_energy', 'Deviation_score'])
 
+        return day_penalties, month_penalties
```

## Comparing `libeeepy-1.9.0.dist-info/RECORD` & `libeeepy-2.0.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-libeeepy/__init__.py,sha256=KIgec28wWmxyDiHQ0ZNfuKCe5F7IqaaGWvTKCUAhw8Q,114
-libeeepy/calculateaccuracy.py,sha256=SZIU-OQXISyfadE7x3uL6jORWFYJI33c9hfaeq6XcY0,53726
+libeeepy/__init__.py,sha256=TZRt1FmtGbbHbRwEv-s8GwKH9xC5pB-Quh0RUslug2k,114
+libeeepy/calculateaccuracy.py,sha256=gR9qmL79kQeqGPm6N7X9U1IIkDra0rpOH0-rcLlHMsM,111845
 libeeepy/dataprocessing.py,sha256=T2iQ07NvScIGYqiYDQZLX9C9k0fNd0BXhcqtKJLdw4U,6448
 libeeepy/operatemysql.py,sha256=xVAAtub3JHis9kxjXzgVKDS31AM1ad2aEJrg9rf6TDQ,5054
-libeeepy-1.9.0.dist-info/METADATA,sha256=yhltQcCPP5kyhHhY-KUjaEU8wiidor_S9L6ybO6saJ8,465
-libeeepy-1.9.0.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-libeeepy-1.9.0.dist-info/top_level.txt,sha256=GwgaDIXkQNHqRQlrOZ32alGenGFq8Q3nqdvyZvmyi_g,9
-libeeepy-1.9.0.dist-info/RECORD,,
+libeeepy-2.0.0.dist-info/METADATA,sha256=1zXsiaAXmaQxqwuvUqdfH1Ma0GbG1KVHlkb7Oqjc1tQ,464
+libeeepy-2.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+libeeepy-2.0.0.dist-info/top_level.txt,sha256=GwgaDIXkQNHqRQlrOZ32alGenGFq8Q3nqdvyZvmyi_g,9
+libeeepy-2.0.0.dist-info/RECORD,,
```

