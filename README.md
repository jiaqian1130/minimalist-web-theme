[demo](https://qian30.me)
# 網頁練習
html語法練習
這是一個叫做Max的大佬設計的網頁，我加了一點東西跟一點改造  
我修改的方法是一種標籤加一個html檔，這個方法只適合小型個人網站，如果是大型網站，維護會很困難
[他的github在這](https://github.com/BaseMax/MoloxBlogTheme)  
我主要新增了
1. 黑暗模式
2. 手機適配
3. 新增評功能
4. 小改排版
5. 404頁面
6. 主頁面改成關於我
------
# 使用

#### 評論區
要用評論區的話請去編輯assets/talk.js
```js
const gitalk = new Gitalk({
    clientID: 'GitHub Application Client ID',
    clientSecret: 'GitHub Application Client Secret',
    repo: 'GitHub repo',
    owner: 'GitHub repo owner',
    admin: ['GitHub repo owner and collaborators, only these guys can initialize github issues'],
    id: location.pathname,      // Ensure uniqueness and length less than 50
    distractionFreeMode: false  // Facebook-like distraction free mode
  })
  gitalk.render('gitalk-container')
```
  
####  自訂頭像及網頁圖標
把圖片命轉換 favicon.ico 以及avatar.png 放進image資料夾裡面
#### 自訂社交連結
````html
<ul class="links">
	<li class="post-item">
		<a href="https://discord.com/users/_your_discord_user_ID" target="_blank" rel="noopener noreferrer"><span class="ti-plus"></span> <p class="hidden">Max Base GitHub</p></a>
	</li>
	<li class="post-item">
		<a href="https://github.com/your_githu_name" target="_blank" rel="noopener noreferrer"><span class="ti-github"></span> <p class="hidden">Max Base GitHub</p></a>
	</li>

	li class="post-item">
		<a href="https://mail.google.com/mail/u/0/?fs=1&tf=cm&to=your_email" target="_blank" rel="noopener noreferrer"><span class="ti-email"></span> <p class="hidden">Max Base Email</p></a>
    </li>
	<li class="post-item">
	<a href="https://www.instagram.com/your_IG/" target="_blank" rel="noopener noreferrer"><span class="ti-instagram"></span> <p class="hidden">Max Base Email</p></a>
	</li>
</ul>
````


