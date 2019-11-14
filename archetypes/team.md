---
name: "{{ replace .Name "-" " " | name }}"
status: {{ .Status }}
info: {{ .Info }}
draft: true
---