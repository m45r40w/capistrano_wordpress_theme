# capistrano_wordpress_theme
Capistranoを利用してテーマファイルの反映を行います

## Installation

実行環境をセットアップする(要`bundler`)
```
git clone git@github.com:m45r40w/capistrano_wordpress_theme.git
cd capistrano_wordpress_theme
bundle install --path=.bundle
```

鍵ファイルを`.ssh`配下に置く
```
cd capistrano_wordpress_theme
cp -p /path/to/key .ssh
```

## How to use

開発用環境へ反映する(`develop`ブランチの内容が反映される)
```
cd capistrano_wordpress_theme
bundle exec cap development deploy
```

本番用環境へ反映する(`master`ブランチの内容が反映される)
```
cd capistrano_wordpress_theme
bundle exec cap production deploy
```

