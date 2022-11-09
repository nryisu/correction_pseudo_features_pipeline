### The file "mm.merge.pair.RData" and "hs.merge.pair.RData" are used for classifing the cell cycle pahse in mouse and human.
`#` The usage like this in R:<br>
`load("mm.merge.pair.RData")
assignments <- cyclone(umi, merge.pair, gene.names=rownames(counts(umi)))
`
