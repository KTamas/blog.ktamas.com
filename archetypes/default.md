---
author: KTamas
id: {{ .UniqueID }}
title: "{{ substr (replace .TranslationBaseName "-" " ") 11 | title }}"{{ with now.UTC.Format "2006-01-02T15:04:05Z" }}
date: {{ . }}
lastMod: {{ . }}{{ end }}{{ with now.UTC.Format "2006-01-02" }}
url: /index.php/{{ replace . "-" "/" }}{{ end }}/{{ substr .Name 11 }}/{{ with now.UTC.Format "2006-01-02" }}
permalink: /index.php/{{ replace . "-" "/"  }}{{ end }}/{{ substr .Name 11 }}/
description: ~
tags: []
type: {{ .Type }}
draft: true
---
