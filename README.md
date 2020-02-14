# Telechannel
このBOTは簡単なコマンド操作で他チャンネルへのメッセージの自動転送や、チャンネル間チャットなどを実現できるDiscord向けのBOTです。  
コマンドを実行するメンバーには**チャンネル管理**権限が必要になります。  

## できること
- 接続先チャンネルとの双方向メッセージ転送
- 接続先チャンネルからの一方向メッセージ転送
- 接続先チャンネルへの一方向メッセージ転送
- DM、グループチャットチャンネルとの接続(ただし、一方向接続のみ)
- 複数のチャンネルとの接続
- 添付ファイルの転送
- 転送されたメッセージの削除(ただし、一定時間内のみ)
- 転送されたメッセージの編集(ただし、メッセージ送信直後のみ)

## できないこと
- 1チャンネルあたり、11チャンネル以上の双方向・一方向(受信側)接続
- 転送されたメッセージへのリアクションの転送
- WebhookやBOTのメッセージの転送

## 使い方
**●指定チャンネルと接続**  
```/connect [チャンネルID or チャンネルメンション]```  
指定されたチャンネルID、またはチャンネルメンションのチャンネルと接続します。  
接続方法を、双方向接続・一方向接続(受信側/送信側)から選択できます。  
  
**●指定チャンネルと切断**  
```/disconnect [チャンネルID or チャンネルメンション]```  
指定されたチャンネルID、またはチャンネルメンションのチャンネルから切断します。  
  
**●接続中チャンネル一覧**  
```/connecting```  
このチャンネルと接続してるチャンネルの接続方法と名前、IDを表示します。  
  
**●権限の検証**  
```/connectable```  
このチャンネルでBOTの動作に必要な権限があるか、検証します。  

## 注意点
接続毎にWebhookを生成します。  
すべてのメッセージを送信する保証はできません。  

## 導入方法
次のリンクからご自身のサーバーに導入できます。  
https://discordapp.com/api/oauth2/authorize?client_id=653253608858583040&permissions=536964160&scope=bot  
