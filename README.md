# relation-app-practice

## 概要
COACHTECH 教材 Tutorial 9-5「リレーション」
Eloquent ORMによるタグやコメントのリレーションをもったブログ投稿一覧

## 使用技術
- PHP 8.5.6
- Laravel 10.50.2
- Laravel Sail
- Eloquent ORM (hasMany / belongsTo / belongsToMany)
- MySQL

## 学んだこと
- hasMany, belongsTo, belongsToManyによる1対1、 1対多、多対多の関係の実装
- eagerLoadingとlazyLoadingの違い
- with, withCount, has, whereHasを使った関連データの扱い方

## 動作確認
```bash
git clone https://github.com/ds1995-dev/relation-app-practice.git
cd relation-app-practice
composer install
cp .env.example .env
./vendor/bin/sail up -d
./vendor/bin/sail artisan key:generate
./vendor/bin/sail artisan migrate --seed
```


