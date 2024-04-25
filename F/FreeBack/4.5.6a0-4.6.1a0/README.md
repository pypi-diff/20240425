# Comparing `tmp/FreeBack-4.5.6a0.tar.gz` & `tmp/FreeBack-4.6.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeBack-4.5.6a0.tar", last modified: Mon Apr 22 19:15:40 2024, max compression
+gzip compressed data, was "FreeBack-4.6.1a0.tar", last modified: Thu Apr 25 03:12:44 2024, max compression
```

## Comparing `FreeBack-4.5.6a0.tar` & `FreeBack-4.6.1a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-22 19:15:40.306087 FreeBack-4.5.6a0/
-drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-22 19:15:40.304901 FreeBack-4.5.6a0/FreeBack/
--rw-r--r--   0 h1nlee     (501) staff       (20)       83 2024-04-20 02:32:40.000000 FreeBack-4.5.6a0/FreeBack/__init__.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    39658 2024-04-16 13:23:25.000000 FreeBack-4.5.6a0/FreeBack/alpha.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    33125 2024-04-22 14:03:41.000000 FreeBack-4.5.6a0/FreeBack/barbybar.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    12237 2024-04-20 06:25:35.000000 FreeBack-4.5.6a0/FreeBack/display.py
--rw-r--r--   0 h1nlee     (501) staff       (20)     9898 2024-04-13 14:29:24.000000 FreeBack-4.5.6a0/FreeBack/event.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    15856 2024-04-20 07:06:42.000000 FreeBack-4.5.6a0/FreeBack/my_pd.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    37494 2024-04-22 19:09:53.000000 FreeBack-4.5.6a0/FreeBack/post.py
--rw-r--r--   0 h1nlee     (501) staff       (20)    10281 2024-04-22 19:14:24.000000 FreeBack-4.5.6a0/FreeBack/strat.py
-drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-22 19:15:40.305617 FreeBack-4.5.6a0/FreeBack.egg-info/
--rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-22 19:15:40.000000 FreeBack-4.5.6a0/FreeBack.egg-info/PKG-INFO
--rw-r--r--   0 h1nlee     (501) staff       (20)      336 2024-04-22 19:15:40.000000 FreeBack-4.5.6a0/FreeBack.egg-info/SOURCES.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)        1 2024-04-22 19:15:40.000000 FreeBack-4.5.6a0/FreeBack.egg-info/dependency_links.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)       63 2024-04-22 19:15:40.000000 FreeBack-4.5.6a0/FreeBack.egg-info/requires.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)        9 2024-04-22 19:15:40.000000 FreeBack-4.5.6a0/FreeBack.egg-info/top_level.txt
--rw-r--r--   0 h1nlee     (501) staff       (20)    35148 2024-04-13 14:29:24.000000 FreeBack-4.5.6a0/LICENSE
--rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-22 19:15:40.305829 FreeBack-4.5.6a0/PKG-INFO
--rw-r--r--   0 h1nlee     (501) staff       (20)      565 2024-04-16 13:23:25.000000 FreeBack-4.5.6a0/README.md
--rw-r--r--   0 h1nlee     (501) staff       (20)       38 2024-04-22 19:15:40.306136 FreeBack-4.5.6a0/setup.cfg
--rw-r--r--   0 h1nlee     (501) staff       (20)     1248 2024-04-22 19:11:34.000000 FreeBack-4.5.6a0/setup.py
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-25 03:12:44.254493 FreeBack-4.6.1a0/
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-25 03:12:44.253247 FreeBack-4.6.1a0/FreeBack/
+-rw-r--r--   0 h1nlee     (501) staff       (20)       83 2024-04-20 02:32:40.000000 FreeBack-4.6.1a0/FreeBack/__init__.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    39718 2024-04-23 12:48:33.000000 FreeBack-4.6.1a0/FreeBack/alpha.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    33139 2024-04-25 01:23:47.000000 FreeBack-4.6.1a0/FreeBack/barbybar.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    14423 2024-04-25 03:10:46.000000 FreeBack-4.6.1a0/FreeBack/display.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)     9918 2024-04-23 12:50:24.000000 FreeBack-4.6.1a0/FreeBack/event.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    15856 2024-04-20 07:06:42.000000 FreeBack-4.6.1a0/FreeBack/my_pd.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    36946 2024-04-25 03:04:47.000000 FreeBack-4.6.1a0/FreeBack/post.py
+-rw-r--r--   0 h1nlee     (501) staff       (20)    10021 2024-04-24 14:08:11.000000 FreeBack-4.6.1a0/FreeBack/strat.py
+drwxr-xr-x   0 h1nlee     (501) staff       (20)        0 2024-04-25 03:12:44.254052 FreeBack-4.6.1a0/FreeBack.egg-info/
+-rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-25 03:12:44.000000 FreeBack-4.6.1a0/FreeBack.egg-info/PKG-INFO
+-rw-r--r--   0 h1nlee     (501) staff       (20)      336 2024-04-25 03:12:44.000000 FreeBack-4.6.1a0/FreeBack.egg-info/SOURCES.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)        1 2024-04-25 03:12:44.000000 FreeBack-4.6.1a0/FreeBack.egg-info/dependency_links.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)       74 2024-04-25 03:12:44.000000 FreeBack-4.6.1a0/FreeBack.egg-info/requires.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)        9 2024-04-25 03:12:44.000000 FreeBack-4.6.1a0/FreeBack.egg-info/top_level.txt
+-rw-r--r--   0 h1nlee     (501) staff       (20)    35148 2024-04-13 14:29:24.000000 FreeBack-4.6.1a0/LICENSE
+-rw-r--r--   0 h1nlee     (501) staff       (20)      991 2024-04-25 03:12:44.254249 FreeBack-4.6.1a0/PKG-INFO
+-rw-r--r--   0 h1nlee     (501) staff       (20)      565 2024-04-16 13:23:25.000000 FreeBack-4.6.1a0/README.md
+-rw-r--r--   0 h1nlee     (501) staff       (20)       38 2024-04-25 03:12:44.254536 FreeBack-4.6.1a0/setup.cfg
+-rw-r--r--   0 h1nlee     (501) staff       (20)     1269 2024-04-25 03:12:11.000000 FreeBack-4.6.1a0/setup.py
```

### Comparing `FreeBack-4.5.6a0/FreeBack/alpha.py` & `FreeBack-4.6.1a0/FreeBack/alpha.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pandas as pd
 import numpy as np
 from scipy import stats
 import statsmodels.api as sm
