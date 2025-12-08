## usersテーブル

|Column            |Type  |Options    |
|email             |string|null: false|
|encrypted_password|string|null: false|
|name              |string|null: false|
|profile           |text  |null: false|
|occupation        |text  |null: false|
|position          |text  |null: false|

## prototypesテーブル

|Column    |Type      |Option                  |
|title     |string    |null: false             |
|catch_copy|text      |null: false             |
|concept   |text      |null: false             |
|user      |references|null: false, foreign_key|

## commentテーブル

|Colum    |Type     |Option                   |
|content  |text     |null: option             |
|prototype|reference|null: option, foreign_key|
|user     |reference|null: option, foreign_key|