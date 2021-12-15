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