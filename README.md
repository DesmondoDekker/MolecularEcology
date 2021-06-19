# qiime2

## denoising ITS 
```
qiime dada2 denoise-paired --i-demultiplexed-seqs demux-paired-end_ITSS.qza --p-trim-left-f 21 --p-trim-left-r 21 --p-trunc-len-f 240 --p-trunc-len-r 180 --o-table table.qza --o-representative-sequences rep-seqs.qza --o-denoising-stats denoising-stats.qza --p-n-reads-learn 50000 --verbose
```

## cluster ITS 97%
```
qiime vsearch cluster-features-de-novo --i-table table.qza --i-sequences rep-seqs.qza --p-perc-identity 0.97 --o-clustered-table table-dn-97.qza --o-clustered-sequences rep-seqs-dn-97.qza
```
