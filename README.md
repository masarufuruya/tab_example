## Tab
* タブごとのコンテンツの切り替えを行うコンポーネント
* タブの切り替えにはtab.jsを利用している

## 手順
* ulタグにnav,nav-tabsクラスをつける
* nav-pillsをつけると、pills形式になる
* aタグ内にdata-toggle="tab"をつけるとJSコードを書かずにタブの切り替えが出来る
      <ul class="nav nav-tabs" role="tablist">
        <li role="presentation" class="active"><a href="#home" role="tab" data-toggle="tab">Home</a></li>
        <li role="presentation"><a href="#profile" role="tab" data-toggle="tab">Profile</a></li>
        <li role="presentation"><a href="#messages" role="tab" data-toggle="tab">Messages</a></li>
        <li role="presentation"><a href="#settings" role="tab" data-toggle="tab">Settings</a></li>
      </ul>

* tab-contentクラスの中にタブの中身を書いていく
* nav-tabsのaタグのhrefとtab-contentのidを同一にする
      <div class="tab-content">
        <div role="tabpanel" class="tab-pane active" id="home">home</div>
        <div role="tabpanel" class="tab-pane" id="profile">...</div>
        <div role="tabpanel" class="tab-pane" id="messages">...</div>
        <div role="tabpanel" class="tab-pane" id="settings">...</div>
      </div>

