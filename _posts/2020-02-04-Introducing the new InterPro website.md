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

* All entries matching specific **Taxonomy nodes** or **Proteomes** can be viewed and downloaded.
* InterProscan results can be viewed within the website with links to matches to InterPro and member entries.
* Introduction of a brand new **Application Programming Interface (API)** for downloading data via scripts
  * We also have an automated script generator to help with getting started with programmatic access.
* Entries from InterPro Member databases searchable and viewable throughout the website
* Interactive 3D representation of structures, showing entry matches in the structure.

## Problems
As we mentioned above the launch of the new site has not been without issues. Many of these have been due to
the processing load on the site and would normally be resolved by the addition of more hardware capcity. 
Unfortunately the addition of this hardware has been delayed due to a pending relocation of our data centre. 


