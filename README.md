# DATATune: Database Parameter Tuning via Autoencoder Latent Space

**ICDM 2024 Under Review ... 🤫**

We verify the DATATune performance improvements on MySQL and RocksDB.<br/>
TADA.ipynb is conducted on MySQL A Workload.<br/> TADA_BB.ipynb is conducted on MySQL B Workload.

| Workload Index | Scale Factor | Data Size | Read | Insert | Scan | Update | ReadModifyWrite | 
|----------------|--------------|-----------|------|--------|------|--------|-----------------|
| [`A`]          | -5.75 | -6.18 | -6.75  |  0.379  | -5.59  | 74.7%  |
| [`B`]          |    -  |    -   | -6.33  |  0.21  | -  | -68.4%  | 
| [`E`]          |    -  |    -   | -4.80  |  0.14  | -  | 57.1%  | 
| [`F`]          | -5.15 | -6.42 | -7.15  |  0.48  | -5.12  | 88.7%  | 

![image](https://github.com/addb-swstarlab/DATATune/assets/72485253/3a0d24b1-949e-477a-aa8e-a7904b50add7)

TADA_RocksDB_external_wk2.ipynb is conducted on RocksDB "R90W10" Workload.
![image](https://github.com/addb-swstarlab/DATATune/assets/72485253/3c085ae8-afdf-44e2-959b-c1addc058ca4)

