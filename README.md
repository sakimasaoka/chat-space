# README

# README

## usersテーブル

|Column|Type|Options|
|------|----|-------|
|id|INT|null: false|
|name|VARCHAR|null: false, foreign_key: true|
|email|VARCHAR|null: false, foreign_key: true|
|password|VARCHAR|null: false, foreign_key: true|


### Association
- has_many :users_groups
- has_many  :groups,  through:  users_groups



## groupsテーブル

|Column|Type|Options|
|------|----|-------|
|id|INT|null: false|




### Association
- has_many :users_groups
- has_many  :users,  through:  users_groups


## messagesテーブル

|Column|Type|Options|
|------|----|-------|
|id|INT|null: false, foreign_key: true|
|text|VARCHAR|null: false|
|time|DATETIME|null: false, foreign_key: true|
|image|VARCHAR|null: false, foreign_key: true|


### Association
- belongs_to :group
- belongs_to :user


## users_groupsテーブル

|Column|Type|Options|
|------|----|-------|
|users_id|INT|null: false|
|groups_id|INT|null: false|


### Association
- belongs_to :user
- belongs_to :group
