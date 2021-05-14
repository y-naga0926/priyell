# DB 設計

## users table

| Column               | Type                | Options                   |
|----------------------|---------------------|---------------------------|
| nickname             | string              | null: false               |
| email                | string              | null: false, unique: true |
| encrypted_password   | string              | null: false               |

### Association

- has_many :items dependent: :destroy
- has_many :purchases dependent: :destroy


## pregnancy_week table

| Column                              | Type       | Options                        |
|-------------------------------------|------------|--------------------------------|
| baby_birthday                       | string     | null: false                    |




### Association




## exam_schedule table

| Column                              | Type       | Options                        |
|-------------------------------------|------------|--------------------------------|
|                                     | string     | null:false                     |
|                                     | integer    | null: false                    |
|                                     | text       | null: false                    |
|                                     | integer    | null: false                    |
|                                     | integer    | null: false                    |
|                                     | integer    | null: false                    |
|                                     | integer    | null: false                    |
|                                     | references | null: false, foreign_key: true |
|                                     | integer    | null: false                    |

### Association



## question table

| Column                        | Type       | Options                        |
|-------------------------------|------------|--------------------------------|
| title                         | string     | null: false, foreign_key: true |
| question_form                 | text       | null: false, foreign_key: true |

### Association


## reservation table

| Column                        | Type       | Options                        |
|-------------------------------|------------|--------------------------------|
| family_name                   | string     | null: false, foreign_key: true |
| first_name                    | string     | null: false, foreign_key: true |
| family_name_kana              | string     | null: false, foreign_key: true |
| first_name_kana               | string     | null: false, foreign_key: true |
| first_name                    | string     | null: false, foreign_key: true |
| exam_day                      | string     |                                |

### Association



