# Restaurant
場所、ジャンル(和食・洋食など)を入力すると、オススメのお店の候補を出してくれるLINE bot。<br/>

<img src="https://github.com/aozam3/Restaurant/assets/65112280/7fe4fa08-42ee-4788-8b3c-be1c84ff6bbb.png" width="300">

<img src="https://github.com/aozam3/Restaurant/assets/65112280/038d05ec-1679-4083-afcc-c84377ad35b0.png" width="300">



## Overview
場所、ジャンル(和食・洋食など)を入力すると、オススメのお店の候補を出してくれるLINE botを開発した。<br/>
さらに、その中から行きたい店名を指定すると、店の詳しい情報も見られる。<br/>
<br/>
なお、LINE botはメッセージを送信すると、前の状態を記憶しておくことができため、Cloud SQLを利用することで、データベースに状態を保存した。<br/>
ユーザーからメッセージを受け取ると、Cloud SQLにアクセスし、前の状態を参照して、次の処理に進む。<br/>

### 例外処理
存在しない地名や料理のジャンルを答えると、例外処理を行う。
<img src="https://github.com/aozam3/Restaurant/assets/65112280/b42156db-b24a-4d5d-bf78-fdab079270e6.png" width="600">

## Requirement
* GCP(Google Cloud Platform)
* ホットペッパーAPI
