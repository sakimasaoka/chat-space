# README

## usersテーブル

|Column|Type|Options|
|------|----|-------|
|id|INT|null: false, foreign_key: true|
|name|VARCHAR|null: false, foreign_key: true|
|email|VARCHAR|null: false, foreign_key: true|
|password|VARCHAR|null: false, foreign_key: true|


### Association
- belongs_to :groups
- belongs_to :messages


## groupsテーブル

|Column|Type|Options|
|------|----|-------|
|id|INT|null: false, foreign_key: true|
|users_id|VARCHAR|null: false, foreign_key: true|
|messages_id|VARCHAR|null: false, foreign_key: true|



### Association
- belongs_to :message
- belongs_to :users


## messagesテーブル

|Column|Type|Options|
|------|----|-------|
|id|INT|null: false, foreign_key: true|
|text|VARCHAR|null: false, foreign_key: true|
|time|DATETIME|null: false, foreign_key: true|
|image|VARCHAR|null: false, foreign_key: true|


### Association
- belongs_to :groups
- belongs_to :users
