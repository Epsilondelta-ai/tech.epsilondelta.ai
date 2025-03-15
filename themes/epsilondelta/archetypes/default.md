+++
date = '{{ .Date }}'
draft = true # Change to false to publish
title = '{{ replace .File.ContentBaseName "-" " " | title }}'
description = '' # post's summary or description
tags = []
authors = []
images = [] # e.g. ['thumbnail.png']
slug = '{{ .File.BaseFileName }}' # uri. e.g. 'awesome-post-name'
audio = []
vedios = []
series = []
+++
