# RecSys-for-CSD

<p align = "justify"> 
Embedding tables are a crucial part of the Recommendation System (RecSys), and they are all placed in memory at the current stage. As the data volume keeps growing, the memory will run out someday. If the embedding tables were stored in storage without optimizations, the latency would not meet the SLA requirement. The embedding lookup is demonstrated to be the large portion of running RecSys, which usually fetches valid data in kilobytes from the whole table in gigabytes. Offloading embedding lookups to the storage will eliminate the transmission of unwanted data. 
</p>

<p align = "justify"> 
The computational storage will be applied to the RecSys developed by Facebook (DLRM). We will integrate three customized CSD platforms into DLRM at the same time for the end-to-end benchmark. The evaluation of the Kaggle benchmark for DLRM achieves1-2 ms per query. And compared with conventional SSD, the I/O traffic is reduced by 80%. Additionally, the energy consumption is reduced by 20%.
</p>

## Steps to run test

- Train dlrm model with dataset, and save model (only need to be done once);
- Convert/transform the saved model into an embedding-only binary file (only need to be done once);
- Run test for SSD with limited page cache and for CSD, and monitor the I/O traffic.

## Architecture

![image](https://github.com/BaiShuhan/RecSys-for-CSD/blob/main/architecture.png)

## Control Flow

![image](https://github.com/BaiShuhan/RecSys-for-CSD/blob/main/control_flow.png)
