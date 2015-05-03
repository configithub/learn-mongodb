

Basic setup
=========

# mongodb admin interface
```
localhost:28017
```

# start/stop mongodb
```
service mongodb start
service mongodb stop
```

# service status for mongodb
```
/etc/init.d/mongodb status
```

update mongodb startup init.d script
```
sudo update-rc.d mongodb defaults
```

update service launch command, edit this file
```
/lib/systemd/system/mongodb.service
```
then launch the daemon update command
```
systemctl daemon-reload
```


Using mongo client
=========

# launch mongo client
```
mongo
```

# change/create database
```
use my_db
```

Create a collection (equivalent of a RDBMS table) by inserting a document (equivalent of a record) in it:
```
db.table.insert({"title":"my_doc_title"})
```

Inspect db size
```
show dbs
```

Remove current db
```
db.dropDatabase()
```

