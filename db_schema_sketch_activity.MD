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