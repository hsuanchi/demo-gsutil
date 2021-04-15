# demo-gsutil

## 1. gsutil tool
gsutil is a Python application that lets you access Cloud Storage from the command line.

* Listing buckets and objects.
* Creating and deleting buckets.
* Uploading, downloading, and deleting objects.
* Moving, copying, and renaming objects.
* Editing object and bucket access control lists (ACLs).


## 2. Install gsutil from PyPI
To install gsutil from PyPI, use the following command:
```
$ pip install gsutil
```


## 3. Setting Up Credentials to Access Protected Data
```
$ gsutil config
```


## [4. How-to guides](https://cloud.google.com/storage/docs/how-to)
4-1. Listing buckets
```
$ gsutil ls
```
4-2 Listing objects
```
$ gsutil ls -r {{gs://BUCKET_NAME/**}}
```
4-3 Downloading objects
```
$ gsutil cp {{gs://BUCKET_NAME/OBJECT_NAME}} {{SAVE_TO_LOCATION}}
```
4-4 Uploading objects
```
$ gsutil cp {{OBJECT_LOCATION}} {{gs://DESTINATION_BUCKET_NAME/}}

$ gsutil cp {{gs://SOURCE_BUCKET_NAME/SOURCE_OBJECT_NAME}} {{gs://DESTINATION_BUCKET_NAME/NAME_OF_COPY}}
```
4-5 Renaming an object
```
$ gsutil mv {{gs://BUCKET_NAME/OLD_OBJECT_NAME}} {{gs://BUCKET_NAME/NEW_OBJECT_NAME}}
```

4-6 Deleting objects
* Warning: Object deletion cannot be undone.
```
$ gsutil rm {{gs://BUCKET_NAME/OBJECT_NAME}}
```
