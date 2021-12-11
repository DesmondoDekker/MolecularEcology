# qiime2 hhhhhhhhh

```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```



## denoising ITS 
```diff
- 
qiime dada2 denoise-paired --i-demultiplexed-seqs demux-paired-end_ITSS.qza --p-trim-left-f 21 --p-trim-left-r 21 --p-trunc-len-f 240 --p-trunc-len-r 180 --o-table table.qza --o-representative-sequences rep-seqs.qza --o-denoising-stats denoising-stats.qza --p-n-reads-learn 50000 --verbose
```

## <font color="green"> XXX <font> cluster ITS 97%
```
qiime vsearch cluster-features-de-novo --i-table table.qza --i-sequences rep-seqs.qza --p-perc-identity 0.97 --o-clustered-table table-dn-97.qza --o-clustered-sequences rep-seqs-dn-97.qza
```
mmm<font color="green"> XXX <font
