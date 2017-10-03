---
published: false
layout: post
category: interpro
---
InterPro has added a new entry type, homologous superfamily, to complement its existing types: family, domain, repeat and site. A homologous superfamily is a group of proteins that share a common evolutionary origin, as indicated by their structural similarities. 

## Why create a new entry type?
Homologous superfamilies are based on [CATH-Gene3D](http://www.cathdb.info/) and [SUPERFAMILY](http://supfam.org/SUPERFAMILY/) entries. These databases use a slightly different methodology to InterPro’s other member databases, in that they often utilise a collection of underlying hidden Markov models to represent diverse structural families, rather than one single signature. As a result, trying to integrate these models into InterPro entries alongside our other member database signatures has not always been straightforward and we have not been able to integrate as much information from these databases as we would like. Creating the new entry type better encapsulates what CATH-Gene3D and SUPERFAMILY are trying to describe and allows us to better represent their data in InterPro. 

This difference in approach between CATH-Gene3D/SUPERFAMILY and the other member databases was highlighted in the recent CATH 4.1 release. This release involved changes to many of the CATH-Gene3D entries to better describe more diverse structural families. This resulted in a divergence in scope from the CATH-Gene3D entries already integrated into InterPro and spurred us to create the new type.

## How do we represent the new entry type?
Homologous superfamily entries are exclusively composed of CATH-Gene3D and/or SUPERFAMILY methods. They are not arranged in hierarchies, and exist as separate entities to families and domains. A typical homologous superfamily entry is shown in Figure 1.

![homologous_sf_screenshot.jpg]({{site.baseurl}}/assets/media/images/posts/homologous_sf_screenshot.jpg)
**Figure 1. InterPro entry page for homologous superfamily EspA/CesA-like.**

Within the protein overview page 'Homologous superfamily' matches are shown on a separate track, in the same way as 'Domain and repeats' (see Figure 2). 

![protein_YAP1_screenshot.jpg]({{site.baseurl}}/assets/media/images/posts/protein_YAP1_screenshot.jpg)
**Figure 2. InterPro protein overview page for AP-1-like ([P19880](http://www.uniprot.org/uniprot/P19880)) transcription factor showing homologous superfamily match.**

## What does this change mean in terms of sequence analysis?
In the short term, this change will have little effect on sequence analysis using InterPro. All member database matches will be calculated as before, but existing CATH-Gene3D and  SUPERFAMILY methods will be removed from existing InterPro entries and reintegrated into new entries corresponding to the homologous superfamily type. Over time, we anticipate that the change will allow us to integrate many more entries from these databases, increasing the sequence and amino acid residue coverage provided by InterPro and allowing us to better represent structural information.