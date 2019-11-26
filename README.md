# README

## usersテーブル

|Column|Type|Options|
|------|----|-------|
|id|INT|null: false|
|name|VARCHAR|null: false|
|email|VARCHAR|null: false, foreign_key: true|
|password|VARCHAR|null: false, foreign_key: true|


### Association
- has_many :users_groups
- has_many :messeages
- has_many  :groups,  through:  users_groups



## groupsテーブル

|Column|Type|Options|
|------|----|-------|
|id|INT|null: false|
|name|VARCHAR|null: false, foreign_key: true|



### Association
- has_many :users_groups
- has_many :messages
- has_many :users,  through:  users_groups


## messagesテーブル

|Column|Type|Options|
|------|----|-------|
|id|INT| null: false, foreign_key: true|
|text|VARCHAR| |
|time|DATETIME| |
|image|VARCHAR| |
|user_id|INT|null: false, foreign_key: true|
|group_id|INT|null: false, foreign_key: true|


### Association
- belongs_to :group
- belongs_to :user


## users_groupsテーブル

|Column|Type|Options|
|------|----|-------|
|user_id|INT|null: false, foreign_key: true|
|group_id|INT|null: false, foreign_key: true|


### Association
- belongs_to :user
- belongs_to :group
