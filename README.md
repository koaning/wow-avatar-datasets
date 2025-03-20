<img src="orc.png" width="125" height="125" align="right" />

### World of Warcraft Avatar Datasets

> A place to host some interesting parquet files.

<br>

This repository contains the parquet files that belong to the [World of Warcraft Avatar History Dataset](http://web.cs.wpi.edu/~claypool/mmsys-dataset/2011/wow/p123.pdf). The original data came in a 577 RAR 
file that contained 138066 text files. Once converted into a standard .csv file it became 2.1G big. So
I figured to make it easier of others to use to instead turn this into more lightweight parquet files. 

To quote the [docs](http://web.cs.wpi.edu/~claypool/mmsys-dataset/2011/wow/author.html); 
the dataset contains the data over 1,107 days between Jan. 2006 and Jan. 2009. 
During the monitored period, 91,065 avatars, and 667,032 sessions associated with the avatars were 
observed. Because the sampling interval was 10 minutes, there should have been 159,408 
samples, each providing the status of all the avatars online during the sampling period. 
To protect players' privacy, we mapped the avatars' names and guild names randomly as 
positive integers with a consistent mapping (i.e., the same names were always mapped 
to the same integers).

This dataset can be an amazing resource to study bot behavior, churn, marketing and video game addiction.

## Download 

To download the data, run: 

```bash
# To get the `lite` version with only player_id, level and timestamp 
wget https://github.com/koaning/wow-avatar-datasets/blob/main/wow-lite.parquet
# To get the `full` version
wget https://github.com/koaning/wow-avatar-datasets/blob/main/wow-full.parquet
```

