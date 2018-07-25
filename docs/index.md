---
layout: default
title: Introduction
---

# Introduction

If you have used [Swagger](https://swagger.io/), [JSON Schema](http://json-schema.org/) or [RAML](https://raml.org/) to document your API you have probably used JSON references.  A JSON reference is a JSON object that looks like `{"$ref": "http://some/where"}` and points to a JSON object somewhere else so you don't have to copy and paste it.  It's kinda like a hyperlink for JSON.

JSON References are usually used with JSON Schema and API tooling but it's actually a [separate standard](https://tools.ietf.org/html/draft-pbryan-zyp-json-ref-03).  It's pretty handy any time you are writing a complex JSON document and need to repeat yourself.

JSON Reference is a library for resolving references.  You can use this library to resolve references into proxy objects, allowing you to work with a JSON schema with references like a normal JSON document.  You can also inline referenced JSON and create new JSON documents without references.

- Resolves all references, replacing them with proxy objects.
- Supports references to external files, urls, or custom sources.
- Safely resolves circular references.
- Supports caching dereferenced schemas.
- Dereferenced schemas can be safely encoded with `json_encode`.
- Works with Swagger, JSON Schema, and any other spec compliant JSON documents.
