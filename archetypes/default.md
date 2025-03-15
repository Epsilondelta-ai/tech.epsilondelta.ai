+++
date = '{{ .Date }}'
draft = true # Change to false to publish
title = '{{ replace .File.ContentBaseName "-" " " | title }}'
tags = []
authors = []
summary = ''
featured_image = '' # e.g. 'thumbnail.png'
slug = '{{ .File.BaseFileName }}' # uri. e.g. 'awesome-post-name'
+++
