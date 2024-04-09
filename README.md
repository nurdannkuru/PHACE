
### PHACE - Phylogeny-Aware Co-Evolution Algorithm


The co-evolution trends of amino acids within or between genes offer valuable insights into protein structure and function. Existing tools for uncovering
co-evolutionary signals primarily rely on multiple sequence alignments (MSAs), often neglecting considerations of phylogenetic relatedness and shared 
evolutionary history. Here, we present a novel approach based on the substitution mapping of amino acid changes onto the phylogenetic tree. We categorize 
amino acids into two groups: 'tolerable' and 'intolerable,' assigned to each position based on the position dynamics concerning the observed amino acids. 
Amino acids deemed 'tolerable' are those observed phylogenetically independently and multiple times at a specific position, signifying the position's 
tolerance to that alteration. Gaps are regarded as a third character type, and we only take phylogenetically independent altered gap characters into 
consideration. Our algorithm is based on a tree traversal process through the nodes and computes the total amount of substitution per branch based on 
the probability differences of two groups of amino acids and gaps between neighboring nodes. To mitigate false co-evolution signals from unaligned regions, 
we employ an MSA-masking approach. When compared to tools utilizing phylogeny (e.g., CAPS and CoMap) and state-of-the-art MSA-based approaches (DCA, GaussDCA, 
PSICOV, and MIp), our method exhibits significantly superior accuracy in identifying co-evolving position pairs, as measured by statistical metrics including 
MCC, AUC, and F1 score. The success of PHACE stems from our capacity to account for the often-overlooked phylogenetic dependency.

![alt text](https://github.com/nurdannkuru/PHACE/blob/main/Outline.svg)