-from FreeBack.post import matplot
-from FreeBack import my_pd
+import FreeBack as FB
 import os
 # 该模块包含：
 # 因子计算常用函数
 # 单因子与多因子检验模块（组合法、回归法）
 
 
 #######################################################################################################
@@ -70,15 +69,15 @@
 # 没有周一和1号的月份用下一个第一个出现的值***
 def resample_select(market, freq='month'):
     if freq=='month':
         return market[market.index.map(lambda x:getattr(x[0], 'day'))==1]
     elif freq=='week':
         return market[market.index.map(lambda x:getattr(x[0], 'weekday')())==0]
 def QQ(factor, date=None):
-    plt, fig, ax = matplot(w=6, d=4)
+    plt, fig, ax = FB.display.matplot(w=6, d=4)
     if date==None:
         norm_dis = pd.Series(np.random.randn(len(factor))).sort_values()
         ax.scatter(norm_dis, factor.sort_values())
     else:
         norm_dis = pd.Series(np.random.randn(len(factor.loc[date]))).sort_values()
         ax.scatter(norm_dis, factor.loc[date].sort_values())
     ax.plot(norm_dis, norm_dis, c='C3', ls='--')
@@ -316,15 +315,15 @@
 # plot
 # 因子组合收益（单边做多，考虑交易成本（默认单边万7））
     def HoldReturn(self, i_period=0, dateleft=None, dateright=None, cost=0):
         if dateleft==None:
             dateleft = self.factor.index[0][0]
         if dateright==None:
             dateright = self.factor.index[-1][0]
-        plt, fig, ax = matplot()
+        plt, fig, ax = FB.display.matplot()
         ax2 = ax.twinx()
         # 画图曲线颜色和透明度区分
         # 不包含等权指数
         if self.justdivide:
             number = len(self.a_b)
         else:
             number = len(self.a_b)-1
@@ -378,15 +377,15 @@
         plt.show()
 # 各组对数收益率-等权对数收益率
     def LogCompare(self, i_period=0, dateleft=None, dateright=None, ifbench=True):
         if dateleft==None:
             dateleft = self.factor.index[0][0]
         if dateright==None:
             dateright = self.factor.index[-1][0]
-        plt, fig, ax = matplot()
+        plt, fig, ax = FB.display.matplot()
         if ifbench:
             benchmark = self.mat_lr[i_period][-1].cumsum()
         else:
             benchmark = 0
         # 画图曲线颜色和透明度区分
         # 等权指数不画
         number = len(self.a_b)-1
@@ -424,15 +423,15 @@
     def Bar(self, i_period=0):
         # 按年度划分收益率
         df_returns = pd.concat(self.mat_lr[i_period], axis=1)\
             .rename(columns=dict(zip(range(len(self.a_b)), self.a_b)))
         df_returns['year'] = df_returns.index.year
         df_returns = 100*(np.exp(df_returns.groupby('year').sum())-1)
         # 作图
-        plt, fig, ax = matplot()
+        plt, fig, ax = FB.display.matplot()
         x = np.arange(len(df_returns))
         width = 0.08
         # 偏移量
         move = np.arange(-len(self.a_b)*width/2,len(self.a_b)*width/2,width)
         for n in range(len(self.a_b)):
             ax.bar(np.arange(len(df_returns))+move[n], df_returns[self.a_b[n]].values,\
                     width=width, label='%s'%(str(self.a_b[n])))
@@ -444,15 +443,15 @@
         else:
             os.mkdir('output')
         plt.savefig('./output/alpha-Portfolio-Bar.png',\
                      bbox_inches='tight')
         plt.show()
 # 各组分组因子值阈值和数量
     def FactorThreshold(self):
-        plt, fig, ax = matplot()
+        plt, fig, ax = FB.display.matplot()
         # 颜色与LogCompare中相同，最大值和最小值为橙色C1
         # 等权指数不画
         number = len(self.a_b)-1
         number0 = int(number/2)
         number1 = number - number0
         #前一半为绿色，后一半为红色 （做多因子数值高组，做空因子数值低组）
         color_list = ['C2']*number0 + ['C3']*number1
@@ -511,15 +510,15 @@
     else:
         group0 = group_value0
         market_factor[group0] = market_factor[group0].groupby('code').shift(delay).dropna()
     if group_value1==None:
         group = market_factor.groupby([group0, 'date'])
         result_returns = group[returns_key].mean()
 
-        plt, fig, ax = matplot()
+        plt, fig, ax = FB.display.matplot()
         ax1 = ax.twinx()
         for i in result_returns.index.get_level_values(0).unique():
             ax.plot(result_returns.loc[i].cumsum(), label='group %s, %.2lf'%(i, \
                         100*np.exp(250*result_returns.loc[i].mean())-100))
             ax1.plot(group['close'].count().loc[i], alpha=0.3)
         ax.legend()
         ax.set_ylabel('累计收益率（单利）')
@@ -562,15 +561,15 @@
             return [1,1-(x-min_r)/max_r,1-(x-min_r)/max_r]
         elif x == 0:
             return [1,1,1]
         else:
             return [1+(x-min_r)/max_r,1,1+(x-min_r)/max_r]
     # 
     plot = np.ones((len(level0s),len(level1s),3))
