# RecSys-for-CSD

## Steps to run test

- Train dlrm model with dataset, and save model (only need to be done once);
- Convert/transform the saved model into an embedding-only binary file (only need to be done once);
- Run test for SSD with limited page cache and for CSD, and monitor the I/O traffic.

## Architecture

<img src="[https://img-blog.csdnimg.cn/2020102116384135.png](https://github.com/BaiShuhan/RecSys-for-CSD/blob/main/architecture.png)" width="100px">
![image](https://github.com/BaiShuhan/RecSys-for-CSD/blob/main/architecture.png)

## Control Flow

![image](https://github.com/BaiShuhan/RecSys-for-CSD/blob/main/control%20flow.png)
