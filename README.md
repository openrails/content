# Open Rails Content

This repository contains [metadata](#metadata) for a curated collection of Open Rails and Microsoft Train Simulator content.

**Everything about this repository is experimental and subject to change at this time.**

## Contributing

If you know of, or have made yourself, any content which satisfies the following criteria, then please raise an issue or create a pull request with the relevant [metadata](#metadata):

- Fits into the [categories](#categories)
- Does not have any [dependencies](#dependencies)
- Runs acceptably in the latest [Stable Version](https://www.openrails.org/download/program/) of Open Rails

## Categories

Content in this collection must fit into one of these categories:

- Routes - *one or more related routes*
- Train cars - *one or more related locomotives and/or wagons*
- Train sets - *one or more related consists*

Each category is stored as a separate JSON document: `routes.json`, `train-cars.json`, `train-sets.json`.

## Dependencies

Content in this collection **must not** require any separate or additional content to work, including the original Microsoft Train Simulator content. However, it is completely fine for included content to link to other content which **does** require separate or additional content to work.

For example, if a route includes activities or timetables, all referenced train sets and train cars must also be included in a single download. If that is not possible, affected activities and timetables may be offered as a separate download, linked from the route's webpage, but only the route will be included in this collection.

We understand that this limitation will exclude some popular content. However, we hope that content creators understand that we are currently focusing on ease of installation, and we have plans to address this limitation shortly.

## Metadata

Content in this collection must have the following metadata in the JSON file, except for the fields explicitly marked as optional:

| Data | Type | Explanation |
|---|---|---|
| `@type` | Text | `https://schema.org/SoftwareApplication` |
| `compensation` | Enum | `commercial`, `donation`, `free` |
| `name` | Text | Single-line |
| `description` | Text | Multi-line, basic Markdown (bold/italic, lists) |
| `author` | Object |
| `author.@type` | Enum | `https://schema.org/Person`, `https://schema.org/Organization` |
| `author.name` | Text | Single-line |
| `author.url` | URL | *(optional)* Homepage for the author, featuring any other content they have created, including content not eligible for this collection |
| `image` | URL | A small image or logo that identifies the content. Recommended width = 600 px |
| `screenshot` | URL | *(optional)* A webpage showcasing the content with screenshots |
| `url` | URL | This is where interested people will be directed, so it should feature a prominent download or purchase option |
