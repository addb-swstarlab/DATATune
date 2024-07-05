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


TADA_RocksDB_external_wk2.ipynb is conducted on RocksDB "R90W10" Workload.
| Workload Index | Value Size   | # of Entry| Read | Write  | Update | 
|----------------|--------------|-----------|------|--------|--------|
| R90W10         | 16384        | 15GB      | 90%  | 10%    | X     | 
| R50W50         | 16384        | 15GB      | 50%  | 50%    | X    | 
| R10W90         | 16384        | 15GB      | 10%   | 90%     | X  |
| UPDATE         | 16384        | 15GB      | -  | -      | O    | 

