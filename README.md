


# lib_CompactCouchDB

Compact and cleanup a CouchDB server


For more technical informations : [documentation](./project.md)

- [Installation](#installation)
- [Sequences](#sequences)
    - [process](#process)
    - [processAll](#processall)


## Installation

1. In your Convertigo Studio use `File->Import->Convertigo->Convertigo Project` and hit the `Next` button
2. In the dialog `Project remote URL` field, paste the text below:
   <table>
     <tr><td>Usage</td><td>Click the copy button</td></tr>
     <tr><td>To contribute</td><td>

     ```
     lib_CompactCouchDB=https://github.com/convertigo/c8oprj-lib-compactcouchdb.git:branch=master
     ```
     </td></tr>
     <tr><td>To simply use</td><td>

     ```
     lib_CompactCouchDB=https://github.com/convertigo/c8oprj-lib-compactcouchdb/archive/master.zip
     ```
     </td></tr>
    </table>
3. Click the `Finish` button. This will automatically import the __lib_CompactCouchDB__ project


## Sequences

### process

Sequence to view statistics or do a database compact. Suitable for one or small amounts of databases.

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>databases</td><td>Databases names to handle or empty for all databases.</td>
</tr>
<tr>
<td>doCompactDB</td><td>"true" to perform a _compact</td>
</tr>
<tr>
<td>doCompactViews</td><td>"true" to perform _compact/{design}</td>
</tr>
<tr>
<td>doViewCleanup</td><td>"true" to perform _view_cleanup</td>
</tr>
<tr>
<td>limit</td><td>Limit the number of the databases to the specified number.</td>
</tr>
<tr>
<td>minFragmentation</td><td>Percentage of database fragmented less than this is skipped.</td>
</tr>
<tr>
<td>minSizeFile</td><td>Database using less than this size in bytes is skipped.</td>
</tr>
<tr>
<td>otherCouchDBpassword</td><td>Specifies the CouchDB password in case of an url is set.</td>
</tr>
<tr>
<td>otherCouchDBurl</td><td>Empty for current fullsync server or the CouchDB url to use.</td>
</tr>
<tr>
<td>otherCouchDBusername</td><td>Specifies the CouchDB username in case of an url is set.</td>
</tr>
<tr>
<td>skip</td><td> Skip this number of databases.</td>
</tr>
</table>

### processAll

Sequence that compacts all dbs of your couchdb server. Suitable for large amount of databases to proceed.

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>doCompactDB</td><td>"true" to perform a _compact.</td>
</tr>
<tr>
<td>doCompactViews</td><td>"true" to perform _compact/{design}.</td>
</tr>
<tr>
<td>doViewCleanup</td><td>"true" to perform _view_cleanup.</td>
</tr>
<tr>
<td>minFragmentation</td><td>Percentage of database fragmented less than this is skipped.</td>
</tr>
<tr>
<td>minSizeFile</td><td>Database using less than this size in bytes is skipped.</td>
</tr>
<tr>
<td>otherCouchDBpassword</td><td>Specifies the CouchDB password in case of an url is set.</td>
</tr>
<tr>
<td>otherCouchDBurl</td><td>Empty for current fullsync server or the CouchDB url to use.</td>
</tr>
<tr>
<td>otherCouchDBusername</td><td>Specifies the CouchDB username in case of an url is set.</td>
</tr>
<tr>
<td>skipFirst</td><td>skip first n databases.</td>
</tr>
</table>



