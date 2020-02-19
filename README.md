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

###Options
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