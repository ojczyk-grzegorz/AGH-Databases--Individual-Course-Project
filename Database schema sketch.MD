## Table schemas
#### users
- <em><strong>PK: id</em></strong>
- <em>FK: user_type_id</em>
- email
- password
- <em>FK: company_id</em>
- <em>FK: field_id</em>
- <em>FK: job_position_id</em>

#### users_details
- <em><strong>PK: id</em></strong>
- first_name
- last_name
- profile_picture
- country
- state
- city
- zip_code
- street
- building_no
- apartment_no

#### users_services ???

#### user_types
- <em><strong>PK: id</em></strong>
- name
- description

#### permissions
- <em><strong>PK: id</em></strong>
- code
- name
- description

#### user_types_permissions
- <em>FK: user_type_id</em>
- <em>FK: permission_id</em>

#### companies
- <em><strong>PK: id</em></strong>
- name
- email
- phone
- website

#### companies_details
- <em><strong>PK: id</em></strong>
- logo
- country
- state
- city
- zip_code
- street
- building_no
- apartment_no

#### fields
- <em><strong>PK: id</em></strong>
- name
- description

#### companies_fields
- <em>FK: company_id</em>
- <em>FK: field_id</em>

#### job_positions
- <em><strong>PK: id</em></strong>
- name
- <em>FK: field_id</em>

#### logins_logs
- <em><strong>PK: id</em></strong>
- <em>FK: user_id</em>
- login_datetime

#### logouts_logs
- <em><strong>PK: id</em></strong>
- <em>FK: user_id</em>
- logout_datetime

#### activity_logs
- <em><strong>PK: id</em></strong>
- <em>FK: user_id</em>
- <em>FK: table_id</em>- 
- activity_datetime

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
