<h1>Building and Validating DNN Models for
Forecasting the Quality of Cloud Services</h1></div>

* * *
This repository manages the files used in the empirical study of the paper:
_**Building and Validating DNN Models for
Forecasting the Quality of Cloud Servicest**_
* * *


The following section presents the results obtained for the 16 variables used to develop the experiment, as well as additional information related to them.

## Index {#Home}
1. [Dataset](#datos)
2. [Jupiter Notebook](#notebook)
3. [BI-GRU Accuracy Metrics](#MetricBiGru)
4. [LSTM Accuracy Metrics](#Metric)
5. [BI-GRU model predictions](#BiGru)
6. [LSTM model predictions](#LSTM)
7. [ARIMA model predictions](#ARIMA)
8. [AUTO ARIMA model predictions](#AUTOARIMA) 


## 1. Datasets {#Datos}
Representation of the **_datasets_**  with the observations of 16 QoS metrics extracted from the cloud service SAlert monitoring.

- <a href ="./experiment/data (1).csv">  Data source </a>


| Variable            | Dataset                                                                  |
|---------------------|----------------------------------------------------------------------------|
| Free Memory         | ![FreeMemory_data.jpg](imgs/dataset/FreeMemory_data.jpg)               |
| Used Memory         | ![UsedMemory_data.jpg](imgs/dataset/UsedMemory_data.jpg)               |
| Free Disk           | ![Free Disk_dataset.png](imgs/dataset/FreeDisk_data.jpg)                   |
| Used Disk           | ![Used Disk_dataset.png](imgs/dataset/UsedDisk_data.jpg)                   |
| Disk read/s         | ![Disk read_s_dataset.png](imgs/dataset/Diskreads_data.jpg)               |
| Disk write/s        | ![Disk write_s_dataset.png](imgs/dataset/Diskwrites_data.jpg)             |
| NetBytes In         | ![NetBytes In_dataset.png](imgs/dataset/NetBytesIn_data.jpg)               |
| NetBytes Out        | ![NetBytes Out_dataset.png](imgs/dataset/NetBytesOut_data.jpg)             |
| NetPackets In       | ![NetPackets In_dataset.png](imgs/dataset/NetPacketsIn_data.jpg)           |
| NetPackets Out      |  ![NetPackets Out_dataset.png](imgs/dataset/NetPacketsOut_data.jpg)          |
| Rx packets          | ![Rx packets_dataset.png](imgs/dataset/Rxpackets_data.jpg)                 |
| Tx packets          | ![Tx packets_dataset.png](imgs/dataset/Txpackets_data.jpg)                 |
| CPU percent         | ![MemoryUsedpercent_dataset.png](imgs/dataset/CPUpercent_data.jpg)         |
| Memory Used percent | ![Used Memory_dataset.png](imgs/dataset/MemoryUsedpercent_data.jpg)       |
| Disk Used percent   | ![Disk Used percent_dataset.png](imgs/dataset/DiskUsedpercent_data.jpg) |
| Uptime              | ![Uptime_dataset.png](imgs/dataset/Uptime_data.jpg)                     |

[Index](#Home)

## 2. Jupiter Notebook {#notebook}
The notebook is available on the link, and the directories required for execution are detailed on the readme.txt file

<p align="center">
    <a href="./experiment/BiGru_bi_univariado_uni_experiment_v6.ipynb">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
    </a>
</p>

The statistics used are available on the link <a href ="./experiment/CAIN v4.xlsx">  Model statistics </a>

[Index](#Home)

## 3. BI-GRU Accuracy Metrics {#MetricBiGru}
BI-GRU model performance evaluation using accuracy metrics **_RMSE, MAE, MAPE_** 

| Variable            | RMSE                                                                     | MAE                                                                     | MAPE                                                                     | 
|---------------------|--------------------------------------------------------------------------|-------------------------------------------------------------------------|--------------------------------------------------------------------------|
| **_Free Memory_**        
Iteration 1| ![Free Memory_mrse.png](imgs/BiGru/metrics/iteration_0_Free%20Memory_rmse.png)                   | ![Free Memory_mae.png](imgs/BiGru/metrics/Iteration_0_Free%20Memory_mae.png)                    | ![Free Memory_mape.png](imgs/BiGru/metrics/iteration_0_Free%20Memory_mape.png)                   | 
|Iteration 2         | ![Free Memory_mrse.png](imgs/BiGru/metrics/iteration_1_Free%20Memory_rmse.png)                   | ![Free Memory_mae.png](imgs/BiGru/metrics/Iteration_1_Free%20Memory_mae.png)                    | ![Free Memory_mape.png](imgs/BiGru/metrics/iteration_1_Free%20Memory_mape.png)                   | 
| Iteration 3        | ![Free Memory_mrse.png](imgs/BiGru/metrics/iteration_2_Free%20Memory_rmse.png)                   | ![Free Memory_mae.png](imgs/BiGru/metrics/Iteration_2_Free%20Memory_mae.png)                    | ![Free Memory_mape.png](imgs/BiGru/metrics/iteration_2_Free%20Memory_mape.png)                   | 
| **_Used Memory_**         
Iteration 1| ![Used Memory_rsme.png](imgs/BiGru/metrics/iteration_0_Used%20Memory_rmse.png)                   | ![Used Memory_mae.png](imgs/BiGru/metrics/Iteration_0_Used%20Memory_mae.png)                    | ![Used Memory_mape.png](imgs/BiGru/metrics/iteration_0_Used%20Memory_mape.png) | 
| Iteration 2         | ![Used Memory_rsme.png](imgs/BiGru/metrics/iteration_1_Used%20Memory_rmse.png)                   | ![Used Memory_mae.png](imgs/BiGru/metrics/Iteration_1_Used%20Memory_mae.png)                    | ![Used Memory_mape.png](imgs/BiGru/metrics/iteration_1_Used%20Memory_mape.png) | 
| Iteration 3         | ![Used Memory_rsme.png](imgs/BiGru/metrics/iteration_2_Used%20Memory_rmse.png)                   | ![Used Memory_mae.png](imgs/BiGru/metrics/Iteration_2_Used%20Memory_mae.png)   | ![Used Memory_mape.png](imgs/BiGru/metrics/iteration_2_Used%20Memory_mape.png)          | 
| **_Free Disk_**           
Iteration 1| ![FreeDisk_rsme.png](imgs/BiGru/metrics/iteration_0_Free%20Disk_rmse.png) |  ![FreeDisk_mae.png](imgs/BiGru/metrics/Iteration_0_Free%20Disk_mae.png)|        ![FreeDisk_mape.png](imgs/BiGru/metrics/iteration_0_Free%20Disk_mape.png) | 
|Iteration 2| ![FreeDisk_rsme.png](imgs/BiGru/metrics/iteration_1_Free%20Disk_rmse.png) |  ![FreeDisk_mae.png](imgs/BiGru/metrics/Iteration_1_Free%20Disk_mae.png)|        ![FreeDisk_mape.png](imgs/BiGru/metrics/iteration_1_Free%20Disk_mape.png) | 
|Iteration 3| ![FreeDisk_rsme.png](imgs/BiGru/metrics/iteration_2_Free%20Disk_rmse.png) |  ![FreeDisk_mae.png](imgs/BiGru/metrics/Iteration_2_Free%20Disk_mae.png)|        ![FreeDisk_mape.png](imgs/BiGru/metrics/iteration_2_Free%20Disk_mape.png) | 
| **_Used Disk_**
Iteration 1| ![Used Disk_rmse.png](imgs/BiGru/metrics/iteration_0_Used%20Disk_rmse.png) | ![Used Disk_mae.png](imgs/BiGru/metrics/Iteration_0_Used%20Disk_mae.png) | ![Used Disk_mape.png](imgs/BiGru/metrics/iteration_0_Used%20Disk_mape.png) | 
|Iteration 2| ![Used Disk_rmse.png](imgs/BiGru/metrics/iteration_1_Used%20Disk_rmse.png) | ![Used Disk_mae.png](imgs/BiGru/metrics/Iteration_1_Used%20Disk_mae.png) | ![Used Disk_mape.png](imgs/BiGru/metrics/iteration_1_Used%20Disk_mape.png) | 
|Iteration 3| ![Used Disk_rmse.png](imgs/BiGru/metrics/iteration_2_Used%20Disk_rmse.png) | ![Used Disk_mae.png](imgs/BiGru/metrics/Iteration_2_Used%20Disk_mae.png) | ![Used Disk_mape.png](imgs/BiGru/metrics/iteration_2_Used%20Disk_mape.png) | 
| **_Disk read/s_**
Iteration 1|![Disk_read_s_rmse.png](imgs/BiGru/metrics/iteration_0_Disk%20read_s_rmse.png) | 	![Disk_read_s_mae.png](imgs/BiGru/metrics/Iteration_0_Disk%20read_s_mae.png) | 	![Disk_read_s_mape.png](imgs/BiGru/metrics/iteration_0_Disk%20read_s_mape.png) | 
|Iteration 2|![Disk_read_s_rmse.png](imgs/BiGru/metrics/iteration_1_Disk%20read_s_rmse.png) | 	![Disk_read_s_mae.png](imgs/BiGru/metrics/Iteration_1_Disk%20read_s_mae.png) | 	![Disk_read_s_mape.png](imgs/BiGru/metrics/iteration_1_Disk%20read_s_mape.png) | 
|Iteration 3|![Disk_read_s_rmse.png](imgs/BiGru/metrics/iteration_2_Disk%20read_s_rmse.png) | 	![Disk_read_s_mae.png](imgs/BiGru/metrics/Iteration_2_Disk%20read_s_mae.png) | 	![Disk_read_s_mape.png](imgs/BiGru/metrics/iteration_2_Disk%20read_s_mape.png) | 
| **_Disk write/s_**
Iteration 1|![Disk write_s_rmse.png](imgs/BiGru/metrics/iteration_0_Disk%20write_s_rmse.png) | 	![Disk write_s_mae.png](imgs/BiGru/metrics/Iteration_0_Disk%20write_s_mae.png) | 	![Disk write_s_mape.png](imgs/BiGru/metrics/iteration_0_Disk%20write_s_mape.png) | 
|Iteration 2|![Disk write_s_rmse.png](imgs/BiGru/metrics/iteration_1_Disk%20write_s_rmse.png) | 	![Disk write_s_mae.png](imgs/BiGru/metrics/Iteration_1_Disk%20write_s_mae.png) | 	![Disk write_s_mape.png](imgs/BiGru/metrics/iteration_1_Disk%20write_s_mape.png) | 
|Iteration 3|![Disk write_s_rmse.png](imgs/BiGru/metrics/iteration_2_Disk%20write_s_rmse.png) | 	![Disk write_s_mae.png](imgs/BiGru/metrics/Iteration_2_Disk%20write_s_mae.png) | 	![Disk write_s_mape.png](imgs/BiGru/metrics/iteration_2_Disk%20write_s_mape.png) | 
| **_NetBytes In_**     
Iteration 1| ![NetBytes In_rmse.png](imgs/BiGru/metrics/iteration_0_NetBytes%20In_rmse.png) | 	![NetBytes In_mae.png](imgs/BiGru/metrics/Iteration_0_NetBytes%20In_mae.png) | 	![NetBytes In_mape.png](imgs/BiGru/metrics/iteration_0_NetBytes%20In_mape.png) | 
|Iteration 2| ![NetBytes In_rmse.png](imgs/BiGru/metrics/iteration_1_NetBytes%20In_rmse.png) | 	![NetBytes In_mae.png](imgs/BiGru/metrics/Iteration_1_NetBytes%20In_mae.png) | 	![NetBytes In_mape.png](imgs/BiGru/metrics/iteration_1_NetBytes%20In_mape.png) | 
|Iteration 3| ![NetBytes In_rmse.png](imgs/BiGru/metrics/iteration_2_NetBytes%20In_rmse.png) | 	![NetBytes In_mae.png](imgs/BiGru/metrics/Iteration_2_NetBytes%20In_mae.png) | 	![NetBytes In_mape.png](imgs/BiGru/metrics/iteration_2_NetBytes%20In_mape.png) | 
| **_NetBytes Out_**  
Iteration 1 |![NetBytes Out_rmse.png](imgs/BiGru/metrics/iteration_0_NetBytes%20Out_rmse.png) | 	![NetBytes Out_mae.png](imgs/BiGru/metrics/Iteration_0_NetBytes%20Out_mae.png) | 	![NetBytes Out_mape.png](imgs/BiGru/metrics/iteration_0_NetBytes%20Out_mape.png) | 
|Iteration 2 | ![NetBytes Out_rmse.png](imgs/BiGru/metrics/iteration_1_NetBytes%20Out_rmse.png) | 	![NetBytes Out_mae.png](imgs/BiGru/metrics/Iteration_1_NetBytes%20Out_mae.png) | 	![NetBytes Out_mape.png](imgs/BiGru/metrics/iteration_1_NetBytes%20Out_mape.png) |
|Iteration 3 | ![NetBytes Out_rmse.png](imgs/BiGru/metrics/iteration_2_NetBytes%20Out_rmse.png) | 	![NetBytes Out_mae.png](imgs/BiGru/metrics/Iteration_2_NetBytes%20Out_mae.png) | 	![NetBytes Out_mape.png](imgs/BiGru/metrics/iteration_2_NetBytes%20Out_mape.png) |
| **_NetPackets In_**   
Iteration 1| ![NetPackets In_rmse.png](imgs/BiGru/metrics/iteration_0_NetPackets%20In_rmse.png) | 	![NetPackets In_mae.png](imgs/BiGru/metrics/Iteration_0_NetPackets%20In_mae.png) | 	![NetPackets In_mape.png](imgs/BiGru/metrics/iteration_0_NetPackets%20In_mape.png) | 
|Iteration 2| ![NetPackets In_rmse.png](imgs/BiGru/metrics/iteration_1_NetPackets%20In_rmse.png) | 	![NetPackets In_mae.png](imgs/BiGru/metrics/Iteration_1_NetPackets%20In_mae.png) | 	![NetPackets In_mape.png](imgs/BiGru/metrics/iteration_1_NetPackets%20In_mape.png) | 
|Iteration 3| ![NetPackets In_rmse.png](imgs/BiGru/metrics/iteration_2_NetPackets%20In_rmse.png) | 	![NetPackets In_mae.png](imgs/BiGru/metrics/Iteration_2_NetPackets%20In_mae.png) | 	![NetPackets In_mape.png](imgs/BiGru/metrics/iteration_2_NetPackets%20In_mape.png) | 
| **_NetPackets Out_**   
Iteration 1|![NetPackets Out_rmse.png](imgs/BiGru/metrics/iteration_0_NetPackets%20Out_rmse.png) | 	![NetPackets Out_mae.png](imgs/BiGru/metrics/Iteration_0_NetPackets%20Out_mae.png) | ![NetPackets Out_mape.png](imgs/BiGru/metrics/iteration_0_NetPackets%20Out_mape.png) | 
|Iteration 2|![NetPackets Out_rmse.png](imgs/BiGru/metrics/iteration_1_NetPackets%20Out_rmse.png) | 	![NetPackets Out_mae.png](imgs/BiGru/metrics/Iteration_1_NetPackets%20Out_mae.png) | ![NetPackets Out_mape.png](imgs/BiGru/metrics/iteration_1_NetPackets%20Out_mape.png) | 
| Iteration 3|![NetPackets Out_rmse.png](imgs/BiGru/metrics/iteration_2_NetPackets%20Out_rmse.png) | 	![NetPackets Out_mae.png](imgs/BiGruu/metrics/Iteration_2_NetPackets%20Out_mae.png) | ![NetPackets Out_mape.png](imgs/BiGru/metrics/iteration_2_NetPackets%20Out_mape.png) |     
| **_Rx packets_**    
Iteration 1|![Rx packets_rmse.png](imgs/BiGru/metrics/iteration_0_Rx%20packets_rmse.png) | 	![Rx packets_mae.png](imgs/BiGru/metrics/Iteration_0_Rx%20packets_mae.png) | 	![Rx packets_mape.png](imgs/BiGru/metrics/iteration_0_Rx%20packets_mape.png) | 
|Iteration 2|![Rx packets_rmse.png](imgs/BiGru/metrics/iteration_1_Rx%20packets_rmse.png) | 	![Rx packets_mae.png](imgs/BiGru/metrics/Iteration_1_Rx%20packets_mae.png) | 	![Rx packets_mape.png](imgs/BiGru/metrics/iteration_1_Rx%20packets_mape.png) | 
|Iteration 3|![Rx packets_rmse.png](imgs/BiGruu/metrics/iteration_2_Rx%20packets_rmse.png) | 	![Rx packets_mae.png](imgs/BiGru/metrics/Iteration_2_Rx%20packets_mae.png) | 	![Rx packets_mape.png](imgs/BiGru/metrics/iteration_2_Rx%20packets_mape.png) | 
| **_Tx packets_**         
Iteration 1 |![Tx packets_rmse.png](imgs/BiGru/metrics/iteration_0_Tx%20packets_rmse.png) | 	![Tx packets_mae.png](imgs/BiGru/metrics/Iteration_0_Tx%20packets_mae.png) | 	![Tx packets_mape.png](imgs/BiGru/metrics/iteration_0_Tx%20packets_mape.png) | 
|Iteration 2 |![Tx packets_rmse.png](imgs/BiGru/metrics/iteration_1_Tx%20packets_rmse.png) | 	![Tx packets_mae.png](imgs/BiGru/metrics/Iteration_1_Tx%20packets_mae.png) | 	![Tx packets_mape.png](imgs/BiGru/metrics/iteration_1_Tx%20packets_mape.png) | 
|Iteration 3 |![Tx packets_rmse.png](imgs/BiGru/metrics/iteration_2_Tx%20packets_rmse.png) | 	![Tx packets_mae.png](imgs/BiGru/metrics/Iteration_2_Tx%20packets_mae.png) | 	![Tx packets_mape.png](imgs/BiGru/metrics/iteration_2_Tx%20packets_mape.png) | 
| **_CPU percent_**
Iteration 1| ![CPU percent_mrse.png](imgs/BiGru/metrics/iteration_0_CPU%20percent_rmse.png)                   | ![CPU percent_mae.png](imgs/BiGru/metrics/Iteration_0_CPU%20percent_mae.png)                    | ![CPU percent_mape.png](imgs/BiGru/metrics/iteration_0_CPU%20percent_mape.png) | 
|Iteration 2         | ![CPU percent_mrse.png](imgs/BiGru/metrics/iteration_1_CPU%20percent_rmse.png)                   | ![CPU percent_mae.png](imgs/BiGru/metrics/Iteration_1_CPU%20percent_mae.png)                    | ![CPU percent_mape.png](imgs/BiGru/metrics/iteration_1_CPU%20percent_mape.png) | 
| Iteration 3| ![CPU percent_mrse.png](imgs/BiGru/metrics/iteration_2_CPU%20percent_rmse.png)                   | ![CPU percent_mae.png](imgs/BiGru/metrics/Iteration_2_CPU%20percent_mae.png)                    | ![CPU percent_mape.png](imgs/BiGru/metrics/iteration_2_CPU%20percent_mape.png)  
| **_Memory Used percent_** 
Iteration 1 |![Memory Used percent_rmse.png](imgs/BiGru/metrics/iteration_0_Memory%20Used%20percent_rmse.png) | 	![Memory Used percent_mae.png](imgs/BiGru/metrics/Iteration_0_Memory%20Used%20percent_mae.png) | 	![Memory Used percent_mape.png](imgs/BiGru/metrics/iteration_0_Memory%20Used%20percent_mape.png) | 
|Iteration 2 |![Memory Used percent_rmse.png](imgs/BiGru/metrics/iteration_1_Memory%20Used%20percent_rmse.png) | 	![Memory Used percent_mae.png](imgs/BiGru/metrics/Iteration_1_Memory%20Used%20percent_mae.png) | 	![Memory Used percent_mape.png](imgs/BiGru/metrics/iteration_1_Memory%20Used%20percent_mape.png) |
|Iteration 3 |![Memory Used percent_rmse.png](imgs/BiGru/metrics/iteration_2_Memory%20Used%20percent_rmse.png) | 	![Memory Used percent_mae.png](imgs/BiGru/metrics/Iteration_2_Memory%20Used%20percent_mae.png) | 	![Memory Used percent_mape.png](imgs/BiGru/metrics/iteration_2_Memory%20Used%20percent_mape.png) |
| **_Disk Used percent_**  
Iteration 1 |![Disk Used percent_rmse.png](imgs/BiGru/metrics/iteration_0_Disk%20Used%20percent_rmse.png) | 	![Disk Used percent_mae.png](imgs/BiGru/metrics/Iteration_0_Disk%20Used%20percent_mae.png) | 	![Disk Used percent_mape.png](imgs/BiGru/metrics/iteration_0_Disk%20Used%20percent_mape.png) | 
Iteration 2 |![Disk Used percent_rmse.png](imgs/BiGru/metrics/iteration_1_Disk%20Used%20percent_rmse.png) | 	![Disk Used percent_mae.png](imgs/BiGru/metrics/Iteration_1_Disk%20Used%20percent_mae.png) | 	![Disk Used percent_mape.png](imgs/BiGru/metrics/iteration_1_Disk%20Used%20percent_mape.png) |
Iteration 3 |![Disk Used percent_rmse.png](imgs/BiGru/metrics/iteration_2_Disk%20Used%20percent_rmse.png) | 	![Disk Used percent_mae.png](imgs/BiGru/metrics/Iteration_2_Disk%20Used%20percent_mae.png) | 	![Disk Used percent_mape.png](imgs/BiGru/metrics/iteration_2_Disk%20Used%20percent_mape.png) |
| **_Uptime_**
Iteration 1 | ![Uptime_rmse.png](imgs/BiGru/metrics/iteration_0_Uptime_rmse.png) | 	![Uptime_mae.png](imgs/BiGru/metrics/Iteration_0_Uptime_mae.png) | 	![Uptime_mape.png](imgs/BiGru/metrics/iteration_0_Uptime_mape.png) | 
|Iteration 2 |  ![Uptime_rmse.png](imgs/BiGru/metrics/iteration_1_Uptime_rmse.png) | 	![Uptime_mae.png](imgs/BiGru/metrics/Iteration_1_Uptime_mae.png) | 	![Uptime_mape.png](imgs/BiGru/metrics/iteration_1_Uptime_mape.png) | 
|Iteration 3 |  ![Uptime_rmse.png](imgs/BiGru/metrics/iteration_2_Uptime_rmse.png) | 	![Uptime_mae.png](imgs/BiGru/metrics/Iteration_2_Uptime_mae.png) | 	![Uptime_mape.png](imgs/BiGru/metrics/iteration_2_Uptime_mape.png) | 

[Index](#Home)

## 4. LSTM Accuracy Metrics {#Metric}
LSTM model performance evaluation using accuracy metrics **_RMSE, MAE, MAPE_** 

| Variable            | RMSE                                                                     | MAE                                                                     | MAPE                                                                     | 
|---------------------|--------------------------------------------------------------------------|-------------------------------------------------------------------------|--------------------------------------------------------------------------|
| **_Free Memory_**        
Iteration 1| ![Free Memory_mrse.png](imgs/LSTM/metrics/iteration_0_Free%20Memory_rmse.png)                   | ![Free Memory_mae.png](imgs/LSTM/metrics/iteration_0_Free%20Memory_mae.png)                    | ![Free Memory_mape.png](imgs/LSTM/metrics/iteration_0_Free%20Memory_mape.png)                   | 
|Iteration 2         | ![Free Memory_mrse.png](imgs/LSTM/metrics/iteration_1_Free%20Memory_rmse.png)                   | ![Free Memory_mae.png](imgs/LSTM/metrics/iteration_1_Free%20Memory_mae.png)                    | ![Free Memory_mape.png](imgs/LSTM/metrics/iteration_1_Free%20Memory_mape.png)                   | 
| Iteration 3        | ![Free Memory_mrse.png](imgs/LSTM/metrics/iteration_2_Free%20Memory_rmse.png)                   | ![Free Memory_mae.png](imgs/LSTM/metrics/iteration_2_Free%20Memory_mae.png)                    | ![Free Memory_mape.png](imgs/LSTM/metrics/iteration_2_Free%20Memory_mape.png)                   | 
| **_Used Memory_**         
Iteration 1| ![Used Memory_rsme.png](imgs/LSTM/metrics/iteration_0_Used%20Memory_rmse.png)                   | ![Used Memory_mae.png](imgs/LSTM/metrics/iteration_0_Used%20Memory_mae.png)                    | ![Used Memory_mape.png](imgs/LSTM/metrics/iteration_0_Used%20Memory_mape.png) | 
| Iteration 2         | ![Used Memory_rsme.png](imgs/LSTM/metrics/iteration_1_Used%20Memory_rmse.png)                   | ![Used Memory_mae.png](imgs/LSTM/metrics/iteration_1_Used%20Memory_mae.png)                    | ![Used Memory_mape.png](imgs/LSTM/metrics/iteration_1_Used%20Memory_mape.png) | 
| Iteration 3         | ![Used Memory_rsme.png](imgs/LSTM/metrics/iteration_2_Used%20Memory_rmse.png)                   | ![Used Memory_mae.png](imgs/LSTM/metrics/iteration_2_Used%20Memory_mae.png)   | ![Used Memory_mape.png](imgs/LSTM/metrics/iteration_2_Used%20Memory_mape.png)          | 
| **_Free Disk_**           
Iteration 1| ![FreeDisk_rsme.png](imgs/LSTM/metrics/iteration_0_Free%20Disk_rmse.png) |  ![FreeDisk_mae.png](imgs/LSTM/metrics/iteration_0_Free%20Disk_mae.png)|        ![FreeDisk_mape.png](imgs/LSTM/metrics/iteration_0_Free%20Disk_mape.png) | 
|Iteration 2| ![FreeDisk_rsme.png](imgs/LSTM/metrics/iteration_1_Free%20Disk_rmse.png) |  ![FreeDisk_mae.png](imgs/LSTM/metrics/iteration_1_Free%20Disk_mae.png)|        ![FreeDisk_mape.png](imgs/LSTM/metrics/iteration_1_Free%20Disk_mape.png) | 
|Iteration 3| ![FreeDisk_rsme.png](imgs/LSTM/metrics/iteration_2_Free%20Disk_rmse.png) |  ![FreeDisk_mae.png](imgs/LSTM/metrics/iteration_2_Free%20Disk_mae.png)|        ![FreeDisk_mape.png](imgs/LSTM/metrics/iteration_2_Free%20Disk_mape.png) | 
| **_Used Disk_**
Iteration 1| ![Used Disk_rmse.png](imgs/LSTM/metrics/iteration_0_Used%20Disk_rmse.png) | ![Used Disk_mae.png](imgs/LSTM/metrics/iteration_0_Used%20Disk_mae.png) | ![Used Disk_mape.png](imgs/LSTM/metrics/iteration_0_Used%20Disk_mape.png) | 
|Iteration 2| ![Used Disk_rmse.png](imgs/LSTM/metrics/iteration_1_Used%20Disk_rmse.png) | ![Used Disk_mae.png](imgs/LSTM/metrics/iteration_1_Used%20Disk_mae.png) | ![Used Disk_mape.png](imgs/LSTM/metrics/iteration_1_Used%20Disk_mape.png) | 
|Iteration 3| ![Used Disk_rmse.png](imgs/LSTM/metrics/iteration_2_Used%20Disk_rmse.png) | ![Used Disk_mae.png](imgs/LSTM/metrics/iteration_2_Used%20Disk_mae.png) | ![Used Disk_mape.png](imgs/LSTM/metrics/iteration_2_Used%20Disk_mape.png) | 
| **_Disk read/s_**
Iteration 1|![Disk_read_s_rmse.png](imgs/LSTM/metrics/iteration_0_Disk%20read_s_rmse.png) | 	![Disk_read_s_mae.png](imgs/LSTM/metrics/iteration_0_Disk%20read_s_mae.png) | 	![Disk_read_s_mape.png](imgs/LSTM/metrics/iteration_0_Disk%20read_s_mape.png) | 
|Iteration 2|![Disk_read_s_rmse.png](imgs/LSTM/metrics/iteration_1_Disk%20read_s_rmse.png) | 	![Disk_read_s_mae.png](imgs/LSTM/metrics/iteration_1_Disk%20read_s_mae.png) | 	![Disk_read_s_mape.png](imgs/LSTM/metrics/iteration_1_Disk%20read_s_mape.png) | 
|Iteration 3|![Disk_read_s_rmse.png](imgs/LSTM/metrics/iteration_2_Disk%20read_s_rmse.png) | 	![Disk_read_s_mae.png](imgs/LSTM/metrics/iteration_2_Disk%20read_s_mae.png) | 	![Disk_read_s_mape.png](imgs/LSTM/metrics/iteration_2_Disk%20read_s_mape.png) | 
| **_Disk write/s_**
Iteration 1|![Disk write_s_rmse.png](imgs/LSTM/metrics/iteration_0_Disk%20write_s_rmse.png) | 	![Disk write_s_mae.png](imgs/LSTM/metrics/iteration_0_Disk%20write_s_mae.png) | 	![Disk write_s_mape.png](imgs/LSTM/metrics/iteration_0_Disk%20write_s_mape.png) | 
|Iteration 2|![Disk write_s_rmse.png](imgs/LSTM/metrics/iteration_1_Disk%20write_s_rmse.png) | 	![Disk write_s_mae.png](imgs/LSTM/metrics/iteration_1_Disk%20write_s_mae.png) | 	![Disk write_s_mape.png](imgs/LSTM/metrics/iteration_1_Disk%20write_s_mape.png) | 
|Iteration 3|![Disk write_s_rmse.png](imgs/LSTM/metrics/iteration_2_Disk%20write_s_rmse.png) | 	![Disk write_s_mae.png](imgs/LSTM/metrics/iteration_2_Disk%20write_s_mae.png) | 	![Disk write_s_mape.png](imgs/LSTM/metrics/iteration_2_Disk%20write_s_mape.png) | 
| **_NetBytes In_**     
Iteration 1| ![NetBytes In_rmse.png](imgs/LSTM/metrics/iteration_0_NetBytes%20In_rmse.png) | 	![NetBytes In_mae.png](imgs/LSTM/metrics/iteration_0_NetBytes%20In_mae.png) | 	![NetBytes In_mape.png](imgs/LSTM/metrics/iteration_0_NetBytes%20In_mape.png) | 
|Iteration 2| ![NetBytes In_rmse.png](imgs/LSTM/metrics/iteration_1_NetBytes%20In_rmse.png) | 	![NetBytes In_mae.png](imgs/LSTM/metrics/iteration_1_NetBytes%20In_mae.png) | 	![NetBytes In_mape.png](imgs/LSTM/metrics/iteration_1_NetBytes%20In_mape.png) | 
|Iteration 3| ![NetBytes In_rmse.png](imgs/LSTM/metrics/iteration_2_NetBytes%20In_rmse.png) | 	![NetBytes In_mae.png](imgs/LSTM/metrics/iteration_2_NetBytes%20In_mae.png) | 	![NetBytes In_mape.png](imgs/LSTM/metrics/iteration_2_NetBytes%20In_mape.png) | 
| **_NetBytes Out_**  
Iteration 1 |![NetBytes Out_rmse.png](imgs/LSTM/metrics/iteration_0_NetBytes%20Out_rmse.png) | 	![NetBytes Out_mae.png](imgs/LSTM/metrics/iteration_0_NetBytes%20Out_mae.png) | 	![NetBytes Out_mape.png](imgs/LSTM/metrics/iteration_0_NetBytes%20Out_mape.png) | 
|Iteration 2 | ![NetBytes Out_rmse.png](imgs/LSTM/metrics/iteration_1_NetBytes%20Out_rmse.png) | 	![NetBytes Out_mae.png](imgs/LSTM/metrics/iteration_1_NetBytes%20Out_mae.png) | 	![NetBytes Out_mape.png](imgs/LSTM/metrics/iteration_1_NetBytes%20Out_mape.png) |
|Iteration 3 | ![NetBytes Out_rmse.png](imgs/LSTM/metrics/iteration_2_NetBytes%20Out_rmse.png) | 	![NetBytes Out_mae.png](imgs/LSTM/metrics/iteration_2_NetBytes%20Out_mae.png) | 	![NetBytes Out_mape.png](imgs/LSTM/metrics/iteration_2_NetBytes%20Out_mape.png) |
| **_NetPackets In_**   
Iteration 1| ![NetPackets In_rmse.png](imgs/LSTM/metrics/iteration_0_NetPackets%20In_rmse.png) | 	![NetPackets In_mae.png](imgs/LSTM/metrics/iteration_0_NetPackets%20In_mae.png) | 	![NetPackets In_mape.png](imgs/LSTM/metrics/iteration_0_NetPackets%20In_mape.png) | 
|Iteration 2| ![NetPackets In_rmse.png](imgs/LSTM/metrics/iteration_1_NetPackets%20In_rmse.png) | 	![NetPackets In_mae.png](imgs/LSTM/metrics/iteration_1_NetPackets%20In_mae.png) | 	![NetPackets In_mape.png](imgs/LSTM/metrics/iteration_1_NetPackets%20In_mape.png) | 
|Iteration 3| ![NetPackets In_rmse.png](imgs/LSTM/metrics/iteration_2_NetPackets%20In_rmse.png) | 	![NetPackets In_mae.png](imgs/LSTM/metrics/iteration_2_NetPackets%20In_mae.png) | 	![NetPackets In_mape.png](imgs/LSTM/metrics/iteration_2_NetPackets%20In_mape.png) | 
| **_NetPackets Out_**   
Iteration 1|![NetPackets Out_rmse.png](imgs/LSTM/metrics/iteration_0_NetPackets%20Out_rmse.png) | 	![NetPackets Out_mae.png](imgs/LSTM/metrics/iteration_0_NetPackets%20Out_mae.png) | ![NetPackets Out_mape.png](imgs/LSTM/metrics/iteration_0_NetPackets%20Out_mape.png) | 
|Iteration 2|![NetPackets Out_rmse.png](imgs/LSTM/metrics/iteration_1_NetPackets%20Out_rmse.png) | 	![NetPackets Out_mae.png](imgs/LSTM/metrics/iteration_1_NetPackets%20Out_mae.png) | ![NetPackets Out_mape.png](imgs/LSTM/metrics/iteration_1_NetPackets%20Out_mape.png) | 
| Iteration 3|![NetPackets Out_rmse.png](imgs/LSTM/metrics/iteration_2_NetPackets%20Out_rmse.png) | 	![NetPackets Out_mae.png](imgs/LSTM/metrics/iteration_2_NetPackets%20Out_mae.png) | ![NetPackets Out_mape.png](imgs/LSTM/metrics/iteration_2_NetPackets%20Out_mape.png) |     
| **_Rx packets_**    
Iteration 1|![Rx packets_rmse.png](imgs/LSTM/metrics/iteration_0_Rx%20packets_rmse.png) | 	![Rx packets_mae.png](imgs/LSTM/metrics/iteration_0_Rx%20packets_mae.png) | 	![Rx packets_mape.png](imgs/LSTM/metrics/iteration_0_Rx%20packets_mape.png) | 
|Iteration 2|![Rx packets_rmse.png](imgs/LSTM/metrics/iteration_1_Rx%20packets_rmse.png) | 	![Rx packets_mae.png](imgs/LSTM/metrics/iteration_1_Rx%20packets_mae.png) | 	![Rx packets_mape.png](imgs/LSTM/metrics/iteration_1_Rx%20packets_mape.png) | 
|Iteration 3|![Rx packets_rmse.png](imgs/LSTM/metrics/iteration_2_Rx%20packets_rmse.png) | 	![Rx packets_mae.png](imgs/LSTM/metrics/iteration_2_Rx%20packets_mae.png) | 	![Rx packets_mape.png](imgs/LSTM/metrics/iteration_2_Rx%20packets_mape.png) | 
| **_Tx packets_**         
Iteration 1 |![Tx packets_rmse.png](imgs/LSTM/metrics/iteration_0_Tx%20packets_rmse.png) | 	![Tx packets_mae.png](imgs/LSTM/metrics/iteration_0_Tx%20packets_mae.png) | 	![Tx packets_mape.png](imgs/LSTM/metrics/iteration_0_Tx%20packets_mape.png) | 
|Iteration 2 |![Tx packets_rmse.png](imgs/LSTM/metrics/iteration_1_Tx%20packets_rmse.png) | 	![Tx packets_mae.png](imgs/LSTM/metrics/iteration_1_Tx%20packets_mae.png) | 	![Tx packets_mape.png](imgs/LSTM/metrics/iteration_1_Tx%20packets_mape.png) | 
|Iteration 3 |![Tx packets_rmse.png](imgs/LSTM/metrics/iteration_2_Tx%20packets_rmse.png) | 	![Tx packets_mae.png](imgs/LSTM/metrics/iteration_2_Tx%20packets_mae.png) | 	![Tx packets_mape.png](imgs/LSTM/metrics/iteration_2_Tx%20packets_mape.png) | 
| **_CPU percent_**
Iteration 1| ![CPU percent_mrse.png](imgs/LSTM/metrics/iteration_0_CPU%20percent_rmse.png)                   | ![CPU percent_mae.png](imgs/LSTM/metrics/iteration_0_CPU%20percent_mae.png)                    | ![CPU percent_mape.png](imgs/LSTM/metrics/iteration_0_CPU%20percent_mape.png) | 
|Iteration 2         | ![CPU percent_mrse.png](imgs/LSTM/metrics/iteration_1_CPU%20percent_rmse.png)                   | ![CPU percent_mae.png](imgs/LSTM/metrics/iteration_1_CPU%20percent_mae.png)                    | ![CPU percent_mape.png](imgs/LSTM/metrics/iteration_1_CPU%20percent_mape.png) | 
| Iteration 3| ![CPU percent_mrse.png](imgs/LSTM/metrics/iteration_2_CPU%20percent_rmse.png)                   | ![CPU percent_mae.png](imgs/LSTM/metrics/iteration_2_CPU%20percent_mae.png)                    | ![CPU percent_mape.png](imgs/LSTM/metrics/iteration_2_CPU%20percent_mape.png)  
| **_Memory Used percent_** 
Iteration 1 |![Memory Used percent_rmse.png](imgs/LSTM/metrics/iteration_0_Memory%20Used%20percent_rmse.png) | 	![Memory Used percent_mae.png](imgs/LSTM/metrics/iteration_0_Memory%20Used%20percent_mae.png) | 	![Memory Used percent_mape.png](imgs/LSTM/metrics/iteration_0_Memory%20Used%20percent_mape.png) | 
|Iteration 2 |![Memory Used percent_rmse.png](imgs/LSTM/metrics/iteration_1_Memory%20Used%20percent_rmse.png) | 	![Memory Used percent_mae.png](imgs/LSTM/metrics/iteration_1_Memory%20Used%20percent_mae.png) | 	![Memory Used percent_mape.png](imgs/LSTM/metrics/iteration_1_Memory%20Used%20percent_mape.png) |
|Iteration 3 |![Memory Used percent_rmse.png](imgs/LSTM/metrics/iteration_2_Memory%20Used%20percent_rmse.png) | 	![Memory Used percent_mae.png](imgs/LSTM/metrics/iteration_2_Memory%20Used%20percent_mae.png) | 	![Memory Used percent_mape.png](imgs/LSTM/metrics/iteration_2_Memory%20Used%20percent_mape.png) |
| **_Disk Used percent_**  
Iteration 1 |![Disk Used percent_rmse.png](imgs/LSTM/metrics/iteration_0_Disk%20Used%20percent_rmse.png) | 	![Disk Used percent_mae.png](imgs/LSTM/metrics/iteration_0_Disk%20Used%20percent_mae.png) | 	![Disk Used percent_mape.png](imgs/LSTM/metrics/iteration_0_Disk%20Used%20percent_mape.png) | 
Iteration 2 |![Disk Used percent_rmse.png](imgs/LSTM/metrics/iteration_1_Disk%20Used%20percent_rmse.png) | 	![Disk Used percent_mae.png](imgs/LSTM/metrics/iteration_1_Disk%20Used%20percent_mae.png) | 	![Disk Used percent_mape.png](imgs/LSTM/metrics/iteration_1_Disk%20Used%20percent_mape.png) |
Iteration 3 |![Disk Used percent_rmse.png](imgs/LSTM/metrics/iteration_2_Disk%20Used%20percent_rmse.png) | 	![Disk Used percent_mae.png](imgs/LSTM/metrics/iteration_2_Disk%20Used%20percent_mae.png) | 	![Disk Used percent_mape.png](imgs/LSTM/metrics/iteration_2_Disk%20Used%20percent_mape.png) |
| **_Uptime_**
Iteration 1 | ![Uptime_rmse.png](imgs/LSTM/metrics/iteration_0_Uptime_rmse.png) | 	![Uptime_mae.png](imgs/LSTM/metrics/iteration_0_Uptime_mae.png) | 	![Uptime_mape.png](imgs/LSTM/metrics/iteration_0_Uptime_mape.png) | 
|Iteration 2 |  ![Uptime_rmse.png](imgs/LSTM/metrics/iteration_1_Uptime_rmse.png) | 	![Uptime_mae.png](imgs/LSTM/metrics/iteration_1_Uptime_mae.png) | 	![Uptime_mape.png](imgs/LSTM/metrics/iteration_1_Uptime_mape.png) | 
|Iteration 3 |  ![Uptime_rmse.png](imgs/LSTM/metrics/iteration_2_Uptime_rmse.png) | 	![Uptime_mae.png](imgs/LSTM/metrics/iteration_2_Uptime_mae.png) | 	![Uptime_mape.png](imgs/LSTM/metrics/iteration_2_Uptime_mape.png) | 

[Index](#Home)

## 5. BI-GRU Model Prediction {#BIGRU}
BI-GRU Model fitting with prequential cross-validation

| Variable            | Iteration 1                | Iteration 2              | Iteration 3  | 
|---------------------|-----------------------|--------------------------------------|-----------------------|
| Free Memory         |![Free Memory_test.png](imgs/BiGru/results/iteration_0_Free%20Memory_test_result.png) | 	![Free Memory_test.png](imgs/BiGru/results/iteration_1_Free%20Memory_test_result.png) | 	![Free Memory_test.png](imgs/BiGru/results/iteration_2_Free%20Memory_test_result.png)| 
| Used Memory         | ![Used Memory_test.png](imgs/BiGru/results/iteration_0_Used%20Memory_test_result.png) | 	![Used Memory_test.png](imgs/BiGru/results/iteration_1_Used%20Memory_test_result.png) | 	![Used Memory_test.png](imgs/BiGru/results/iteration_2_Used%20Memory_test_result.png)|
| Free Disk           | ![Free Disk_test.png](imgs/BiGru/results/iteration_0_Free%20Disk_test_result.png) | 	![Free Disk_test.png](imgs/BiGru/results/iteration_1_Free%20Disk_test_result.png) | 	![Free Disk_test.png](imgs/BiGru/results/iteration_2_Free%20Disk_test_result.png) |  
| Used Disk           | ![Used Disk_test.png](imgs/BiGru/results/iteration_0_Used%20Disk_test_result.png) | 	![Used Disk_test.png](imgs/BiGru/results/iteration_1_Used%20Disk_test_result.png) | 	![Used Disk_test.png](imgs/BiGru/results/iteration_2_Used%20Disk_test_result.png) | 
| Disk read/s         | ![Disk read_s_test.png](imgs/BiGru/results/iteration_0_Disk%20read_s_test_result.png) | 	![Disk read_s_test.png](imgs/BiGru/results/iteration_1_Disk%20read_s_test_result.png) | 	![Disk read_s_test.png](imgs/BiGru/results/iteration_2_Disk%20read_s_test_result.png) | 
| Disk write/s        | ![Disk write_s_test.png](imgs/BiGru/results/iteration_0_Disk%20write_s_test_result.png) | 	![Disk write_s_test.png](imgs/BiGru/results/iteration_1_Disk%20write_s_test_result.png) | 	![Disk write_s_test.png](imgs/BiGru/results/iteration_2_Disk%20write_s_test_result.png) | 
| NetBytes In   | ![NetBytes In_test.png](imgs/BiGru/results/iteration_0_NetBytes%20In_test_result.png) | 	![NetBytes In_test.png](imgs/BiGru/results/iteration_1_NetBytes%20In_test_result.png) | 	![NetBytes In_test.png](imgs/BiGru/results/iteration_2_NetBytes%20In_test_result.png)| 
| NetBytes Out        | ![NetBytes Out_test.png](imgs/BiGru/results/iteration_0_NetBytes%20Out_test_result.png) | 	![NetBytes Out_test.png](imgs/BiGru/results/iteration_1_NetBytes%20Out_test_result.png) | 	![NetBytes Out_test.png](imgs/BiGru/results/iteration_2_NetBytes%20Out_test_result.png) | 
| NetPackets In       | ![NetPackets In_test.png](imgs/BiGru/results/iteration_0_NetPackets%20In_test_result.png) | 	![NetPackets In_test.png](imgs/BiGru/results/iteration_1_NetPackets%20In_test_result.png) | 	![NetPackets In_test.png](imgs/BiGru/results/iteration_2_NetPackets%20In_test_result.png) |
| NetPackets Out      |   ![NetPackets Out_test.png](imgs/BiGru/results/iteration_0_NetPackets%20Out_test_result.png) | 	![NetPackets Out_test.png](imgs/BiGru/results/iteration_1_NetPackets%20Out_test_result.png) | 	![NetPackets Out_test.png](imgs/BiGru/results/iteration_2_NetPackets%20Out_test_result.png) | 
| Rx packets          | ![Rx packets_test.png](imgs/BiGru/results/iteration_0_Rx%20packets_test_result.png) | 	![Rx packets_test.png](imgs/BiGru/results/iteration_1_Rx%20packets_test_result.png) | 	![Rx packets_test.png](imgs/BiGru/results/iteration_2_Rx%20packets_test_result.png) | 
| Tx packets          | ![Tx packets_test.png](imgs/BiGru/results/iteration_0_Tx%20packets_test_result.png) | 	![Tx packets_test.png](imgs/BiGru/results/iteration_1_Tx%20packets_test_result.png) | 	![Tx packets_test.png](imgs/BiGru/results/iteration_2_Tx%20packets_test_result.png) | 
| CPU percent         | ![CPU percent_test.png](imgs/BiGru/results/iteration_0_CPU%20percent_test_result.png) | 	![CPU percent_test.png](imgs/BiGru/results/iteration_1_CPU%20percent_test_result.png) | 	![CPU percent_test.png](imgs/BiGru/results/iteration_2_CPU%20percent_test_result.png)| 
| Memory Used percent | ![Memory Used percent_test.png](imgs/BiGru/results/iteration_0_Memory%20Used%20percent_test_result.png) | 	![Memory Used percent_test.png](imgs/BiGru/results/iteration_1_Memory%20Used%20percent_test_result.png) | 	![Memory Used percent_test.png](imgs/BiGru/results/iteration_2_Memory%20Used%20percent_test_result.png) | 
| Disk Used percent   | ![Disk Used percent_test.png](imgs/BiGru/results/iteration_0_Disk%20Used%20percent_test_result.png) | 	![Disk Used percent_test.png](imgs/BiGru/results/iteration_1_Disk%20Used%20percent_test_result.png) | 	![Disk Used percent_test.png](imgs/BiGru/results/iteration_2_Disk%20Used%20percent_test_result.png) | 
| Uptime              | ![Uptime_test.png](imgs/BiGru/results/iteration_0_Uptime_test_result.png) | 	![Uptime_test.png](imgs/BiGru/results/iteration_1_Uptime_test_result.png) | 	![Uptime_test.png](imgs/BiGru/results/iteration_2_Uptime_test_result.png) | 

[Index](#Home)

## 6. LSTM Model Prediction {#LSTM}
LSTM Model fitting with prequential cross-validation

| Variable            | Iteration 1                | Iteration 2              | Iteration 3  | 
|---------------------|-----------------------|--------------------------------------|-----------------------|
| Free Memory         |![Free Memory_test.png](imgs/LSTM/results/iteration_0_Free%20Memory_test_result.png) | 	![Free Memory_test.png](imgs/LSTM/results/iteration_1_Free%20Memory_test_result.png) | 	![Free Memory_test.png](imgs/LSTM/results/iteration_2_Free%20Memory_test_result.png)| 
| Used Memory         | ![Used Memory_test.png](imgs/LSTM/results/iteration_0_Used%20Memory_test_result.png) | 	![Used Memory_test.png](imgs/LSTM/results/iteration_1_Used%20Memory_test_result.png) | 	![Used Memory_test.png](imgs/LSTM/results/iteration_2_Used%20Memory_test_result.png)|
| Free Disk           | ![Free Disk_test.png](imgs/LSTM/results/iteration_0_Free%20Disk_test_result.png) | 	![Free Disk_test.png](imgs/LSTM/results/iteration_1_Free%20Disk_test_result.png) | 	![Free Disk_test.png](imgs/LSTM/results/iteration_2_Free%20Disk_test_result.png) |  
| Used Disk           | ![Used Disk_test.png](imgs/LSTM/results/iteration_0_Used%20Disk_test_result.png) | 	![Used Disk_test.png](imgs/LSTM/results/iteration_1_Used%20Disk_test_result.png) | 	![Used Disk_test.png](imgs/LSTM/results/iteration_2_Used%20Disk_test_result.png) | 
| Disk read/s         | ![Disk read_s_test.png](imgs/LSTM/results/iteration_0_Disk%20read_s_test_result.png) | 	![Disk read_s_test.png](imgs/LSTM/results/iteration_1_Disk%20read_s_test_result.png) | 	![Disk read_s_test.png](imgs/LSTM/results/iteration_2_Disk%20read_s_test_result.png) | 
| Disk write/s        | ![Disk write_s_test.png](imgs/LSTM/results/iteration_0_Disk%20write_s_test_result.png) | 	![Disk write_s_test.png](imgs/LSTM/results/iteration_1_Disk%20write_s_test_result.png) | 	![Disk write_s_test.png](imgs/LSTM/results/iteration_2_Disk%20write_s_test_result.png) | 
| NetBytes In   | ![NetBytes In_test.png](imgs/LSTM/results/iteration_0_NetBytes%20In_test_result.png) | 	![NetBytes In_test.png](imgs/LSTM/results/iteration_1_NetBytes%20In_test_result.png) | 	![NetBytes In_test.png](imgs/LSTM/results/iteration_2_NetBytes%20In_test_result.png)| 
| NetBytes Out        | ![NetBytes Out_test.png](imgs/LSTM/results/iteration_0_NetBytes%20Out_test_result.png) | 	![NetBytes Out_test.png](imgs/LSTM/results/iteration_1_NetBytes%20Out_test_result.png) | 	![NetBytes Out_test.png](imgs/LSTM/results/iteration_2_NetBytes%20Out_test_result.png) | 
| NetPackets In       | ![NetPackets In_test.png](imgs/LSTM/results/iteration_0_NetPackets%20In_test_result.png) | 	![NetPackets In_test.png](imgs/LSTM/results/iteration_1_NetPackets%20In_test_result.png) | 	![NetPackets In_test.png](imgs/LSTM/results/iteration_2_NetPackets%20In_test_result.png) |
| NetPackets Out      |   ![NetPackets Out_test.png](imgs/LSTM/results/iteration_0_NetPackets%20Out_test_result.png) | 	![NetPackets Out_test.png](imgs/LSTM/results/iteration_1_NetPackets%20Out_test_result.png) | 	![NetPackets Out_test.png](imgs/LSTM/results/iteration_2_NetPackets%20Out_test_result.png) | 
| Rx packets          | ![Rx packets_test.png](imgs/LSTM/results/iteration_0_Rx%20packets_test_result.png) | 	![Rx packets_test.png](imgs/LSTM/results/iteration_1_Rx%20packets_test_result.png) | 	![Rx packets_test.png](imgs/LSTM/results/iteration_2_Rx%20packets_test_result.png) | 
| Tx packets          | ![Tx packets_test.png](imgs/LSTM/results/iteration_0_Tx%20packets_test_result.png) | 	![Tx packets_test.png](imgs/LSTM/results/iteration_1_Tx%20packets_test_result.png) | 	![Tx packets_test.png](imgs/LSTM/results/iteration_2_Tx%20packets_test_result.png) | 
| CPU percent         | ![CPU percent_test.png](imgs/LSTM/results/iteration_0_CPU%20percent_test_result.png) | 	![CPU percent_test.png](imgs/LSTM/results/iteration_1_CPU%20percent_test_result.png) | 	![CPU percent_test.png](imgs/LSTM/results/iteration_2_CPU%20percent_test_result.png)| 
| Memory Used percent | ![Memory Used percent_test.png](imgs/LSTM/results/iteration_0_Memory%20Used%20percent_test_result.png) | 	![Memory Used percent_test.png](imgs/LSTM/results/iteration_1_Memory%20Used%20percent_test_result.png) | 	![Memory Used percent_test.png](imgs/LSTM/results/iteration_2_Memory%20Used%20percent_test_result.png) | 
| Disk Used percent   | ![Disk Used percent_test.png](imgs/LSTM/results/iteration_0_Disk%20Used%20percent_test_result.png) | 	![Disk Used percent_test.png](imgs/LSTM/results/iteration_1_Disk%20Used%20percent_test_result.png) | 	![Disk Used percent_test.png](imgs/LSTM/results/iteration_2_Disk%20Used%20percent_test_result.png) | 
| Uptime              | ![Uptime_test.png](imgs/LSTM/results/iteration_0_Uptime_test_result.png) | 	![Uptime_test.png](imgs/LSTM/results/iteration_1_Uptime_test_result.png) | 	![Uptime_test.png](imgs/LSTM/results/iteration_2_Uptime_test_result.png) | 

[Index](#Home)

## 7. ARIMA Model Prediction {#ARIMA}
ARIMA Model fitting with prequential cross-validation

| Variable            | Iteration 1                | Iteration 2              | Iteration 3  | 
|---------------------|-----------------------|--------------------------------------|-----------------------|
| Free Memory         | ![FreeMemory_.png](imgs/Arima/Iteration-0_FreeMemory_test_result.png) | 	![FreeMemory_.png](imgs/Arima/Iteration-1_FreeMemory_test_result.png) | 	![FreeMemory_.png](imgs/Arima/Iteration-2_FreeMemory_test_result.png) | 
| Used Memory         | ![UsedMemory_.png](imgs/Arima/Iteration-0_UsedMemory_test_result.png) | 	![UsedMemory_.png](imgs/Arima/Iteration-1_UsedMemory_test_result.png) | 	![UsedMemory_.png](imgs/Arima/Iteration-2_UsedMemory_test_result.png) |   
| Free Disk           | ![FreeDisk_test.png](imgs/Arima/Iteration-0_FreeDisk_test_result.png) | 	![FreeDisk_test.png](imgs/Arima/Iteration-1_FreeDisk_test_result.png) | 	![FreeDisk_test.png](imgs/Arima/Iteration-2_FreeDisk_test_result.png) | 
| Used Disk           | ![UsedDisk_test.png](imgs/Arima/Iteration-0_UsedDisk_test_result.png) | 	![UsedDisk_test.png](imgs/Arima/Iteration-1_UsedDisk_test_result.png) | 	![UsedDisk_test.png](imgs/Arima/Iteration-2_UsedDisk_test_result.png) | 
| Disk read/s         | ![Diskreads_test.png](imgs/Arima/Iteration-0_Diskreads_test_result.png) | 	![Diskreads_test.png](imgs/Arima/Iteration-1_Diskreads_test_result.png) | 	![Diskreads_test.png](imgs/Arima/Iteration-2_Diskreads_test_result.png) | 
| Disk write/s        | ![Diskwrites_test.png](imgs/Arima/Iteration-0_Diskwrites_test_result.png) | 	![Diskwrites_test.png](imgs/Arima/Iteration-1_Diskwrites_test_result.png) | 	![Diskwrites_test.png](imgs/Arima/Iteration-2_Diskwrites_test_result.png) | 
| NetBytes In         | ![NetBytes In_test.png](imgs/Arima/Iteration-0_NetBytesIn_test_result.png) | 	![NetBytes In_test.png](imgs/Arima/Iteration-1_NetBytesIn_test_result.png) | 	![NetBytes In_test.png](imgs/Arima/Iteration-2_NetBytesIn_test_result.png) | 
| NetBytes Out        | ![NetBytesOut_test.png](imgs/Arima/Iteration-0_NetBytesOut_test_result.png) | 	![NetBytesOut_test.png](imgs/Arima/Iteration-1_NetBytesOut_test_result.png) | 	![NetBytesOut_test.png](imgs/Arima/Iteration-2_NetBytesOut_test_result.png) | 
| NetPackets In       | ![NetPacketsIn_test.png](imgs/Arima/Iteration-0_NetPacketsIn_test_result.png) | 	![NetPacketsIn_test.png](imgs/Arima/Iteration-1_NetPacketsIn_test_result.png) | 	![NetPacketsIn_test.png](imgs/Arima/Iteration-2_NetPacketsIn_test_result.png) | 
| NetPackets Out      |  ![NetPacketsOut_test.png](imgs/Arima/Iteration-0_NetPacketsOut_test_result.png) | 	![NetPacketsOut_test.png](imgs/Arima/Iteration-1_NetPacketsOut_test_result.png) | 	![NetPacketsOut_test.png](imgs/Arima/Iteration-2_NetPacketsOut_test_result.png) |
| Rx packets          | ![Rxpackets_test.png](imgs/Arima/Iteration-0_Rxpackets_test_result.png) | 	![Rxpackets_test.png](imgs/Arima/Iteration-1_Rxpackets_test_result.png) | 	![Rxpackets_test.png](imgs/Arima/Iteration-2_Rxpackets_test_result.png) | 
| Tx packets          | ![Txpackets_test.png](imgs/Arima/Iteration-0_Txpackets_test_result.png) | 	![Txpackets_test.png](imgs/Arima/Iteration-1_Txpackets_test_result.png) | 	![Txpackets_test.png](imgs/Arima/Iteration-2_Txpackets_test_result.png) | 
| CPU percent         | ![CPUpercent_test.png](imgs/Arima/Iteration-0_CPUpercent_test_result.png) | 	![CPUpercent_test.png](imgs/Arima/Iteration-1_CPUpercent_test_result.png) | 	![CPUpercent_test.png](imgs/Arima/Iteration-2_CPUpercent_test_result.png) | 
| Memory Used percent | ![MemoryUsedpercent_test.png](imgs/Arima/Iteration-0_MemoryUsedpercent_test_result.png) | 	![MemoryUsedpercent_test.png](imgs/Arima/Iteration-1_MemoryUsedpercent_test_result.png) | 	![MemoryUsedpercent_test.png](imgs/Arima/Iteration-2_MemoryUsedpercent_test_result.png) | 
| Disk Used percent   | ![DiskUsedpercent_test.png](imgs/Arima/Iteration-0_DiskUsedpercent_test_result.png) | 	![DiskUsedpercent_test.png](imgs/Arima/Iteration-1_DiskUsedpercent_test_result.png) | 	![DiskUsedpercent_test.png](imgs/Arima/Iteration-2_DiskUsedpercent_test_result.png) | 
| Uptime              |![Uptime_rmse.png](imgs/Arima/Iteration-0_Uptime_test_result.png) | 	![Uptime_mae.png](imgs/Arima/Iteration-1_Uptime_test_result.png) | 	![Uptime_mape.png](imgs/Arima/Iteration-2_Uptime_test_result.png) | 

[Index](#Home)



## 8. AUTOARIMA Model Prediction {#AUTOARIMA}
ARIMA Model auto fitting with prequential cross-validation

| Variable            | Iteration 1                | Iteration 2              | Iteration 3  | 
|---------------------|-----------------------|--------------------------------------|-----------------------|
| Free Memory         | ![FreeMemory_.png](imgs/AutoArima/Iteration-0_FreeMemory_test_result.jpg) | 	![FreeMemory_.png](imgs/AutoArima/Iteration-1_FreeMemory_test_result.jpg) | 	![FreeMemory_.png](imgs/AutoArima/Iteration-2_FreeMemory_test_result.jpg) | 
| Used Memory         | ![UsedMemory_.png](imgs/AutoArima/Iteration-0_UsedMemory_test_result.jpg) | 	![UsedMemory_.png](imgs/AutoArima/Iteration-1_UsedMemory_test_result.jpg) | 	![UsedMemory_.png](imgs/AutoArima/Iteration-2_UsedMemory_test_result.jpg) |   
| Free Disk           | ![FreeDisk_test.png](imgs/AutoArima/Iteration-0_FreeDisk_test_result.jpg) | 	![FreeDisk_test.png](imgs/AutoArima/Iteration-1_FreeDisk_test_result.jpg) | 	![FreeDisk_test.png](imgs/AutoArima/Iteration-2_FreeDisk_test_result.jpg) | 
| Used Disk           | ![UsedDisk_test.png](imgs/AutoArima/Iteration-0_UsedDisk_test_result.jpg) | 	![UsedDisk_test.png](imgs/AutoArima/Iteration-1_UsedDisk_test_result.jpg) | 	![UsedDisk_test.png](imgs/AutoArima/Iteration-2_UsedDisk_test_result.jpg) | 
| Disk read/s         | ![Diskreads_test.png](imgs/AutoArima/Iteration-0_Diskreads_test_result.jpg) | 	![Diskreads_test.png](imgs/AutoArima/Iteration-1_Diskreads_test_result.jpg) | 	![Diskreads_test.png](imgs/AutoArima/Iteration-2_Diskreads_test_result.jpg) | 


[Index](#Home)
