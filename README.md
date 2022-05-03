# lib_CompactCouchDB

**Convertigo** library for **admin** user that allow to perform FullSync or CouchDB compact for all databases (or selected).

Sequence **process**
- databases: databases names to handle or empty for all databases
- doCompactDB: true to perform a _compact
- doCompactViews: true to perform _compact/{design}
- doViewCleanup: true to perform _view_cleanup
- minSizeFile: database using less than this size is skipped
- minFragmentation: database fragmented less than this is skipped
- otherCouchDBurl: empty for current fullsync server or the a CouchDB url to use it
- otherCouchDBusername: specify CouchDB username in case of an url is set
- otherCouchDBpassword: specify CouchDB password in case of an url is set