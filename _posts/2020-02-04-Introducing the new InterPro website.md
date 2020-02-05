---
published: false
layout: post
category: interpro
author: Matloob Qureshi
---


![image of InterPro 7 titlebar](https://github.com/ProteinsWebTeam/interpro-blog/blob/master/assets/media/images/posts/interpro7-titlebar.png)

# Introducing the new InterPro website

We released a new version of the InterPro website in September 2019. This release was a complete ground-up redesign 
of the website involving changes to both the underying data and the web interface. Given the scale of changes we made, 
perhaps it's unsurprising that we encountered some hiccups. We'll talk about those later in this post.

## Goals
### Add commonly requested features
We looked at requests from users received via emails to our helpdesk and other communication with the team and collated everything into a list of the most commonly requested features.
### Show all entries from Member databases
One of our key goals was to improve access to InterPro member database information within the new website. For example, not all entries from member databases have been integrated into InterPro entries yet. We want to display entries defined by member databases regardless of intergration in InterPro in the new site.
### Ensuring codebase is flexible
The technologies and code used to build the previous version of the website were getting increasingly outdated and
limiting the addition of new features to the website.
### Improve scalability of InterPro releases
At the time of writing InterPro us updated approximately every 8 weeks and processes for preparing InterPro releases
were beginning to struggle to analyse the large quantities of protein data being submitted to public databases.

## New features
We'll be going into more detail about the new website and setup in future posts but it's worth highlighting some 
key additions which we hope improve the experience of using InterPro.

### Addition of a number of new data types, taxonomies, proteomes and sets (from Pfam and Panther member databases)
The addition of new datatypes can be seen throughout the site but the **browse** tab is a good starting point for looking into how we connected these datatypes to our data.

![image data typed in new website](https://github.com/ProteinsWebTeam/interpro-blog/blob/master/assets/media/images/posts/interpro7-data-types.png)

### All entries matching specific **Taxonomy nodes** or Proteomes can be viewed and downloaded.
The new taxonomy or proteome page shows lists of all entries, proteins and structures linked to that node or proteome. This can be used to explore data at different levels of the taxonomic tree.

![image of Entries matching taxonomy node:9606 Homo sapiens](https://github.com/ProteinsWebTeam/interpro-blog/blob/master/assets/media/images/posts/interpro7-homo-sapiens-taxonomy-entry-view.png)

### InterProscan results can be viewed within the website with links to matches to InterPro and member entries.
Just as with previous versions of the InterPro website, InterProScan sequence searches can be submitted from the search page but now we've added the ability to view the results within the website. We've also added the ability to view and share the results for as long as they're stored in the InterProScan service (currently results are stored on our servers for 1 week).

![image of InterProScan results](https://github.com/ProteinsWebTeam/interpro-blog/blob/master/assets/media/images/posts/interpro7-interproscan-results.png)

### Introduction of a brand new Application Programming Interface (API for downloading data via scripts
The new website makes use of our api to present data, but the data can be accessed directly without a browser. Documentation for the API can be found at our [github repository](https://github.com/ProteinsWebTeam/interpro7-api/tree/master/docs)

![image of API results](https://github.com/ProteinsWebTeam/interpro-blog/blob/master/assets/media/images/posts/interpro7-api-json.png)

### We have an automated script generator to help with getting started with programmatic access.
The automated script generator is a great starting point for using our API programmatically as it creates scripts in one of three languages, Python, Javascript or Perl. These scripts can be can be edited to run more complex queries.

![image of API results](https://github.com/ProteinsWebTeam/interpro-blog/blob/master/assets/media/images/posts/interpro7-script-generator.png)

### Entries from InterPro Member databases searchable and viewable throughout the website
![image of member database selector](https://github.com/ProteinsWebTeam/interpro-blog/blob/master/assets/media/images/posts/interpro7-member-databases.png)
### Interactive 3D representations of structures, highlighting the location entry matches within the structure.
![image of 3D structure highlighting entry](https://github.com/ProteinsWebTeam/interpro-blog/blob/master/assets/media/images/posts/interpro7-litemol.png)
### We show the following information when showing proteins in the new ProtVista graphical view:
  * **Hydrophobicity plot** of whole protein.
  * **Match convservation plot** of Pfam matches to protein showing the extent to which the protein matches the HMM model.
  * **Genome 3D predictions** on protein (where available).
  * **Isoforms** can be selected to view matches to particular splice variants.
### Integration of modern web standards to provide a good experience on a variety of devices and improve the discoverability 
of our data through search engines e.g **BioSchema**

## Problems and roadmap
As we mentioned above the launch of the new site has not been without issues. Many of these have been due to
the processing load on the site and would normally be resolved by the addition of more hardware capacity. 
Unfortunately the addition of more hardware has been delayed due to a pending relocation of our data centre.

In the meantime we've been working to try and make the site more efficient by caching website queries for rapid
response when the same query is made again. We have also been assessing queries that cause particularly heavy load 
on the servers and pre-computing the data for those queries where possible.

Another major aspect of the work we've been focussing on has been server efficiency to get the most performance out
of the hardware we have. We've been looking into optimising threading and connection management to get the most out
of our setup. We have also been investigating running parallel clusters of nodes to allow us to increase the number of
requests we can handle simulataneously, although this work is still at an experimental stage. We have also moved our 
databases onto solid-state drives (SSD) to reduce general query times.

We're going to be continuing to monitor site performance and making improvements until we have the website working
faster. As mentioned earlier, we should be able to add extra hardware to our website and API once the data centre 
relocation has been completed.

In addition to this we have been optimising the user experience side of things and responding to requests to enable
users to get to the data that they want as efficiently as they can. With this in mind we have also been undertaking
a small User Experience (UX) study to see where we should apply our efforts. 

We'll keep you updated with more information InterPro soon



