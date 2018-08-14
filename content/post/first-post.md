+++
title = "First Post"
date = 2018-05-07T20:55:01-07:00
draft = false

# Tags and categories
# For example, use `tags = []` for no tags, or the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []
tags_include = []
tags_exclude = []
categories = []

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
# Use `caption` to display an image caption.
#   Markdown linking is allowed, e.g. `caption = "[Image credit](http://example.org)"`.
# Set `preview` to `false` to disable the thumbnail in listings.
[header]
image = ""
caption = ""
preview = true

+++

## About me

I am a part time student in Georgia Tech's OMSCS program. I am currently employed at a software company in Tucson. I graduated from the University of Arizona in 2016 with an engineering degree.

I plan to use this blog as a record of my work and my ideas. My current interests include machine learning and data science, finance, economics, mineral exploration, geostatistics, GIS, and remote sensing.  

## Building the Blog

My blog is hosted on AWS. I have a cloudfront distribution that . I had a lot of trouble finding documentation on this process unfortunately. Turned out to be a lot easier than most of the articles would have you believe. 

If Amazon is your registrar it winds up being extremely easy- simply visit https://us-east-2.console.aws.amazon.com/acm/, press "Request Certificate", "Request a public certificate", enter your domain name (I just used the wildcard *.nicholasshea.com, in case I decide to add an API endpoint at api.nicholasshea.com or something like that) 
select DNS validation.

This part is somewhat tricky- 


Then you'll need to 

Get screenshots of the process.

I made two pretty painful mistakes: 
1) initially forgot to set the s3 bucket to public
2) did not select the http-to-https upgrading option. Instead I initially chose to drop all non-HTTPS traffic.

