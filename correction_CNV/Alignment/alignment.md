# build the reference index
sh 0index.sh
# alignment
sh 1alignment.sh 
# move the mapping bam files to one directory, like named 'bam' and then merge  them to a count matrix.
sh 2_feature.sh
