# GitHub pull request練習用リポジトリ


## pull request手順

以下の通りです

1. 各自でGithubアカウント作成/ログイン
1. pull request test用リポジトリをfork
1. forkしたリポジトリを取得/変更を加える
1. Pull Requestをする

## 1. Githubアカウント作成/ログイン

以下を参考にGithubアカウントを作成してログインする。<br>
[GitHub-アカウントの準備と設定](https://git-scm.com/book/ja/v2/GitHub-アカウントの準備と設定)

## 2. pull request test用リポジトリをfork

Github UI上から、以下のtest用リポジトリをforkする。<br>
> [https://github.com/seigot/test_pull_request](https://github.com/seigot/test_pull_request)

fork手順自体は、以下を参考にすると分かりやすい。

> [リポジトリをフォークする](https://docs.github.com/ja/free-pro-team@latest/github/getting-started-with-github/fork-a-repo)<br>
> リポジトリのフォークの例

## 3. forkしたリポジトリを取得/変更を加える

別のマシンで、forkしたリポジトリを取得する。

```
# 例）ユーザ名"seigot"の場合の例、ユーザ名は各自のアカウント名に変更する
git clone https://github.com/seigot/test_pull_request
```

https://github.com/xxx/test_pull_request (ユーザ名：xxx のリポジトリ)をcloneする場合

```
# 例）ユーザ名"seigot"の場合の例、ユーザ名は各自のアカウント名に変更する
git clone https://github.com/xxx/test_pull_request
```

forkしたリポジトリに変更を加える

```
cd test_pull_request             # ディレクトリを移動
git checkout -b test_branch main     # 変更用ブランチへ移動
echo "test" >> README.md         # READMEを変更（最終行に"test"を追記）
git add README.md                # 変更対象に登録
git commit -m "test commit"      # commit messageを記載
git push origin test_branch      # forkしたリポジトリへ変更を登録
```

### 4. Pull Requestをする

以下を参考に、[test_pull_request](https://github.com/seigot/test_pull_request)のリポジトリにPull Requestをします<br>

>[フォークからプルリクエストを作成する](https://docs.github.com/ja/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request-from-a-fork)<br>
フォークからプルリクエストを作成する<br>
1.作成したフォークの元であるリポジトリに移動します。<br>
2.Above the list of files, click  Pull request.<br>
3.[Compare] ページで [compare across forks] をクリックします。<br>
4.[base branch] ドロップダウンメニューで、変更をマージする上流リポジトリのブランチを選択します。<br>
5.[head fork] ドロップダウンメニューでフォークを選択し、次に [compare branch] ドロップダウンメニューを使用して、変更を加えたブランチを選択します。<br>
6.プルリクエストのタイトルと説明を入力します。<br>
7.ユーザが所有するフォークでは、上流のリポジトリに対するプッシュアクセス件を持つ人がプルリクエストに変更することを許したくない場合は、Allow edits from maintainers（メンテナからの編集を許可）の選択を解除してください。<br>
8.レビューの準備ができたプルリクエストを作成するには、Create Pull Request（プルリクエストの作成）をクリックしてください。<br>

以上

# 参考
[GitHub-アカウントの準備と設定](https://git-scm.com/book/ja/v2/GitHub-アカウントの準備と設定)<br>
[リポジトリをフォークする](https://docs.github.com/ja/free-pro-team@latest/github/getting-started-with-github/fork-a-repo)<br>
[プルリクエストの作成方法](https://docs.github.com/ja/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request)<br>
[フォークからプルリクエストを作成する](https://docs.github.com/ja/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request-from-a-fork)<br>
[[実践] はじめてのPull Requestをやってみよう](https://qiita.com/wataryooou/items/8dce6b6d5f54ab2cef04)<br>
[【GitHub】Pull Requestの手順](https://qiita.com/aipacommander/items/d61d21988a36a4d0e58b)<br>

## 以下、テスト用
test1 <br>
test
test2
test2
test2
