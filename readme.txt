IAMSAM is a forward simulation to test predictions of the Indel Associated Mutation model.
IAMSAM (Indel Associated Mutation with Selfing And the letter M)

IAMSAM posits an infinite-allele indel site linked to a non-recombining infinite-sites SNP locus. Command line parameters are:

R: relative mutation rate for indel hets
F: selfing rate
O: original selfing rate
M: mutations rate per locus at SNPs
I: mutations rate per site at the indel
T: generations to run
Q: generations at which selfing evolves
S: random seed
N: diploid popsize

Output is `pop.F  pop.R  pi  num_alleles  is_indel`.

Download iamsam.cc and compile with "g++ iamsam.cc -o iamsam -lgsl -lgslcblas -lm" (requires gnu scientific library).

References

Tian D, Wang Q, Zhang P, Araki H, Yang S et al. (2008) Single-nucleotide mutation rate increases close to insertions/deletions in eukaryotes. Nature 455: 105-108.
Hollister JD, Ross-Ibarra J, Gaut BS (2010) Indel-associated mutation rate varies with mating system in flowering plants. Molecular Biology and Evolution 27: 409-416.
