# data-Import-from-Sqoop-S3
This repository gives a command code to import data from Sqoop to S3
sqoop import \
-Dfs.s3a.access.key=<> \
-Dfs.s3a.secret.key=<>  \
-Dfs.s3a.endpoint=s3.us-east-2.amazonaws.com  \
--connect jdbc:mysql://localhost/test \
--username root \
--password <> \
--table <> \
-m 1 \
--target-dir s3a://<bucketname/sudip_import;
