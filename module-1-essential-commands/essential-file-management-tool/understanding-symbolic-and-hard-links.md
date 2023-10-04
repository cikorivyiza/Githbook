# Understanding symbolic and hard links

<figure><img src="../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="429">Symbolic links</th><th>Hard links</th></tr></thead><tbody><tr><td>A separate file with a path to the target.</td><td>References the same inode as the original file.</td></tr><tr><td>Small file size, independent of the target's size</td><td>No separate file size; shares data with the original</td></tr><tr><td>Can span different filesystems and link to directories,can cross partitions</td><td>Generally confined to the same filesystem and files only, don't cross partitions.</td></tr><tr><td>Easy to manage during backup and restore.</td><td>Can complicate backup and restore operations.</td></tr><tr><td>Editable; you can change the target.</td><td>Inflexible; always points to the same data</td></tr><tr><td>Has its own permissions and ownership</td><td>Shares permissions and ownership with the original</td></tr><tr><td>Versatile for creating shortcuts and symbolic references.</td><td>Used for creating multiple references to the same data.</td></tr></tbody></table>