-    plt, fig, ax = matplot()
+    plt, fig, ax = FB.display.matplot()
     for level0 in range(len(level0s)):
         for level1 in range(len(level1s)):
             # 先列再行
             plot[level0][level1] = color_map(dict_returns[(level0s[level0], level1s[level1])], \
                                     0.9*min(dict_returns.values()), 1.1*max(dict_returns.values()))
             # 先行再列
             ax.text(level1, level0, 
@@ -739,15 +738,15 @@
         self.fr_dict = fr_dict
         self.cross_dict = cross_dict
         self.gamma_dict = gamma_dict
         self.result = result
         display(result)
     # 因子收益率
     def factor_return(self, period=1, rolling_period=20):
-        plt, fig, ax = matplot()
+        plt, fig, ax = FB.display.matplot()
         cumsum_fr = 250*self.fr_dict[period].cumsum()
         ax.plot(cumsum_fr, label='累计因子收益率', c='C0')
         ax.plot(cumsum_fr.rolling(20).min(),\
                  alpha=0.5, c='C2')
         ax.plot(cumsum_fr.rolling(20).max(),\
                   alpha=0.5, c='C3')
         ax.legend(loc='lower left')
@@ -756,15 +755,15 @@
         ax2.plot(250*self.fr_dict[period].rolling(rolling_period).mean(), label='滚动因子收益率（右）', c='C1')
         #ax2.legend(loc='lower right')
         ax2.legend(bbox_to_anchor=(0.78, 1.06), loc=10, ncol=1)
         ax.set_xlim(self.factor.index[0][0], self.factor.index[-1][0])
         plt.show() 
     # 截面因子与收益率（散点图） n为分级靠档组数
     def cross(self, date=None, period=1, n=100):
-        plt, fig, ax = matplot()
+        plt, fig, ax = FB.display.matplot()
         df_corr = self.cross_dict[period].copy()
         if self.point:
             beta = self.fr_dict[period]
         else:
             beta = self.fr_dict[period]*period
         gamma = self.gamma_dict[period]
         r = self.IC_dict[period]
```

### Comparing `FreeBack-4.5.6a0/FreeBack/barbybar.py` & `FreeBack-4.6.1a0/FreeBack/barbybar.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,16 @@
     # 更新现金函数
     def update_cash(self, cash):
         self.cur_cash = cash
         self.series_cash.loc[self.cur_bar] = cash
     # 每个bar开始结束时调用
     # 更新净值函数 包含更新hold amount
     def update_net(self):
-        self.cur_hold_amount = (self.cur_hold_vol * self.cur_market['close']).loc[self.cur_hold_vol.index].sort_values(ascending=False) 
+        self.cur_hold_amount = (self.cur_hold_vol * self.cur_market['close']).\
+            loc[self.cur_hold_vol.index].sort_values(ascending=False) 
         hold_amount = self.cur_hold_amount
         name_hold = hold_amount.index
         name_notnan = hold_amount[~np.isnan(hold_amount)].index
         name_delist = list(set(name_hold) - set(name_notnan))
         # 如果持有中有退市标的
         if name_delist != []:
             self.log_error('hold lost----delist list: %s'%name_delist)
```

### Comparing `FreeBack-4.5.6a0/FreeBack/display.py` & `FreeBack-4.6.1a0/FreeBack/display.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import matplotlib.pyplot as plt
 from mpl_toolkits.axisartist.parasite_axes import HostAxes, ParasiteAxes
 import seaborn as sns
 from pyecharts import options as opts
 from pyecharts.charts import Kline,Bar,Grid,Line
 from pyecharts.commons.utils import JsCode
 import numpy as np
-import datetime
+import datetime, xlsxwriter
 
 ###########################################################
 ######################## 静态图 ###########################
 ###########################################################
 
 
 # matplot绘图
@@ -171,14 +171,65 @@
             if not np.isnan(calendar[i_][j_]):
                 ax.text(j_, i_, calendar[i_][j_].round(2), ha='center', va='center')
 
     return plt, fig, ax
 '''
 
 
+# excel表
+def write_df(df, name, title=True, index=True, col_width={}, row_width={}):
+    workbook = xlsxwriter.Workbook('%s.xlsx'%name)
+    worksheet = workbook.add_worksheet()
+    worksheet.freeze_panes(1, 1)   # 冻结首行
+    # 列宽设置
+    for k,v in col_width.items():
+        worksheet.set_column('%s:%s'%(k,k), v)
+    # 行高设置
+    for k,v in row_width.items():
+        worksheet.set_row('%s:%s'%(k,k), v)
+    # 格式
+    general_prop = {'font_size':10, 'align':'center', 'valign':'vcenter', 'text_wrap':1}
+    format_title = workbook.add_format(dict([(k,general_prop[k]) for k in general_prop]\
+                                +[('font_size',14), ('bold',True),\
+                                    ('bg_color','#0066ff'), ('font_color','#ffffff')]))
+    format_text = workbook.add_format(dict([(k,general_prop[k]) for k in general_prop]\
+                                +[('num_format', '#,##0.0')]))
+    format_date = workbook.add_format(dict([(k,general_prop[k]) for k in general_prop]\
+                                +[('num_format', 'yyyy-mm-dd')]))
+    def judge_format(text):
+        return format
+        # 标题与序号 
+    if index:
+        if (type(df.index[0])==datetime.date) | (type(df.index[0])==type(df.index[0])):
+            worksheet.write_column("A%s"%(int(title)+1), list(df.index), format_date)
+        else:
+            worksheet.write_column("A%s"%(int(title)+1), list(df.index), format_text)
+        if title:
+            if df.index.name==None:
+                worksheet.write(0, 0, '', format_title)
+            else:
+                worksheet.write(0, 0, df.index.name, format_title)
+            worksheet.write_row("B1", list(df.columns), format_title)
+    elif title:
+        worksheet.write_row("A1", list(df.columns), format_title)
+    # Iterate over the data and write it out row by row.
+    row=int(title)
+    col=int(index)
+    for i, r in df.iterrows():
+        for j, v in r.items():
+            try:
+                worksheet.write(row, col, v, format_text)
+            except:
+                worksheet.write(row, col, '')
+            col += 1
+        col = int(index)
+        row += 1
+    workbook.close()
+
+
 
 ###########################################################
 ######################## 动态交互图 ###########################
 ###########################################################
```

### Comparing `FreeBack-4.5.6a0/FreeBack/event.py` & `FreeBack-4.6.1a0/FreeBack/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import pandas as pd
 import numpy as np
-from FreeBack.post import matplot
-from FreeBack.my_pd import parallel_group
-
+import FreeBack as FB
 
 class Event():
     '''
     事件驱动测试
     参数格式:
     multi——index: date, code
     signal: 入场信号,index格式
@@ -50,15 +48,15 @@
         elif self.bench_type == 'equal':
             self.bench_sr = self.bench_sr
         if type(self.custom_bench)==type(None):
             self.bench_sr = self.custom_bench.loc[self.bench_sr.index]
         self.sr = self.sr - self.bench_sr
         self.sr.name = 'sr'
         cols = [i-self.before+1 for i in range(self.length)]
-        self.signal_sr_df = parallel_group(self.sr, fun1, n_core=self.n_core).loc[self.signal]
+        self.signal_sr_df = FB.my_pd.parallel_group(self.sr, fun1, n_core=self.n_core).loc[self.signal]
         self.number = self.signal_sr_df[0].groupby(level='date').count()
         self.bench_net = (self.bench_sr + 1).cumprod()
         self.net = (self.signal_sr_df+1).cumprod(axis=1)
 
     def fast_init(self):
         self.length = self.before + self.after
         self.sr = (self.price/self.price.groupby('code').shift() - 1).fillna(0)
@@ -81,15 +79,15 @@
         self.number = self.signal_sr_df[0].groupby(level='date').count()
         # 净值
         self.bench_net = (self.bench_sr + 1).cumprod()
         self.net = (self.signal_sr_df+1).cumprod(axis=1)
 
     # 每日触发信号数量, bench_type zero时没有bench
     def draw_turnover(self):
-        plt0, fig0, ax0 = matplot()
+        plt0, fig0, ax0 = FB.display.matplot()
         ax1 = ax0.twinx()
         num = self.number
         ax1.plot(num.cumsum(), color='C2', label='累计样本量（右）')
         # 触发次数过多的截断
         index = num[num > (num.mean() + 5*num.std())].index
         num.loc[index] = num.mean() + 5*num.std()
         ax0.bar(num.index, num.values, color='grey', label='每日样本量')
@@ -97,15 +95,15 @@
             #ax1.plot(self.bench_net, color='steelblue', label='基准净值（右）')
         #fig0.legend(bbox_to_anchor=(0.5, 0), loc=10, ncol=2)
         fig0.legend(loc='lower center', ncol=2)
         plt0.show()
     
     # 每日超额, 事件净值(取均值)
     def draw_net(self):
-        plt0, fig0, ax0 = matplot()
+        plt0, fig0, ax0 = FB.display.matplot()
         sr = self.signal_sr_df.mean(axis=0)
         ax0.bar(sr.index, sr.values, width=0.5,  label='单日超额', color='darkgoldenrod')
         ax1 = ax0.twinx()
         net = self.net.mean()
         net = net/net.loc[1]
         ax1.plot(net, color='crimson', label='累计净值（右）', linewidth=2.0)
         ax1.hlines(1, sr.index[0], sr.index[-1], colors='k', linestyles='--')
@@ -130,53 +128,53 @@
         ## 收益率分布
         ##plt, fig, ax = post.matplot()
         ##sns.histplot(trade_result[2])
         ##plt.show()
         position = (winrate*win - (1-winrate)*loss)/(win*loss)
         position[position<0] = 0
         # 作图
-        plt, fig, ax = matplot()
+        plt, fig, ax = FB.display.matplot()
         ax.plot(100*winrate, c='C2', label='胜率')
         ax.plot(100*odds, c='C0', label='赔率')
         ax1 = ax.twinx()
         ax1.plot(position, c='C3', label='最佳仓位')
         ax.set_ylabel('（%）')
         ax.set_xlabel('bar')
         fig.legend(loc='lower center', ncol=3)
         plt.show()
 
 
     # 净值累计加减一个方差
     def draw_std_net(self):
-        plt1, fig1, ax1 = matplot()
+        plt1, fig1, ax1 = FB.display.matplot()
         net = self.net.loc[:, 1:]
         net_mean = net.mean()
         net_up = net_mean + self.net.std()
         net_low = net_mean - self.net.std()
         ax1.plot(net_mean, color='darkblue', linewidth=2.0, label='均值')
         ax1.plot(net_up, color='darkred', linewidth=2.0, label='均值+方差')
         ax1.plot(net_low, color='darkgreen', linewidth=2.0, label='均值-方差')
         ax1.legend(loc='upper left')
         plt1.show()
     
     # 净值累计最大值&净值最小值
     def draw_e_ratio(self):
-        plt1, fig1, ax1 = matplot()
+        plt1, fig1, ax1 = FB.display.matplot()
         net = self.net.loc[:, 1:]
         net_max = net.cummax(axis=1).mean()
         net_min = net.cummin(axis=1).mean()
         e_ratio = net_max/net_min
         ax1.plot(e_ratio, color='darkred', linewidth=2.0)
         ax1.set_xlabel('set_xlabel')
         plt1.show()
     
     # 仅一个信号
     # i是siganl中第i个信号
     def draw_one_signal_net(self, date, code):
-        plt0, fig0, ax0 = matplot()
+        plt0, fig0, ax0 = FB.display.matplot()
         sr = self.signal_sr_df.loc[date, code]
         ax0.bar(sr.index, sr.values, width=0.5,  label='单日超额', color='darkgoldenrod')
         ax1 = ax0.twinx()
         net = self.net.loc[date, code]
         net = net/net.loc[1]
         ax1.plot(net, color='crimson', label='累计净值', linewidth=2.0)
         fig0.legend(loc='lower center')
```

### Comparing `FreeBack-4.5.6a0/FreeBack/my_pd.py` & `FreeBack-4.6.1a0/FreeBack/my_pd.py`

 * *Files identical despite different names*

### Comparing `FreeBack-4.5.6a0/FreeBack/post.py` & `FreeBack-4.6.1a0/FreeBack/post.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 import datetime
 import statsmodels.api as sm
+from statsmodels.sandbox.stats.runs import runstest_1samp
 from plottable import ColumnDefinition, ColDef, Table
 from matplotlib.colors import LinearSegmentedColormap
-from FreeBack.display import *
 import FreeBack as FB
 import os
 # 该模块处理策略的后处理(业绩评价、归因）工作，主要包含：
 # 1. ReturnsPost 收益率序列后处理
 # 2. HoldPost 持仓矩阵后处理
 # 3. WorldPost barbybar模块World对象后处理
 
@@ -36,14 +36,15 @@
             benchmark = pd.DataFrame(index = self.returns.index)
             benchmark['zero'] = 0
             self.benchmark = benchmark
         self.benchmark = benchmark.loc[self.returns.index].fillna(0)
         self.sigma_benchmark = np.exp(np.log(self.benchmark[\
             self.benchmark.columns[0]]+1).std())-1
         self.cal_detail()
+        self.detail()
     # 详细评价表
     def cal_detail(self):
         # 策略绝对表现
         self.net = (1+self.returns).cumprod()
         self.lr = np.log(self.returns + 1)
         #self.returns.index.name = 'date'
         self.years = (self.returns.index[-1]-self.returns.index[0]).days/365  
@@ -78,48 +79,48 @@
         col0.loc[1] = '%s, %s'%(round(self.years,1), len(self.net))
         col1 = pd.DataFrame(columns=['col1'])
         col1.loc[0] = '年化收益率（%）'
         col1.loc[1] = round(self.return_annual*100,1)
         col1.loc[2] = '年化超额收益率（%）'
         col1.loc[3] = round(self.excess_return_annual*100,1)
         col2 = pd.DataFrame(columns=['col2'])
-        col2.loc[0] = '日胜率（%）'
-        col2.loc[1] = round(100*(self.returns>0).mean(),1) 
+        col2.loc[0] = '日胜率（%）'  # 没亏就是赢
+        col2.loc[1] = round(100*(self.returns>=0).mean(),1) 
         col2.loc[2] = '超额日胜率（%）'
         col2.loc[3] = round(100*(self.excess_lr>0).mean(),1) 
         col3 = pd.DataFrame(columns=['col3'])
         col3.loc[0] = '最大回撤（%）'
         col3.loc[1] = round(max(self.drawdown)*100, 1)
         col3.loc[2] = '超额最大回撤（%）'
         col3.loc[3] = round(max(self.excess_drawdown)*100, 1)
         col3.loc[4] = '波动率（%）'
         col3.loc[5] = round(self.sigma*np.sqrt(250)*100, 1)
         col4 = pd.DataFrame(columns=['col4'])
         col4.loc[0] = 'beta系数'
         col4.loc[1] = round(self.beta,2) 
-        col4.loc[2] = '詹森指数（%）'
+        col4.loc[2] = 'alpha（%）'
         col4.loc[3] = round(self.alpha*250*100,1)
         col5 = pd.DataFrame(columns=['col5'])
         col5.loc[0] = '夏普比率'
         col5.loc[1] = round(self.sharpe,2)
         col5.loc[2] = '超额夏普' 
         col5.loc[3] = round(self.excess_sharpe,2)
         col5.loc[4] = '卡玛比率'
         col5.loc[5] = round(self.return_annual/max(self.drawdown),2)
         col6 = pd.DataFrame(columns=['col6'])
         col6.loc[0] = ''
         col6.loc[1] = '' 
         col7 = pd.DataFrame(columns=['col7'])
-        col7.loc[0] = 'Hurst指数' 
-        col7.loc[1] = '' 
+        col7.loc[0] = '游程检验（%）'   # 拒绝随机假设的概率 
+        col7.loc[1] = round(100*runstest_1samp(self.returns>0)[1],2)
         df_details = pd.concat([col0, col1, col2, col3, \
                 col4, col5, col6, col7], axis=1).fillna('')
         self.df_details = df_details
     def detail(self):
-        plt, fig, ax = matplot(w=22)
+        plt, fig, ax = FB.display.matplot(w=22)
         column_definitions = [ColumnDefinition(name='col0', group="基本参数"), \
                               ColumnDefinition(name='col1', group="收益能力"), \
                             ColumnDefinition(name='col2', group='收益能力'), \
                             ColumnDefinition(name='col3', group='风险水平'), \
                             ColumnDefinition(name="col4", group='风险调整'), \
                             ColumnDefinition(name="col5", group='风险调整'), \
                             ColumnDefinition(name="col6", group='策略执行'),
@@ -320,100 +321,81 @@
         check_output()
         plt.savefig('./output/pnl_monthly.png')
         plt.show()
 
 
 
 ############################################################################################
-################################### 处理持仓表 ##############################################
-############################################################################################
-
-
-
-class HoldPost(ReturnsPost):
-    # 持仓表、单边交易成本、market
-    def __init__(self, df_hold, market=None, comm=0/1e4, \
-                 benchmark=0, stratname='策略'):
-        self.df_hold = df_hold
-        self.comm = comm
-        self.market = market
-        # 等权持仓
-        df_hold['weight'] = 1
-        df_hold['weight'] = df_hold['weight']/df_hold['weight'].groupby('date').sum()
-        # 初始状态全仓为现金,没有现金列则
-        pos_df = df_hold['weight'].unstack('code').fillna(0)
-        pos_df_shift = pos_df.shift().fillna(0).copy()
-        pos_df_shift.loc[pos_df.index[0], 'deposit'] = 1
-        pos_df_shift.fillna(0)
-        # 去掉现金列的绝对值增减之和即为换手率
-        self.turnover_ser = abs(pos_df-pos_df_shift).drop(columns=['deposit', ]).sum(axis=1)
-        # 收益率
-        returns = (df_hold.groupby('date')['next_returns'].mean()+1)*(1-self.turnover_ser*self.comm)-1
-        super(HoldPost, self).__init__(returns, benchmark=benchmark, stratname=stratname)
-        self.df_details.loc[0, 'col6'] = '年换手' 
-        self.df_details.loc[1, 'col6'] = round(self.turnover_ser.mean()*250,1)
-    def turnover(self):
-        plt, fig, ax = FB.display.matplot()
-        ax.plot(self.turnover_ser*250, alpha=0.2)
-        ax.plot(self.turnover_ser.rolling(20).mean()*250, label='20日滚动换手')
-        ax.plot(self.turnover_ser.rolling(250).mean()*250, label='250日滚动换手')
-        ax.legend()
-        check_output()
-        plt.savefig('./output/turnover.png')
-        plt.show()
-    def get_contribution(self):
-        real_returns = self.df_hold['next_returns']/self.df_hold.groupby('date')['next_returns'].count()
-        self.contribution = ((real_returns+1).groupby('code').prod()-1).sort_values()
-    def get_holdtable(self):
-        # 持仓明细
-        result_hold = {}
-        for r in self.df_hold[[]].join(self.market['name'])['name'].unstack().iterrows():
-            temp_str = ''
-            for i,v in r[1].dropna().items():
-                temp_str += str(v)+'('+str(i)+'),'
-            result_hold[r[0]] = temp_str
-        self.result_hold = pd.Series(result_hold)
-        self.result_hold.to_excel('./output/hold.xlsx')
-
-
-
-############################################################################################
 ################################### 处理Strat对象 ##############################################
 ############################################################################################
 
 
 
 class StratPost(ReturnsPost):
     # 持仓表、单边交易成本、market()
     def __init__(self, strat0, market=None, \
-                 benchmark=0, stratname='策略'):
-        self.strat = strat0
+                 benchmark=0, stratname='策略', rf=0.03):
+        #self.strat = strat0
         self.market = market
-    def turnover(self):
+        self.turnover = strat0.turnover 
+        self.df_hold = strat0.df_hold
+        self.df_amount = strat0.df_amount
+        super().__init__(strat0.returns, benchmark, stratname, rf)
+    def detail(self):
+        # 空仓时间
+        self.df_details.loc[2, 'col0'] = '空仓时间（日）'
+        self.df_details.loc[3, 'col0'] = (self.df_hold.drop(columns='cash')==0).all(axis=1).sum()
+        # 策略执行
+        self.df_details.loc[0, 'col6'] = '年化换手，持股周期'
+        self.df_details.loc[1, 'col6'] = '%s, %s'%(round(self.turnover.sum()/self.years),\
+                                                   round(500/(self.turnover.sum()/self.years)))
+        super().detail()
+    def plot_turnover(self):
         plt, fig, ax = FB.display.matplot()
-        ax.plot(self.turnover_ser*250, alpha=0.2)
-        ax.plot(self.turnover_ser.rolling(20).mean()*250, label='20日滚动换手')
-        ax.plot(self.turnover_ser.rolling(250).mean()*250, label='250日滚动换手')
+        ax.plot(self.turnover*250, alpha=0.2)
+        ax.plot(self.turnover.rolling(20).mean()*250, label='20日滚动换手')
+        ax.plot(self.turnover.rolling(250).mean()*250, label='250日滚动换手')
         ax.legend()
         check_output()
         plt.savefig('./output/turnover.png')
         plt.show()
-    def get_contribution(self):
-        real_returns = self.df_hold['next_returns']/self.df_hold.groupby('date')['next_returns'].count()
-        self.contribution = ((real_returns+1).groupby('code').prod()-1).sort_values()
     def get_holdtable(self):
-        # 持仓明细
-        result_hold = {}
-        for r in self.df_hold[[]].join(self.market['name'])['name'].unstack().iterrows():
-            temp_str = ''
-            for i,v in r[1].dropna().items():
-                temp_str += str(v)+'('+str(i)+'),'
-            result_hold[r[0]] = temp_str
-        self.result_hold = pd.Series(result_hold)
-        self.result_hold.to_excel('./output/hold.xlsx')
+        # 持仓数量
+        held = pd.DataFrame(self.df_hold.stack()[self.df_hold.stack()!=0]).\
+                    rename(columns={0:'hold'})
+        # 持仓金额
+        held = held.join(pd.DataFrame(self.df_amount.stack()).rename(columns={0:'amount'}))
+        # 是否加入持仓品种名称
+        try:
+            if 'name' in self.market.columns:
+                held = held.join(self.market['name'])
+                held.loc[held.index[held.index.get_level_values(1)=='cash'], 'name'] = '现金'
+        except:
+            pass
+        self.held = held
+        # 持仓表(名称，代码，持仓量，持仓额)
+        result_hold = pd.DataFrame()
+        for date in self.held.index.get_level_values(0).unique():
+            temp = self.held.loc[date].sort_values(by='amount', ascending=False)
+            iamount = 0
+            for idx,val in temp.iterrows():
+                if 'name' in self.market.columns:
+                    keystring = val['name']+'('+str(idx)+')'+ ', 持仓量：'+str(val['hold'])+', 持仓额：'+str(val['amount'])
+                else:
+                    keystring = str(idx) + ', 持仓量：'+str(round(val['hold'],0))+', 持仓额：'+str(round(val['amount'],1))
+                result_hold.loc[date, 'hold%s'%iamount] = keystring
+                iamount += 1
+        result_hold = result_hold.join(pd.DataFrame(10000*self.returns).rename(columns={0:'收益率(万)'}))
+        result_hold.index.name = '日期'
+        self.result_hold = result_hold
+
+        FB.display.write_df(result_hold , "./output/持仓表", col_width={'A':10})
+
+        #self.result_hold = pd.Series(result_hold)
+        #self.result_hold.to_excel('./output/hold.xlsx')
 
 
 
 ########################################################################################################
 ####################################  barbybar.world  ##################################################
 ########################################################################################################
 
@@ -587,15 +569,15 @@
         col7.loc[4] = '' 
         col7.loc[5] = '' 
         col7.loc[6] = '' 
         col7.loc[7] = '' 
         df_details = pd.concat([col0, col1, col2, col3, \
                 col4, col5, col6, col7], axis=1)
 
-        plt, fig, ax = matplot(w=22)
+        plt, fig, ax = FB.display.matplot(w=22)
         column_definitions = [ColumnDefinition(name='col0', group="收益能力"), \
                               ColumnDefinition(name='col1', group="收益能力"), \
                             ColumnDefinition(name='col2', group='收益能力'), \
                             ColumnDefinition(name='col3', group='风险水平'), \
                             ColumnDefinition(name="col4", group='风险水平'), \
                             ColumnDefinition(name="col5", group='风险调整'), \
                             ColumnDefinition(name="col6", group='风险调整'),
@@ -613,15 +595,15 @@
         tab.columns["index"].set_facecolor("white")
         tab.columns["index"].set_fontcolor("white")
         tab.columns["index"].set_linewidth(0)
         plt.savefig('details.png')
         plt.show()
 # 净值曲线
     def pnl(self, timerange=None, detail=False, filename=None, log=False, excess=True):
-        plt, fig, ax = matplot(w=10)
+        plt, fig, ax = FB.display.matplot(w=10)
         # 只画一段时间内净值（用于展示局部信息,只列出sharpe）
         if type(timerange) != type(None):
             # 时间段内净值与基准
             net = self.net.loc[timerange[0]:timerange[1]]
             returns = self.returns.loc[timerange[0]:timerange[1]]
             # 计算夏普
             years = (pd.to_datetime(timerange[1])-pd.to_datetime(timerange[0])).days/365
@@ -718,15 +700,15 @@
         self.winrate = self.trades_win.sum().values[0]/len(self.trades)
         self.odds = -(self.trades[self.trades_win[0]].mean()/self.trades[self.trades_loss[0]].mean()).values[0]
     def trade_plot(self):
         # 交易次数
         Close_count = self.Close_amount.reset_index()[['date',0]].set_index('date')
         Close_count = Close_count.groupby('date').count().cumsum()
         # 画图
-        plt, fig, ax = matplot()
+        plt, fig, ax = FB.display.matplot()
         ax.plot(Close_count, label='累积交易次数 胜率：%s 盈亏比：%s'%(round(self.winrate, 2), round(self.odds, 2)))
         ax.set_xlim(self.net.index[0], self.net.index[-1])
         ax.legend()
         plt.gcf().autofmt_xdate()
         plt.savefig('trade.png')
         plt.show()
     def trade_monthly(self):
@@ -739,15 +721,15 @@
         self.month_winrate = count_win/(count_win + count_loss)
 #        self.month_odds = -mean_win/mean_loss
         plt,fig,ax = month_thermal(self.month_winrate, 0.5)
         plt.savefig('trade_monthly.png') 
         plt.show()
 # 仓位分析
     def position(self):
-        plt, fig, ax = matplot()
+        plt, fig, ax = FB.display.matplot()
         held_amount = self.held.groupby('date').sum()
         # 0是资产 1是现金
         df_total = pd.concat([self.held.groupby('date').sum(), self.cash], axis=1).fillna(0)
         df_max = pd.concat([self.held.groupby('date').max(), self.cash], axis=1).fillna(0)
         df_count = pd.concat([self.held.groupby('date').count(), self.cash], axis=1).fillna(0)
         ax.plot(df_total[0]/df_total.sum(axis=1), label='非现金仓位')
         ax.set_xlim(self.held.index[0][0], self.held.index[-1][0])
```

### Comparing `FreeBack-4.5.6a0/FreeBack/strat.py` & `FreeBack-4.6.1a0/FreeBack/strat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,84 +1,104 @@
 import FreeBack as FB
 import numpy as np
 import pandas as pd
 
+
+
 ####################################################################
 ########################## 常用策略框架 ##############################
 ###################################################################
 
+
+
 # 择股策略、元策略
 class MetaStrat():
-    # 'inexclude':, 
+    # 'inexclude':,
         # 当格式为('bool', False)时， 'bool'列为筛选条件, True为符合条件的证券
         # 格式为（False, 'bool'), 'bool'列为排除条件, False为符合条件的证券
         # 格式为 ['code0', 'code1', ] 时为等权持有固定证券组合，'cash'表示持有现金
     # 'score':float,   按score列由大到小选取证券,等权持有
     # 'hold_num':float,    取前hold_num（大于1表示数量，小于1小于百分比）只
     # market，pd.DataFrame, 需要包括策略需要调取的列，可以先不加
     # price，当前日期可以获得的价格数据,可以使用 'close'收盘价（有一点未来信息），或者下根bar开盘价/TWAP/VWAP
     def __init__(self, inexclude, score=None, hold_num=None, market=None, price='close', interval=1):
         self.inexclude = inexclude
         self.score = score
         self.hold_num = hold_num
         self.market = market
         self.price = price
         self.interval = interval
+    # 为market添加cash品种
+    def add_cash(self):
+        cash = pd.DataFrame(index=self.market.index.get_level_values(0).unique())
+        cash['code']  = 'cash'
+        cash['name'] = '现金'
+        cash[self.price] = 1
+        cash = cash.reset_index().set_index(['date', 'code'])
+        self.market = pd.concat([self.market, cash]).sort_values('date')
     # 获得持仓表(持仓张数)
     def get_hold(self):
         # 按列表持股
         if type(self.inexclude)==list:
-            if 'cash' in (self.inexclude): 
-                cash = pd.DataFrame(index=self.market.index.get_level_values(0).unique())
-                cash['code']  = 'cash'
-                cash['name'] = '现金'
-                cash[self.price] = 1
-                cash = cash.reset_index().set_index(['date', 'code'])
-                self.market = pd.concat([self.market, cash]).sort_values('date') 
+            if 'cash' in (self.inexclude):
+                self.add_cash()
             df_hold = self.market.loc[:, self.inexclude, :]
         # 按排除、排序规则持股
         else:
             keeppool_rank = (lambda x: self.market[self.market[x[0]]] if x[0] \
                                 else self.market[~self.market[x[1]]])(self.inexclude)[self.score].\
                                     groupby('date').rank(ascending=False, pct=(self.hold_num<1))
-            df_hold = self.market.loc[keeppool_rank[keeppool_rank<=self.hold_num].index]
-        # 等权（每只股票买一块钱）
-        self.df_hold = (1/df_hold[self.price].unstack()).fillna(0)
+            df_hold = self.market.loc[keeppool_rank[keeppool_rank<=self.hold_num].index].copy()
+            # 检查有无空仓情形，如果有的话就添加现金
+            lost_bars = list(set(self.market.index.get_level_values(0))-set(df_hold.index.get_level_values(0)))
+            if lost_bars!=[]:
+                self.add_cash()
+                df_hold = pd.concat([self.market.loc[lost_bars, 'cash', :], df_hold])
+        # 等权（总账户市值1块钱）
+        df_hold = (1/df_hold[self.price].unstack()).fillna(0)
+        df_hold = df_hold.apply(lambda x: x/(x!=0).sum(), axis=1)
+        # 去掉一直持仓为0的品种
+        always_not_hold = (df_hold==0).all()
+        self.df_hold = df_hold[always_not_hold[~always_not_hold].index].copy()
     # 调仓间隔不为1时，需考虑调仓问题
     def get_interval(self):
         if self.interval!=1:
             # 以interval为周期 调整持仓的持仓表
             # 选取的index  interval = 3  0,0,0,3,3,3,6...
             take_hold = [self.df_hold.index[int(i/self.interval)*self.interval]\
                                 for i in range(len(self.df_hold.index))]
             real_hold = self.df_hold.loc[take_hold].copy()
             ## 提取的index非连续，复原到原来的连续交易日index
             real_hold.index = self.df_hold.index
-            self.df_hold = real_hold
-
-            #index_date = self.df_hold.index.get_level_values(0).unique()
-            #index_select = {index_date[i]:index_date[i-i%self.interval] for i in range(len(index_date))}
-            #result = [] 
-            #for k,v in index_select.items():
-            #    df = self.df_hold.loc[v].copy()
-            #    df['date'] = k
-            #    result.append(df.reset_index())
-            #self.df_hold = pd.concat(result).sort_values(by='date').set_index(['date', 'code'])
+            # 去掉一直持仓为0的品种
+            always_not_hold = (real_hold==0).all()
+            self.df_hold = real_hold[always_not_hold[~always_not_hold].index].copy()
     # 运行策略
     def run(self):
         self.get_hold()
         self.get_interval()
-        df_price = pd.DataFrame(self.market[self.price]).pivot_table(self.price, 'date' ,'code')
+        # 判断cash是否在持仓，如果在的话避免price没有cash列
+        if 'cash' in self.df_hold.columns:
+            self.add_cash()
+        # 价格矩阵，去掉全是0的列
+        self.df_price = pd.DataFrame(self.market[self.price]).\
+            pivot_table(self.price, 'date' ,'code')[self.df_hold.columns].copy()
+        # 货值矩阵
+        self.df_amount = (self.df_hold*self.df_price).fillna(0)
         # 权重矩阵
-        df_weight = (self.df_hold*df_price).fillna(0)
-        self.df_weight = (df_weight.apply(lambda x: (x/x.sum()).fillna(0), axis=1))
+        self.df_weight = (self.df_amount.apply(lambda x: (x/x.sum()).fillna(0), axis=1))
         # 净值贡献矩阵
-        returns = (df_price/df_price.shift() - 1).fillna(0)
+        returns = (self.df_price/self.df_price.shift() - 1).fillna(0)
         self.df_contri = (self.df_weight.shift()*returns).fillna(0)
         self.returns = self.df_contri.sum(axis=1)    
+        # 交易金额
+        delta_hold = self.df_hold-self.df_hold.shift().fillna(0)
+        self.delta_amount = (delta_hold*self.df_price).fillna(0)
+        self.turnover = abs(self.delta_amount.drop(columns='cash').sum(axis=1))/self.df_amount.sum(axis=1)
+
 
 
 # 组合策略、择时策略
 # 根据择时条件选择陪着不同的择股策略
 # conds = [满足条件0的交易日（index或lsit），满足条件1的交易日, ..., 满足条件n的交易日]
 # strats =[条件0对应策略0（MetaStrat）,   非条件0且条件1对应策略1, ... , 非条件0到条件n-1且条件n对应策略n， 剩余时间执行条件n+1]
 class ComboStrat(MetaStrat):
@@ -121,42 +141,19 @@
             strati = self.strats[i]
             strati.market = self.market.loc[stat_days[i]]
             strati.price = self.price
             print('状态%s交易日：'%i, len(stat_days[i]))
             strati.get_hold()
             df_holds.append(strati.df_hold)
         self.df_hold = pd.concat(df_holds).sort_values(by='date').fillna(0)
-#    def get_interval(self):
-#        if self.interval!=1:
-#            index_date = self.df_hold.index.get_level_values(0).unique()
-#            index_select = {index_date[i]:index_date[i-i%self.interval] for i in range(len(index_date))}
-#            result = [] 
-#            for k,v in index_select.items():
-#                df = self.df_hold.loc[v].copy()
-#                df['date'] = k
-#                result.append(df.reset_index())
-#            self.df_hold = pd.concat(result).sort_values(by='date').set_index(['date', 'code'])
-#    def run(self):
-#        self.get_hold()
-#        self.get_interval()
-#        df_price = pd.DataFrame(self.market[self.price]).pivot_table(self.price, 'date' ,'code')
-#        # 权重矩阵
-#        df_weight = (self.df_hold*df_price).fillna(0)
-#        self.df_weight = (df_weight.apply(lambda x: (x/x.sum()).fillna(0), axis=1))
-#        # 净值贡献矩阵
-#        returns = (df_price/df_price.shift() - 1).fillna(0)
-#        self.df_contri = (self.df_weight.shift()*returns).fillna(0)
-#        self.returns = self.df_contri.sum(axis=1)
-
-
-
 
 
 
 
+'''
 #===========================  选股策略  ===================================
 # market, multiindex(date, code) 必须列为 'bool', 'score', ‘next_return'
 def ChooseSecurities(market, strat0):
     # 添加保证金账户（空仓）
     def add_deposit(market):
         deposit = pd.DataFrame(index=market.index.get_level_values(0).unique())
         deposit['code']  = 'deposit'
@@ -219,15 +216,15 @@
         df_holdi = ChooseSecurities(market_stati, strati) 
         df_holds.append(df_holdi)
     return pd.concat(df_holds).sort_values(by='date')
 
 
 
 ###########
-
+'''
```

### Comparing `FreeBack-4.5.6a0/FreeBack.egg-info/PKG-INFO` & `FreeBack-4.6.1a0/FreeBack.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeBack
-Version: 4.5.6a0
+Version: 4.6.1a0
 Summary: Package for backtest
 Home-page: https://github.com/LHanLi/FreeBack
 Author: LH.Li,zzq
 Author-email: lh98lee@zju.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `FreeBack-4.5.6a0/LICENSE` & `FreeBack-4.6.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `FreeBack-4.5.6a0/PKG-INFO` & `FreeBack-4.6.1a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeBack
-Version: 4.5.6a0
+Version: 4.6.1a0
 Summary: Package for backtest
 Home-page: https://github.com/LHanLi/FreeBack
 Author: LH.Li,zzq
 Author-email: lh98lee@zju.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `FreeBack-4.5.6a0/README.md` & `FreeBack-4.6.1a0/README.md`

 * *Files identical despite different names*

### Comparing `FreeBack-4.5.6a0/setup.py` & `FreeBack-4.6.1a0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 setup(
     name="FreeBack",
     # 版本号: 第几次模块增加，第几次函数增加，第几次函数功能修改
     # (每次高级别序号增加后,低级别序号归0)
     # alpha为调试版,beta为测试版,stable为稳定版 
-    version="4.5.6-alpha",
+    version="4.6.1-alpha",
     author="LH.Li,zzq",
     author_email="lh98lee@zju.edu.cn",  
     description='Package for backtest',
     long_description=long_description, 
     # 描述文件为md格式
     long_description_content_type="text/markdown",
     url="https://github.com/LHanLi/FreeBack",
@@ -22,14 +22,15 @@
         'pandas',
         'scipy',
         'statsmodels',
         'seaborn',
         'plottable',
         'pyecharts',
         'numpy_ext',
+        'xlsxwriter'
     ],
     classifiers=[
          # 该软件包仅与Python3兼容
         "Programming Language :: Python :: 3",
         # 根据GPL 3.0许可证开源
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         # 与操作系统无关
```

