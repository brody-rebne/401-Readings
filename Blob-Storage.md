## Blob Storage

### Overview

- Blob storage is a cloud storage format optimized for unstructured data
- Blob storage is ideal for things like:
  - Images
  - Audio files
  - Video files
  - Backup/archival data
  - Data dumps in general

### Structure

- Blob storage is structured around 3 types of resources
- #### Account
  - The namespace for all the data
  - Functions as the base address for accessing your objects
- #### Container
  - A container groups and organizes blobs semantically
  - Similar to a directory/folder in a file system
  - Unlike directories, they cannot be nested
  - The functionality of nested organization is done through naming blobs to include filepathing
- #### Blobs
  - Blobs store the actual objects
  - Azure supports 3 different types of blobs:
    - ##### Block Blobs
      - Text and binary
      - ~4.7TB max size
      - Made up of individually managed blocks of data
    - ##### Append Blobs
      - Optimized for append operations (?)
      - Made up of blocks
    - ##### Page Blobs
      - Random access files
      - 8TB max size
      - Serve as disks for Azure VMs
