---
layout: documentation
category: documentation
level: ninja
title: Adding yourself in the wiki contributors list
---

If you want to have a nice header on the page you have written, you can add yourself as wiki contributor.

To do so, you have to edit the ```_config.yml``` file and append your information at the end of the author section. This file is accessible only by github, you can't edit it with prose.io.


## _config.yml
```
##############################################
# Authors Section
# Append your information here:
##############################################
authors:
  matthieulapeyre:
    display_name: Matthieu Lapeyre
    gravatar: ef7c64d1a92babba8d87df3436ecef68
    email: matthieulapeyre@gmail.com
    website:
    social:
        github: matthieu-lapeyre
        linkedin: in/matthieulapeyre
  ....
  ....
  ....

  yournickname:
    display_name:
    gravatar:
    email:
    website:
    social:
        github:
        linkedin: in/
        facebook:
        twitter:
        pinterest:

##############################################
# Wiki configuration
# DO NOT TOUCH !
##############################################
...
...
```
