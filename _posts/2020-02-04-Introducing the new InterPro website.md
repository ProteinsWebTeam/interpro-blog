# Introducing the new InterPro website

We released a new version of the InterPro website in September 2019. This release is a complete ground-up redesign 
of the website involving changes to both the underying data and also the way users can interact with the data in the 
website. Given the large scale changes perhaps it's unsurprising that we encountered some hiccups, we'll talk about
those later in this post.

## Motivations
### User requests
We looked common requests for new functionality received from users via emails to our helpdesk and other 
communication with the team and collated a list of most requested features.
### Member databases
One of our key goals was to improve access to InterPro member database information within the new website.
### Ensuring codebase is flexible
The technologies and code used to build the previous version of the website were getting increasingly outdated and
limiting the addition of new features to the website.
### Scaling with ever-increasing quantities of data
At the time of writing InterPro us updated approximately every 8 weeks and processes for preparing InterPro releases
were beginning to struggle to analyse the large quantities of protein data being submitted to public databases.

## New features
We'll be going into more detail about the new website and setup in future posts but it's worth highlighting some 
key additions which we hope improve the experience of using InterPro.

* Addition of a number of new data types, **taxonomies, proteomes and sets** (from Pfam and Panther member databases)
* All entries matching specific **Taxonomy nodes** or **Proteomes** can be viewed and downloaded.
* InterProscan results can be viewed within the website with links to matches to InterPro and member entries.
* Introduction of a brand new **Application Programming Interface (API)** for downloading data via scripts
   * We also have an automated script generator to help with getting started with programmatic access.
* Entries from InterPro **Member databases** searchable and viewable throughout the website
* **Interactive 3D representations** of structures, highlighting the location entry matches within the structure.
* We show the following information when showing proteins in the new **ProtVista** graphical view:
  * **Hydrophobicity plot** of whole protein.
  * **Match convservation plot** of Pfam matches to protein showing the extent to which the protein matches the HMM model.
  * **Genome 3D predictions** on protein (where available).
  * **Isoforms** can be selected to view matches to particular splice variants.

## Problems
As we mentioned above the launch of the new site has not been without issues. Many of these have been due to
the processing load on the site and would normally be resolved by the addition of more hardware capacity. 
Unfortunately the addition of more hardware has been delayed due to a pending relocation of our data centre.

In the meantime we've been working to try and make the site more efficient by caching website queries for rapid
response when the same query is made again. We have also been assessing queries that case particular load on the 
servers and pre-computing the data for those queries where possible.

Another major aspect of the work we've been focussing on has been server efficiency to get the most performance out
of the hardware we have. We've been looking at threading and process and connection management to get the most out
of our setup. We have also been looking at running parallel clusters of nodes to allow us to increase the number of
requests we can handle.

We're going to be continuing to monitor site performance and making improvements until we have the website working
faster. 



