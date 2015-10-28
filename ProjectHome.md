LATEST VERSION DOWNLOAD LINK:

http://lilab.research.bcm.edu/dldcc-web/lilab/yxi/bsmap/bsmap-2.90.tgz

BSMAP is a short reads mapping software for bisulfite sequencing reads.  Bisulfite treatment converts unmethylated Cytosines into Uracils (sequenced as Thymine) and leave methylated Cytosines unchanged, hence provides a way to study DNA cytosine methylation at single nucleotide resolution.  BSMAP aligns the Ts in the reads to both Cs and Ts in the reference.

RRBSMAP is a specifically designed version of BSMAP for reduced representation bisulfite sequencing (RRBS), it indexes the genome only on the enzyme digestion sites and therefore guarantees all reads were mapped to digestion sites, and greatly reduces the CPU/memory usage.  Since BSMAP-2.0, RRBSMAP has been merged into BSMAP.

BSMAP has the following features:

read length up to 144 nt, allow up to 15 mismatches, gap size up to 3 bp.  standard FASTA/FASTQ/SAM input format. SAM/text format output.

support single end and pair end mapping.  support multi-thread mapping.

support both "Lister protocol" (sequence 2 forward strands only) and "Cokus protocol" (sequence all 4 bisulfite converted strands)

reads are directly mapped to original reference genome sequence, no need to preprocess the reads and reference genome to convert C to T.

support both whole genome bisulfite sequencing (WGBS) mode and reduced representation bisulfite sequencing (RRBS) mode,  allow changing the digestion site information to support different digestion enzymes for RRBS.

allow trimming adapter sequences and low quality nucleotides from the 3'end of reads

allow trade off between speed/memory usage/mapping sensitivity.  For human genome, the RRBS mode uses ~3GB.  In WGBS mode, the typical memory usage is ~9GB, but can be as low as 5GB.

allow alignment for other nucleotide transitions, for example, can be set to detect the A=>I(G) transition in RNA editing.

including down stream script to extract methylation ratios from mapping results.


Using 8 threads, BSMAP could map 28M 76nt pair-end WGBS reads to the human genome in about 2 hours, the memory usage is about 9GB.  (Intel Xeon X5690 @3.47GHz)


Citations:

Xi Y, Li W: BSMAP: whole genome Bisulfite Sequence MAPping program. BMC Bioinformatics (2009) 10:232.


Methylation studies using BSMAP/RRBSMAP:

The Honey Bee Epigenomes: Differential Methylation of Brain DNA in Queens and Workers
Lyko and Foret et al. PLoS Biol (2010) 8(11)
