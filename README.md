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
その様に思う海が大好き女子に共通の友人を見つけたり、
新たなチャレンジの為のアプリ。

Meeting on the beach.  
**Umi** de **Au**.  
海で会う。  

Creating fun memories together.  
Issho ni tanoshii omoide wo **UmiAu**.  
一緒に楽しい思い出を生み合う。  

## App URL
https://umiau.herokuapp.com/

## Accounts for Tests
### Basic Authentication
ID: admin  
PW: 9876  

### Plan Organizer for Test
ID: test1@gmail.com  
PW: test111111  

### Participant for Test
ID: test2@gmail.com  
PW: test222222 

## Requirement Definitions

### プラン新規作成機能  
`プランの内容および詳細を作成`  
主催者が『プラン名/マリンアクティビティ/日時/場所』以外にも、プラン当日の大まかな流れや利用ショップ等プランの詳細を作成できる  
- マリンアクティビティ、日時、開催都道府県はActive Hushを使用
- プランはイメージ写真や画像を掲載可能
-------
### プラン詳細画面機能
`プランの内容および詳細を表示`  
『プラン名/マリンアクティビティ/日時/場所』以外にも、プラン当日の大まかな流れや利用ショップ、主催者の情報の掲載ができる
- プランの詳細『プラン名/マリンアクティビティ/日時/場所』以外にも、プラン当日の大まかな流れや利用ショップ、主催者の情報（マイページ）を確認できる。
-------
### プラン一覧表示
`新着のプランを表示可能にする`  
トップページに、新着のプランを表示させ、どんなプランが予定されているのかを知らせる
- プランは数点開催予定されていることが前提
- プラン名/マリンアクティビティ/日時/場所のみを1セットにして表示
-------
### プランログ機能
`プランが実施されたことを証明ならびに記録`  
写真を掲載し、どんなプランであったかを記録することができる
- 実際にプランが開催されたとしても、ログを残すかは任意
- 実施もしくは参加したプランの思い出を写真付きでログを残せる
- 可能であれば、ダイビングについては、ログブックとしての機能を追加させたい

## Future Plans for Adding New Functions
### マイページ編集機能
`登録したユーザー情報を更新する`
登録済みのユーザー情報を変更可能にする
・登録済みのユーザー情報（アイコン・住所等）を更新できる
### SNS認証
`ユーザーアカウント登録方法の選択肢を増やす`
SNSアカウント（Googleアカウン、Facabookアカウント）を利用したログイン方法を選択肢として追加する
- ユーザーアカウントの登録方法を「手打ち入力」「Googleアカウントを利用」「Facabookアカウントを利用」の3つから選べるようにする
- SNSアカウントを選択した場合、既にパスワードは入力されてる状態で表示される
### プラン編集機能
`プランを編集可能にする`
プランに変更があった、もしくはヒューマンエラーによるタイプミス等があった場合、内容を修正ならびに変更を可能にする
- プラン詳細画面より、内容に変更、修正ができる
### プラン削除機能
`プランを削除可能にする`
主催者のみがプランの削除が可能。但し問題点として、主催者が闇雲にイベントを削除できてしまうと、トラブルになりかねない為、この機能を付けるべきかは迷うところ
- プラン詳細画面より、プランを削除できる
### コメント機能
`ユーザー同士がオープンかつカジュアルにコミュニケーションを取る`
主催者とプランに興味を持ったユーザーが、プラン詳細画面上で、連絡を取ることが可能
- 主催者とプランに興味を持ったユーザーが、プラン詳細画面上で、掲示板形式で連絡を取る
### 参加表明ボタン機能
`参加表明を手軽に、だけど曖昧にしない`
SNSによくある『いいねボタン』を応用し、参加表明の簡略化を可能にする
- SNSによくある『いいねボタン』同様、ただクリックするだけ
### DM機能
`主催者と参加表明をした参加者が、オープンにはできない個別具体的な連絡を取る`
主催者と参加表明をした参加者が、直接的に連絡を取ることが可能
- 主催者と参加表明をした参加者が、直接的にリアルタイムチャットにて連絡を取り合うことができる
### プラン募集終了機能
`視覚的にプランの参加募集終了している旨を知らせる`
視覚的にプランの参加募集終了している旨を知らせることを可能にする
- プラン編集画面にて、プラン募集終了ボタンをクリックすると、プラン募集終了である旨が表示される
### プラン終了機能
`プラン開催日時を迎えると、視覚的にそれが終了している旨を知らせる`
プラン開催日時を迎えると、視覚的にそれが終了している旨を知らせることを可能にする
- 可能であれば、プラン開催日時を迎えると、自動的にそれが終了している旨を知らせる
### 検索機能
`ユーザーが簡単にデータ検索出来るようにする`
複数条件を指定した上でマリンアクティビティやイベントの検索を可能にする
- プランは数点開催予定されていることが前提
- プラン名/マリンアクティビティ/日時/場所などの検索条件を指定する欄を儲ける
- 条件に該当するイベントの検索結果のページで表示する

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

-------

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

-------

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

## How to Use on Your Local
### Ruby version
ruby 2.6.5  
### Please Execute the Following Commands
% git clone https://github.com/we-b/umiau.git  
% cd umiau  
% bundle install  
% yarn install  
% rails db:create  
% rails db:migrate  