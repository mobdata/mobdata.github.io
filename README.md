## Welcome to MobData

MobData provides a suite of (mostly) JavaScript apps to manage multiple [Apache CouchDB](https://couchdb.apache.org/) nodes. Easily define complex filters so that only the data you want distributed gets distributed. Resolve replication conflicts with the React-based "little-differ" app to edit and push JSON documents. Monitor the status of all of your CouchDB nodes with the MobBoss app.

### MobNode

[MobNode](https://github.com/mobdata/mobnode) manages the replication filters for an instance of CouchDB. Filters are a feature of CouchDB used to define which data can be sent to remote CouchDB servers. These filters, written in a complex JSON syntax, are difficult to write and CouchDB provides no native view. MobNode has an easy to use language, "MobDsl", so that you can define, review, and apply filters in an intuitive way.

The webapp runs on NodeJs and serves a ReactJs UI. 


### MobBoss

The [MobBoss](https://github.com/mobdata/mobboss) webapp is a tool for monitoring your CouchDB servers. The app gives users visual cues as to the network status, CouchDB instance's status, and replication status for each server, all in a single page, with the ability to drill down into each server's details to resolve conflicts. 

The webapp runs on NodeJs, alongside a [telegraf](https://github.com/influxdata/telegraf) instance, and serves a ReactJs UI.

### little-differ

The [little-differ](https://github.com/mobdata/little-differ) and [little-differ-react](https://github.com/mobdata/little-differ-react) apps help manage the complex 3-way conflicts that occur with CouchDB replication. Displayed in a manner familiar to git users, JSON documents from 2 servers where an automatic merge can't be done, are easily viewed, edited, and applied back to CouchDB.

little=differ is deployed within MobBoss or little=differ-react can be run as a standalone React app.

### Support or Contact

Contact us at mobdatasolution@gmail.com and we’ll help you get started.
