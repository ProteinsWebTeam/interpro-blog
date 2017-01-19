---
published: false
---
## New entries in InterPro 61.0 - the tip of the iceberg
The thing about icebergs is, with 90% of their volume hidden beneath the water, it can be hard to appreciate their true size. The same can be said about InterPro 61.0, which represents a real iceberg of a release, with a huge amount of unseen work below the surface that is not fully reflected in the release note statistics. 

The major challenge for this release has been the update to PANTHER 11.1, which has seen many changes compared to version 10.0, most notably a switch to using HMMER3.  While this transforms the speed at which we can calculate PANTHER matches, it has brought a few problems too. As a result of the update, nearly 3,000 InterPro entries were at risk of removal, since their underlying PANTHER signatures had been deleted as part of the database rebuild between PANTHER 10.0 and 11.1. The InterPro curators have been working their socks off, trying to find replacement signatures (either in PANTHER 11.1 or from other member databases) that match equivalent sets of sequences so that this huge number of InterPro entries and corresponding annotation was not lost from the resource.

In the end, they pulled off a pretty amazing feat: only 190 of the at risk InterPro entries were lost, with replacement signatures found for the remaining ~2,600. Despite all this upheaval, they still found time to integrate new signatures from a range of different databases, so that the total number of InterPro entries actually grew, from 29,700 entries in release 60.0 to 29,774 in 61.0.

Of course, the work does not stop there. For InterPro release 62.0, we are planning to update several databases, including CATH-Gene3D, which has also undergone substantial changes since we last updated it in InterPro, back in release 41.0. In the meantime, we hope you find this release useful.  If you spot any issues or have any thoughts you would like to share, please provide your feedback to interhelp@ebi.ac.uk.
