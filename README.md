# テーブル設計

## users テーブル

| Column     | Type   | Options  |
| ---------- | ------ | -------- |
| email      | string | NOT NULL |
| password   | string | NOT NULL |
| name       | string | NOT NULL |
| profile    | text   | NOT NULL |
| occupation | text   | NOT NULL |
| position   | text   | NOT NULL |

## prototypesテーブル

| Colum      | Type       | Option   |
| ---------- | ---------- | -------- |
| title      | string     | NOT NULL |
| catch_copy | text       | NOT NULL |
| concept    | text       | NOT NULL |
| user       | references |          |

## commentsテーブル

| Colum     | Type       | Options  |
| --------- | ---------- | -------- |
| text      | text       | NOT NULL |
| user      | references |          |
| prototype | references |          |