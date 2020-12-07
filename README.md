InterPro blog
=============

Using Jekyll and served using GitHub pages
[see blog](https://ProteinsWebTeam.github.io/interpro-blog/).

Used on the [InterPro website](https://www.ebi.ac.uk/interpro/)
to display the latest blog posts.

## Recommended format for the blog post
The front matter for the post content should have the following data which are used by the InterPro website to render them.

```
published
layout
category
author
excerpt
image_category
```

### Options
_Published_ is either true or false depending on the post's published status.

_Layout_ is post by default.

The following values can be given to the _Category_ option  
* interpro
* focus

_Author_ is optional. 

_Excerpt_ is the short extract to show about the post.

_Image_category_ is for the InterPro website to show images while rendering the blog posts accordingly. The following options are considered.
* General
* Technical
* Biological

## Steps to create a new blog post

1. Upload images used in the blog post to the `assets/media/images/posts` folder
2. Log into https://prose.io/ with your github identifiers and go into the `ProteinsWebTeam/interpro-blog/posts` folder
3. Click on **New file**, the file name format should be `[date-of-publication]-[blog-post-title-with-dash-between-words].md`
4. Add text and images to the article, rendering can be viewed by clicking on the eye icon on the right hand side, go back to editing by clicking on the pen icon
5. Add metadata by clicking on the corresponding icon, this should contain at least the following (see **Recommended format for the blog post** above for more details):
	```
    layout:
    category:
    image_category:
    author:
    ```
6. Go back to the edit mode and click on the "Unpublished" text in the top menu to make the blog post available publicly
7. Click on the save button to commit the changes on github
