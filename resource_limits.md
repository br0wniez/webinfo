# Storage Policy

Home directories are limited to 200 GB. Project space is limited to 250 GB. Scratch storage is limited to 1 TB (2 TB on Xena). Center-wide project scratch space is limited to 1 TB. To purchase additional storage please see our [pricing spreadsheet](https://carc.unm.edu/research/premium-research-computing-services.html).

The 'quotas' command shows your quota usage.

# Compute Usage Policy

To ensure that all research and class projects get their fair share of the clusters and to prevent any one group from using a disproportionate amount of resources, we utilize Slurm’s built-in job accounting and fairshare system.
The cluster is a limited resource and Fairshare allows us to ensure everyone gets a fair opportunity to use it regardless of how big or small the group is.
Your compute resource allocation is shared among everyone in the slurm account you select. 

For more on slurm accounts see this quickbyte: [https://github.com/UNM-CARC/QuickBytes/blob/master/slurm_accounting.md](https://github.com/UNM-CARC/QuickBytes/blob/master/slurm_accounting.md)
Note that your slurm account is not the same as your CARC login account.

To see the predicted start time of your job based on your fairshare score, use the following command:
`squeue --start --job <job_id>`

## Xena Configuration

| Queue                | GPU                             | Bigmem                                | Debug    |
|---:                  |:---:                            |:---:                                  |:---:     |
| Number of Processors | 192                             | 128                                   | 8        |
| Number of Nodes      | 12 (singleGPU) <br> 4 (dualGPU) | 1                                     | 2        |
| Processors per Node  | 16                              | 32                                    | 4        |
| Walltime(H:M:S)      | 48:00:00                        | 48:00:00                              | 04:00:00 |
| Memory Limit         | 62 Gb (singleGPU and dualGPU)   | 1 Tb (bigmem-1TB)<br>3 Tb (bigmem-3TB)| 62 Gb    |


## Wheeler Configuration


|                Queue: |   Default  |    Debug   |
|----------------------:|:----------:|:----------:|
| Number of Processors  |     400    |     32     |
|      Number of Nodes  |     50     |      4     |
|   Processors per Node |      8     |      8     |
|       Walltime(H:M:S) |  48:00:00  |  04:00:00  |
|         Memory Limit  |    48 Gb   |    48 Gb   |



## Gibbs Configuration


|                     | Limit       |
|---:                 | :---:       |
|Number of Processors |	96          |	
|Number of Nodes	    |  6          | 
|Processors per Node  |	16          |        
|Walltime(H:M:S)      |  96:00:00   |
|Memory Limit         |    62 Gb    |


## Hopper Configuration


|                Queue: |   General  |    Debug   | Condo    | Private |
|----------------------:|:----------:|:----------:| :---:    | :---:   |
| Number of Processors  |     64     |     8      | 192      | Determined by <br> queue owner |
|      Number of Nodes  |     2      |      2     | 6        |  |
|   Processors per Node |    32      |      8     | 32       |  |
|       Walltime(H:M:S) |  48:00:00  |  04:00:00  | 48:00:00 |  |
|        Memory Limits  |    95 Gb   |    95 Gb   |          |  |
