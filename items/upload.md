﻿# Upload contents for an item on OneDrive

Items on OneDrive with a [File facet][file-facet] have one or more streams of content
associated with the item. The default stream represents the contents of the
file. Other streams may be used to represent item thumbnails or alternative
data formats.

There are four OneDrive APIs that can be used to upload the contents of an item. The
correct method to use depends on where the content is coming from and how large
the contents of the item are.

* **[Simple item upload](upload_put.md)** is available for items with less than
    100MB of content.

* **[Resumable item upload](upload_large_files.md)** is provided for large files or
    when a resumable transfer may be necessary.

* **[Multipart item upload](upload_post.md)** allows you to upload both the
    contents of an item and provide metadata about the item in the same call.

* **[Upload from URL (preview)](upload_url.md)** allows you to upload the contents of a
    file by providing a URL where the contents of the file can be retrieved.

[file-facet]: ../facets/file_facet.md
