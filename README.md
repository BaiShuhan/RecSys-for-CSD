# RecSys-for-CSD

## Steps to run test

- Train dlrm model with dataset, and save model (only need to be done once);
- Convert/transform the saved model into an embedding-only binary file (only need to be done once);
- Run test for SSD with limited page cache and for CSD, and monitor the I/O traffic.
