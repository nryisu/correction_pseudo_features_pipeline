# build the reference index
sh 0index.sh
# alignment
sh 1alignment.sh 
# mv mapping bamfile to one directory named 'bam' and then merge to count matrix.
sh 2_feature.sh
