Storage Types

## Block Storage

Block storage chops data into blocks and stores them as separate pieces. Each block of data is given a unique identifier, which allows a storage system to place the smaller pieces of data wherever is most convenient.

The application makes SCSI calls to find the correct address of the blocks, then organizes them to form the complete file.

## File Storage

- Organizes and represents data as a hierarchy of files in folders
- File-based storage systems must scale out by adding more systems, rather than scale up by adding more capacity
- Limited metadata

## Object Storage

Object storage, also known as object-based storage, is a flat structure in which files are broken into pieces and spread out among hardware.

In object storage, the data is broken into discrete units called objects and is kept in a single repository, instead of being kept as files in folders or as blocks on servers.

- Good to store unstructured data
- Rich metadata