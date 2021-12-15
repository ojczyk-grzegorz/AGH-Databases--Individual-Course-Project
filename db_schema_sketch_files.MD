## Table schemas
#### files
- <em><strong>PK: id</em></strong> // file_id + version_id
- file_id
- version_id
- name
- picture
- description
- size
- server_link
- download_link

#### files_collections
- <em><strong>PK: id</em></strong>
- name
- picture
- description
- size
- server_link
- download_link

#### files_files_collections_exchange
- <em>FK: files_collection_id</em>
- <em>FK: file_id</em>

#### file_download_logs
- <em><strong>PK: id</em></strong> // == activity_id
- <em>FK: file_id</em>

#### file_collection_download_logs
- <em><strong>PK: id</em></strong> // == activity_id
- <em>FK: file_collection_id</em>

#### schedules
- <em><strong>PK: id</em></strong> // == activity_id
