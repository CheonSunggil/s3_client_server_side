# s3_client_server_side
A library that makes it easy to upload and load data using the server-side data storage method using AWS S3 buckets.



## Install

```
pip install s3_client_server_side
```

## S3Client

```
from s3_client_server_side import s3_client
client = s3_client_server_side.S3Client(BUCKET_NAME, ACCESSKEY=False, SECRETKEY=False)

```

## Upload File

```
upload_pkl_file(save_key: str, data: object)
upload_h5_file(self, save_key: str, data: object)
upload_byte_file(self, save_key: str, data: str)

```

## Load File

```
get_pkl_file(self, key: str) -> object
get_h5_file(self, model_key: str) -> object
get_byte_file(self, key: str) -> object

```

## Find the latest data key from bucket

```
get_latest_file_key(self, storage_path: str) -> str
get_latest_folder_key(self, storage_path: str) -> str

```

