# DATATune: Database Parameter Tuning via Autoencoder Latent Space

**ICDM 2024 Under Review ... 🤫**

We verify the DATATune performance improvements on MySQL and RocksDB.<br/>
TADA.ipynb is conducted on MySQL A Workload.<br/> TADA_BB.ipynb is conducted on MySQL B Workload.

| Workload Index | Scale Factor | Data Size | Read | Insert | Scan | Update | Read Modify Write |
|----------------|--------------|-----------|------|--------|------|--------|-------------------|
| A              | 12000        | 15GB      | 50%  | -      | -    | 50%    | -                 |
| B              | 12000        | 15GB      | 95%  | -      | -    | 5%     | -                 |
| E              | 12000        | 15GB      | -    | 5%     | 95%  | -      | -                 |
| F              | 12000        | 15GB      | 50%  | -      | -    | -      | 50%               |


![image](https://github.com/addb-swstarlab/DATATune/assets/72485253/3a0d24b1-949e-477a-aa8e-a7904b50add7)

TADA_RocksDB_external_wk2.ipynb is conducted on RocksDB "R90W10" Workload.
![image](https://github.com/addb-swstarlab/DATATune/assets/72485253/3c085ae8-afdf-44e2-959b-c1addc058ca4)

