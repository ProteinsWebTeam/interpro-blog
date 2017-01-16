---
published: true
layout: post
title: A new InterPro member database
date: 2016-06-09T05:15:00.000Z
category: interpro
---
# CDD joins InterPro
We are pleased to announce that the NCBI Conserved Domain Database
([CDD](http://www.ncbi.nlm.nih.gov/Structure/cdd/cdd.shtml)) has joined the
[InterPro](https://www.ebi.ac.uk/interpro/) consortium as a member database,
and has begun to be integrated into the resource.
This is the first new member database to be integrated into InterPro since
[HAMAP](http://hamap.expasy.org/) was included, back in 2009.
As you can see, it has been 7 years since a new database has been added,
and this is a first for the current InterPro team.

While there are some similarities between CDD and InterPro,
with both resource aggregating data from
[Pfam](http://pfam.xfam.org/), [TIGRFAMs](http://www.jcvi.org/cgi-bin/tigrfams/index.cgi)
and [SMART](http://smart.embl-heidelberg.de/), CDD also utilises COGs and PRKs,
whereas InterPro incorporates eight other resources.
Unlike InterPro, the CDD team also curate their own models,
using position specific scoring matrixes (PSSMs) to represent protein domains,
and it is these models that have been prioritised for integration into InterPro.

# What does CDD bring?
This release contains all 11,273 CDD models, with 318 already integrated into InterPro.
It will take time for the rest of the entries to be curated into the InterPro hierarchy,
ensuring that we are consistent with both CDD’s and our own relationship trees,
as well as assigning GO terms for InterPro2GO. The NCBI models are often functionally specific,
with multiple CDD entries covering the same sequence set as
a single Pfam profile hidden Markov model (HMM), for example.

Having such algorithmic and database diversity helps capture as much
knowledge as possible about the function of a protein.
CDD uses a derivative of RPS-BLAST that performs the appropriate assignment
of proteins to database entries. This software, rpsbproc (also known as CD-search),
has been incorporated into the latest version of InterProScan,
making CDD accessible via our web services too.

![A0AM81]({{site.baseurl}}/assets/media/images/posts/A0AM81_600.png)

**Figure 1. [InterProScan](https://www.ebi.ac.uk/interpro/interproscan.html) result for UniProt protein [A0AM81](http://www.uniprot.org/).**
CDD entry cd00770 extends coverage of the protein and adds more functionally specific information
about the C-terminal aminoacyl-tRNA synthetase domain
(in this case, that it is a serine-tRNA ligase domain).

# What Next?
With summer fast approaching, we have our typical break from database releases,
with the next InterPro release not anticipated until the beginning of September.
In the meantime, we have a number of planned infrastructural changes
that will broaden the scope of InterPro further...
We will describe these changes in detail once they are ready!

Rob Finn 
*on behalf of the InterPro team*
