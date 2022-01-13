[toc]
# Visualizing-Oracle-Performance-Data-By-Graph

I finished a project about how to visualize oracle performance by graph in recent two months (2021.11 - 2021.12).

### 1. Introduction - What's VOPDBG ?

In this section I'll share something with you about the introduction about **visualizing oracle performance data by graph**. Yes, as well-known as, `VOPDBG` is the combination of the first letter abbreviation for **V**isualizing **O**racle **P**erformance **D**ata **B**y **G**raph.

### 2. Oracle Performance Metrics

Here we primarily concentrate visualizeng the following `oracle performance metrics`.

- `ASPAC` (**A**ctive **S**essions **P**er **A**ctivity **C**lass)
   - [acquire_aspac.sql](https://github.com/guestart/Oracle-SQL-Scripts/blob/master/awr_trend/acquire_aspac.sql)
- `ASPWC` (**A**ctive **S**essions **P**er **W**ait **C**lass)
   - [acquire_aspwc.sql](https://github.com/guestart/Oracle-SQL-Scripts/blob/master/awr_trend/acquire_aspwc.sql)
- `AAS` (**A**verage **A**ctive **S**essions)
   - [acquire_aas_2.sql](https://github.com/guestart/Oracle-SQL-Scripts/blob/master/awr_trend/acquire_aas_2.sql)
- `AASLC` (**A**verage **A**ctive **S**essions & **L**ogic **C**PUs)
   - [acquire_logic_cpus_union_aas.sql](https://github.com/guestart/Oracle-SQL-Scripts/blob/master/awr_trend/acquire_logic_cpus_union_aas.sql)
- `ARP` (**A**verage **R**unnable **P**rocesses)
   - [acquire_arp.sql](https://github.com/guestart/Oracle-SQL-Scripts/blob/master/awr_trend/acquire_arp.sql)
   - [acquire_arp_2.sql](https://github.com/guestart/Oracle-SQL-Scripts/blob/master/awr_trend/acquire_arp_2.sql)
- `CLC` (**C**urrent **L**ogons **C**ount)
   - [acquire_clc.sql](https://github.com/guestart/Oracle-SQL-Scripts/blob/master/awr_trend/acquire_clc.sql)
- `COL` (**C**urrent **O**S **L**oad)
   - [acquire_col.sql](https://github.com/guestart/Oracle-SQL-Scripts/blob/master/awr_trend/acquire_col.sql)
- `DT` (**D**B **T**ime)
   - [acquire_dbtime.sql](https://github.com/guestart/Oracle-SQL-Scripts/blob/master/awr_trend/acquire_dbtime.sql)
- `LFSSBR` (**L**atency **F**or **S**ynchronous **S**ingle **B**lock **R**eads)
   - [acquire_assbrl.sql](https://github.com/guestart/Oracle-SQL-Scripts/blob/master/awr_trend/acquire_assbrl.sql)
- `PRPWRS` (**P**hysical **R**eads and **P**hysical **W**rites and **R**edo **S**ize)
   - [acquire_prps_union_pwps_union_rsps.sql](https://github.com/guestart/Oracle-SQL-Scripts/blob/master/awr_trend/acquire_prps_union_pwps_union_rsps.sql)
- `TPRTPWTI` (**T**otal **P**hysical **R**eads and **T**otal **P**hysical **W**rites and **T**otal **I**O)
- `UTPSLPS` (**U**ser **T**ransaction **P**er **S**econd and **L**ogons **P**er **S**econd)
   - [acquire_lps_union_tps.sql](https://github.com/guestart/Oracle-SQL-Scripts/blob/master/awr_trend/acquire_lps_union_tps.sql)

### 3. How To Visualize Oracle Performance Data ?

Fortunately Oracle SQL Develooper offers a very cool function that is called **User Defined Reports** on **Reports** label tab (you can find it by clicking `Reorts` on the `View` menu). Or taking a look at the three steps as below:

![user_defined_reports_1.png](https://github.com/guestart/Visualizing-Oracle-Performance-Data-By-Graph/blob/main/user_defined_reports_1.png)

![user_defined_reports_2.png](https://github.com/guestart/Visualizing-Oracle-Performance-Data-By-Graph/blob/main/user_defined_reports_2.png)

![user_defined_reports_3.png](https://github.com/guestart/Visualizing-Oracle-Performance-Data-By-Graph/blob/main/user_defined_reports_3.png)

We can use the **User Defined Reports** to visualize oracle performance metrics mentioned previously in the **section 2**.

### 4. Using cool XML files to generate User Defined Reports of Oracle SQL Developer

You can directly download these [XML files](https://github.com/guestart/Oracle-SQL-Scripts/tree/master/XML_Reports) to your laptop and then choose **Open Report** by right-clicking the entry **User Defined Reports** in the Reports label tab of Oracle SQL Developer, next to choose a XML file that has already been saved to your computer, until you finished adding all of XML files using similar approach. Ultimately the oracle performance metrics have been shown on Reports label tab of Oracle SQL Developer, such as the following screenshot:

![user_defined_reports_4.png](https://github.com/guestart/Visualizing-Oracle-Performance-Data-By-Graph/blob/main/user_defined_reports_4.png)

### 5. Relevant Blog Posts

On one hand I've also published a series of relevant blog posts on [modb.pro](https://www.modb.pro/), they're listed in chronological order as below:

- [Visualizing the Oracle Perfornance Graph by Average Active Sessions](https://www.modb.pro/db/158813) - Chinese
- [Visualizing the Oracle Performance Graph by Average Active Sessions & Logic CPUs](https://www.modb.pro/db/160390) - Chinese
- [Visualizing the Oracle Performance Graph by Average Runnable Processes](https://www.modb.pro/db/172906) - Chinese
- [Visualizing the Oracle Performance Graph by Active Sessions Per Activity Class](https://www.modb.pro/db/181155) - Chinese
- [Visualizing the Oracle Performance Graph by Active Sessions Per Wait Class](https://www.modb.pro/db/188688)

On the other hand you're able to find the previous list as well from [here](https://quanwenzhao.wordpress.com/2022/01/04/the-catalogue-of-visualizing-performance-data/).

### 6. License

This repository complies with the License of [GNU General Public License v2.0](https://github.com/guestart/Visualizing-Oracle-Performance-Data-By-Graph/blob/main/LICENSE), if you copy or forward it please consent all of the content of this protocol.
