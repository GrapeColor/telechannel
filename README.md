# Telechannel
このBOTは簡単なコマンド操作でチャンネル間相互チャットを実現するDiscord向けのBOTです。  
コマンドを実行するメンバーには**チャンネル管理**権限が必要になります。  

## できること
- 接続先へのメッセージ送信
- 添付ファイルの送信
- 複数のチャンネルとの接続

## できないこと
- 接続先に送信されたメッセージの編集・削除
- WebhookやBOTのメッセージを接続先へ送信

## 使い方
- `/connect` : このBOTの使用方法を表示します。
- `/connect [相手のチャンネルID]` : 指定されたチャンネルと、コマンドを入力したチャンネルを接続します
- `/disconnect [相手のチャンネルID]` : 指定されたチャンネルと、コマンドを入力したチャンネルとの接続を切断します
- `/connecting` : コマンドを入力したチャンネルと接続済みのチャンネルを表示します

## 注意点
接続毎にWebhookを生成します。  
このBOTはいわゆるベストエフォート型のサービスですので、すべてのメッセージを送信する保証はできません。  

## 導入方法
次のリンクからご自身のサーバーに導入できます。  
https://discordapp.com/api/oauth2/authorize?client_id=653253608858583040&permissions=536890368&scope=bot  
