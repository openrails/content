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

## Dependencies

Content in this collection **must not** require any separate or additional content to work, including the original Microsoft Train Simulator content. However, it is completely fine for included content to link to other content which **does** require separate or additional content to work.

For example, if a route includes activities or timetables, all referenced train sets and train cars must also be included in a single download. If that is not possible, affected activities and timetables may be offered as a separate download, linked from the route's webpage, but only the route will be included in this collection.

We understand that this limitation will exclude some popular content. However, we hope that content creators understand that we are currently focusing on ease of installation, and we have plans to address this limitation shortly.

## Metadata

Content in this collection must have the following metadata:

| Data | Type | Explanation |
|---|---|---|
| Category | Enum | Route, Train Car, Train Set |
| Compensation | Enum | Commercial, Donation, Free |
| Name | Text | Single-line |
| Description | Text | Multi-line, basic Markdown (bold/italic, lists) |
| Author | Text | Single-line |
| Image | ? | **What are we doing here???** |
| URL | URL | This is where interested people will be directed, so it should feature a prominent download or purchase option |
