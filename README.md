# DATATune: Database Parameter Tuning via Autoencoder Latent Space
SAC 2025 UnderReview ... 😵‍💫

We propose DATATune as a novel approach that differs from trditional database parameter tuning methods.  
To minimize the time required for data generation, DATATune incorporates an **augmentation method for small datasets**. Moreover, it **creates a latent space** by reducing database parameter information and **optimizing all parameters**. Furthermore, by injecting external metric information in the latent space yield precise tuning results by **directly incorporating information from the target workload**.  
Our results show that when comparing the performance improvements of DATATune and the baseline models across four different workloads on MySQL and RocksDB, we observed maximum performance improvements of **1332% for RocksDB** and up to **11.82% in throughput and 46.01% in latency for MySQL**.

This is our experiment workload information.  
### MySQL Workload Information

| Workload Index | Scale Factor | Data Size | Read  | Insert | Scan | Update | Read Modify Write |
| -------------- | ------------ | --------- | ----- | ------ | ---- | ------ | ----------------- |
| A              | 12000        | 15GB      | 50%   | -      | -    | -      | 50%               |
| B              | 12000        | 15GB      | 95%   | -      | -    | 5%     | -                 |
| E              | 12000        | 15GB      | -     | -      | 5%   | 95%    | -                 |
| F              | 12000        | 15GB      | 50%   | -      | -    | -      | 50%               |


### RocksDB Workload Information

| Workload Index | Value Size | # of Entry | READ  | WRITE | UPDATE |
| -------------- | ---------- | ---------- | ----- | ----- | ------ |
| R90W10         | 16384      | 65472      | 90%   | 10%   | X      |
| R50W50         | 16384      | 65472      | 50%   | 50%   | -      |
| R10W90         | 16384      | 65472      | 10%   | 90%   | -      |
| UPDATE         | 16384      | 65472      | -     | -     | O      |



(The 'sac experiment' file is the code that performed the ablation study.)
