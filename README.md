# RecSys-for-CSD

## Steps to run test

- Train dlrm model with dataset, and save model (only need to be done once);
- Convert/transform the saved model into an embedding-only binary file (only need to be done once);
- Run test for SSD with limited page cache and for CSD, and monitor the I/O traffic.

## Architecture

<div align=center><img width="150" height="150" src="[https://img-blog.csdn.net/20161028230559575](https://github.com/BaiShuhan/RecSys-for-CSD/blob/main/architecture.png)"/></div>
![image](https://github.com/BaiShuhan/RecSys-for-CSD/blob/main/architecture.png)

## Control Flow

![image](https://github.com/BaiShuhan/RecSys-for-CSD/blob/main/control%20flow.png)
