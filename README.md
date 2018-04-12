CreateProfile
====
GoogleSpreadsheetようのGAS。別シート(DB)に集めた個人情報から検索画面シートを生成し、検索ボタンを押したら結果シートが作成される。

## Sheets
以下の4つのシートから構成されます。
*DB
個人情報を集めておく
*Search
検索画面
*Result
実際にプロフィールが出来上がる
*Format
Resultのレイアウトを定義する

## Scripts
以下の3つのスクリプトがあります。
*EditProfile
Resultにプロフィールを作成する
*CreateSearch
検索画面を作成する
*CallScripts(Searchに紐づけされている)
EditProfileとCreateSearchを呼び出す

## Description
CallScriptsはSearchに配置された2つのボタンにそれぞれ紐づけされています。  
ボタンを押すとCreateSearchかEditProfileが呼び出され、シートを編集します。
