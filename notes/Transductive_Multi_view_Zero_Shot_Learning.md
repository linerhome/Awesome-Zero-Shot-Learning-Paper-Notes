Early ZSL papers, including this one, learns a projection from a low-level feature space to the semantic represention space by the 
auxiliary dataset and applied without adaptation to the target dataset. 

This paper stated the problem of domain shift in zero-shot learning. The visual space and semantic space have different dimensionalities,
resulting in the information loss in the mapping from visual space to semantic space. Also, since the auxiliary domain and the target 
domain have different and potentially unrelated classes, the underlying data distributions differ. Using the projection functions learned
from the auxiliary domain without any adaptation to the target domain causes an unknown shift/bias.
+ Different classes visually present the same attribute in different ways. 

Another problem is the prototype sparsity, which refers to the fact that for each target class, only a single prototype is available for 
zero-shot learning given a semantic representation.

To overcome above two problematic phenomenon in zero-shot learning, the paper proposed a heterogeneous multi-view hypergraph label 
propagation method for zero-shot leanring in the transductive embedding space. It effectivey exploits the complementary informaion 
offered by different semantic representations and takes advantages of the manifold structures of multiple representation spaces in 
coherent manner.

The method 
+ rectifies the projection shift between the auxiliary and target domain.
+ exploits the complementarity of multiple semantic representations.
+ significantly outperforms existing methods for both zero-shot and N-shot recognition.
+ enables novel cross-view annotation tasks.


The domain shift problem is also tackled in the typical ZSL method semantic autoencoder(SAE).
