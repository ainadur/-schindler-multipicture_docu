# All images should be stored in Azure with metadata

Azure is the chosen platform to store images and its metadata.

Microsoft provides binary storage with high availability and scalability using Blob Storage. We will be using that to store images.

Cosmos DB is the solution Azure based of a managed database NOSQL, that is the best solution to store JSON type metadata.

## User Stories

- [[]]

## Legacy system 4AllPortal

4AllPortal was the old platform where images have been stored. the metadata was not really being used from this solution.

This was managed through the consulting company Click.it, wich whom we had a contract including storage costs and support.

## Why migrating

### AI projects

Azure is the chosen platform for our AI processes. We are using images for some ongoing projects, like Spare Parts recognition.
Migrating images to Azure improve the way AI can be fed with them.

### Multipicture project

We are developing a new project to manage more than one image for spare parts (currently only one images are allowed). To do so, we need to adapt the APIs used to store data in 4AllPortal and also request a test environment on that platform.
This is similar to what need to be newly developed in Azure environment. We estimate the effort to be bigger but not significantly.

### Manage custom metadata

4AllPortal metadata is not supporting all the metadata that need to be managed for new projects, like multipicture. Without migration, a new way to storege metadata needs to be developed anyway.

### Consolidation of image management

We can leverage on this change to consolidate other images in the same storage to benefit for the high scalability of Azure Blob Storage.
This will also allow us to enrich the metadata of images used in other projects that currently do not manage metadata.
