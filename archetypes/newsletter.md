---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: true
---

** Insert lead paragraph here **

## New Cool Posts

{{ range first 5 ( where .Site.RegularPages "Type" "cool" ) }}
* {{ .Title }}
{{ end }}