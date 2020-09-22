## App Name
UmiAu

## Outline and Origin of This App Name
Surprisingly, there are girls who get a diving license alone or start taking class of surf school alone.
They could get along with someone there, but in reality through it's not easy.
Wanna enjoy with friends who likes to enjoy beach life.
Wanna share my own memories on the beach.
App for girls who likes to enjoy beach life. 

一人でダイビングのライセンスを取ったり、一人でサーフスクールに通い始める女子が意外といる。
そこで誰かと仲良くなれたらいいのだけど、実際はそんなに簡単なことではなかったりする。
『海が好き』という共通の仲間と楽しみたい。
海での思い出をシェアしたい。
海が大好き女子の為のアプリ。

Meeting on the beach.
**Umi** de **Au**.
海で会う。

Creating fun memories together.
Issho ni tanoshii omoide wo **UmiAu**.
一緒に楽しい思い出を生み合う。


## App URL
https://umiau.herokuapp.com/

## Tables
### users table

| Column             | Type    | Options     |
| ------------------ | ------- | ----------- |
| nickname           | string  | null: false |
| favorite_genre1_id | integer | null: false |
| favorite_genre2_id | integer | null: false |
| favorite_genre3_id | integer | null: false |
| email              | string  | null: false |
| password           | string  | null: false |
| family_name        | string  | null: false |
| given_name         | string  | null: false |
| family_name_kana   | string  | null: false |
| given_name_kana    | string  | null: false |
| phone_num          | string  | null: false |
| birth_day          | date    | null: false |

#### Association
- has_many :plans
- has_many :logs
- belongs_to_active_hash :genre


### plans table

| Column             | Type       | Options                        |
| ------------------ | ---------- | ------------------------------ |
| user               | references | null: false, foreign_key: true |
| name               | string     | null: false                    |
| genre_id           | integer    | null: false                    |
| date               | date       | null: false                    |
| time               | string     | null: false                    |
| location1_id       | integer    | null: false                    |
| location2          | integer    | null: false                    |
| detail             | text       | null: false                    |

#### Association
- belongs_to :users
- has_one :logs
- belongs_to_active_hash :genre
- belongs_to_active_hash :location


### logs table

| Column             | Type       | Options                        |
| ------------------ | ---------- | ------------------------------ |
| user               | references | null: false, foreign_key: true |
| plan               | references | null: false, foreign_key: true |
| title              | string     | null: false                    |
| note               | text       | null: false                    |

#### Association
- belongs_to :users
- belongs_to :plans