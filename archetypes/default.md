---
title: "{{ replace .Name '-' ' ' | title }}"
date: {{ .Date }}
draft: {{ .Site.Params.defaultDraft | default true }}
categories: []
tags: []
---
