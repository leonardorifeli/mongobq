[![Build Status](https://travis-ci.org/hakobera/mongobq.svg?branch=master)](https://travis-ci.org/hakobera/mongobq)

# mongobq

`mongobq` is a command line tool to import MongoDB collection into BigQuery.

mongobq >= 0.2.0 only works with node >= 0.12.0.
You want to use with node 0.10 or below, use 0.1.4.

## Usage

```
  Usage: mongobq [options]

  Options:

    -h, --help                      output usage information
    -V, --version                   output the version number
    --host <hostname>               specifies a hostname for the mongod. (Default: "localhost")
    --port <port>                   specifies the TCP port for the mongod. (Default: 27017)
    -u, --username <username>       specifies a mongodb username to authenticate
    -p, --password <password>       specifies a mongodb password to authenticate
    -d, --database <database>       specifies the name of the database
    -c, --collection <collection>   specifies the collection to export
    -f, --fields <field1[,field2]>  specifies a field or fields to include in the export
    -q, --query <JSON>              provides a JSON document as a query that optionally limits the documents returned in the export
    -l, --limit <limit>             limit number of documents returned from query
    -s, --skip <skip>               skip specified number of documents
    -K, --keyfile <keyfile>         specifies the key file path
    -B, --bucket <bucket>           specifies the Google Cloud Storage bucket name
    -O, --path <path>               specifies the output path of the bucket (Default: "/")
    -X, --suffix <suffix format>    specifies the suffix format (Default: "YYYYMMDDHHmmss")
    -P, --project <project>         specifies the project ID of Google Cloud Platform
    -D, --dataset <dataset>         specifies the dataset ID of BigQuery
    -T, --table <table>             specifies the table ID of BigQuery
    -S, --schema <schemafile>       specifies the table schema of BigQuery table to import
    --autoclean                     clean after run
    --async                         no wait load job
    --nocompress                    nocompress data when upload to Google Cloud Storage
    --dryrun                        run as dryrun mode
```

## License

Apache License, Version 2.0
