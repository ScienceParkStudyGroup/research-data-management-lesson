---
title: "The FAIR principles"
teaching: 60	
exercises: 30 
questions:
- "How are gene expression levels distributed within a RNA-seq experiment?"
- "Why do I need to scale/normalize read counts?"
- "How do I know that my RNA-seq experiment has worked according to my experimental design?"
- "How informative is PCA and sample clustering for RNA-seq quality checks?"
objectives:
- "Be able to calculate size factors and normalize counts using `DESeq2`."
- "Be able to create PCA and sample clustering plots to explore RNA-seq count results."
- "Be able to interpret a PCA plot and discuss its relationship with the experimental design."
keypoints:
- "Several biaises including sequencing depth can result in analysis artifacts and must be corrected trough scaling/normalisation."
- "RNA-seq results in a multivariate output that can be explored through data reduction methods (e.g. PCA)."
- "Sample clustering and PCA should indicate whether the observed experimental variability can be explained by the experimental design."
---

# Table of contents
<!-- MarkdownTOC autolink="True" levels="1,2" -->

- [FAIR definitions](#fair-definitions)
	- [Detailed defintions](#detailed-defintions)

<!-- /MarkdownTOC -->

# FAIR definitions

## Detailed defintions

- _Findable_:
    * F1. (Meta)data are assigned a globally unique and persistent identifier
    * F2. Data are described with rich metadata (defined by R1 below)
    * F3. Metadata clearly and explicitly include the identifier of the data they describe
    * F4. (Meta)data are registered or indexed in a searchable resource
- _Accessible_:
    * A1. (Meta)data are retrievable by their identifier using a standardised communications protocol
        - A1.1 The protocol is open, free, and universally implementable
        - A1.2 The protocol allows for an authentication and authorisation procedure, where necessary
        - A2. Metadata are accessible, even when the data are no longer available
- _Interoperable_: 
    * I1. (Meta)data use a formal, accessible, shared, and broadly applicable language for knowledge representation.
    * I2. (Meta)data use vocabularies that follow FAIR principles.
    * I3. (Meta)data include qualified references to other (meta)data
- _Reusable_: 
    * R1. (Meta)data are richly described with a plurality of accurate and relevant attributes
        - R1.1. (Meta)data are released with a clear and accessible data usage license
        - R1.2. (Meta)data are associated with detailed provenance
        - R1.3. (Meta)data meet domain-relevant community standards
https://www.mondkapjes.nl/account/reset?token=d006421e90b07259-74d85ba-5fb62f15-5898df80ceb0ba57