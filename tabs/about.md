---
layout: about
# multilingual page pair id, this must pair with translations of this page. (This name must be unique)
lng_pair: id_about

# image for page specific usage
img: ":profile.png"
# publish date (used for seo)
# if not specified, site.time will be used.
#date: 2022-03-03 12:32:00 +0000

# for override items in _data/lang/[language].yml
#title: My title
#button_name: "My button"
# for override side_and_top_nav_buttons in _data/conf/main.yml
#icon: "fa fa-bath"

# seo
# if not specified, date will be used.
#meta_modify_date: 2022-03-03 12:32:00 +0000
# check the meta_common_description in _data/owner/[language].yml
#meta_description: ""

# optional
# if you enabled image_viewer_posts you don't need to enable this. This is only if image_viewer_posts = false
#image_viewer_on: true
# if you enabled image_lazy_loader_posts you don't need to enable this. This is only if image_lazy_loader_posts = false
#image_lazy_loader_on: true
# exclude from on site search
#on_site_search_exclude: true
# exclude from search engines
#search_engine_exclude: true
# to disable this page, simply set published: false or delete this file
#published: false
---

Hello, my name is Lucas Berg. I am a brazilian researcher with a PhD in Computational Modeling by the Federal University of Juiz de Fora. During my career, I work in different research projects related to cardiac electrophysiology. My major interest is High Performance Computing (HPC) and I believe that software development in this area can really improve our world by reducing the ammount of time spent on solving complex problems.

In addition, for me learning programming is something that everyone should know, especially nowadays where almost everything depends on some kind of software to work. Programming is not only important to understand our connected world, but also helps us in improving our problem solving techniques. Because of that, I always try to pass my knowledge to someone who is facing a similar problem that I already been through. I reckon that helping other people either by teaching them about how to use a new technology or by giving suggestions on how to tackle a problem can be a motivation for not giving up, especially in this field  .

{%- comment -%}
{%- comment -%} Please delete below and place your page content here {%- endcomment -%}

{%- include util/auto-content-generator.liquid -%}
{{ website_info_text_first }}

{{ website_info_text_second }}
{%- endcomment -%}
