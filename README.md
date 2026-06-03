<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>明川市第三中学校友录</title>
<style>
  *{margin:0;padding:0;box-sizing:border-box}
  body{font-family:"Microsoft YaHei","PingFang SC",sans-serif;background:#f0f2f5;color:#333;line-height:1.8;padding:10px}
  .container{max-width:500px;margin:0 auto}
  .page{display:none;background:#fff;padding:20px;border-radius:8px;box-shadow:0 1px 3px rgba(0,0,0,0.1)}
  .page.active{display:block}
  .header{background:#4a90d9;color:#fff;padding:15px;border-radius:8px 8px 0 0;margin:-20px -20px 15px -20px;font-size:18px;font-weight:bold;text-align:center}
  .search-box{margin:15px 0;display:flex;gap:8px}
  .search-box input{flex:1;padding:10px;border:1px solid #ddd;border-radius:4px;font-size:14px}
  .search-box button{padding:10px 20px;background:#4a90d9;color:#fff;border:none;border-radius:4px;font-size:14px}
  .profile-card{border:1px solid #e0e0e0;border-radius:6px;padding:15px;margin:15px 0}
  .profile-card img{width:80px;height:80px;background:#e0e0e0;border-radius:50%;margin-bottom:10px;display:block}
  .comment{border-bottom:1px solid #f0f0f0;padding:12px 0;font-size:14px}
  .comment strong{color:#4a90d9;font-size:13px}
  .comment small{color:#999;font-size:11px}
  .forum-post{border:1px solid #e0e0e0;padding:12px;margin:8px 0;border-radius:4px;color:#999;font-size:13px}
  .forum-post.open{border-color:#4a90d9;color:#333;cursor:pointer}
  .forum-post.open:hover{background:#f7faff}
  .forum-reply{padding:8px 0;border-bottom:1px dotted #eee;font-size:12px}
  .link{color:#4a90d9;cursor:pointer;text-decoration:underline;font-size:13px}
  .back-link{color:#999;cursor:pointer;font-size:12px;margin-bottom:10px;display:block}
  .input-box{width:100%;padding:12px;border:1px solid #ddd;border-radius:4px;margin:15px 0;font-size:16px;text-align:center;letter-spacing:4px}
  .hint{color:#999;font-size:12px;text-align:center;margin-top:8px}
  hr{margin:15px 0;border:none;border-top:1px solid #eee}
</style>
</head>
<body>
<div class="container">

<!-- 校友录搜索页 -->
<div class="page active" id="page-search">
  <div class="header">明川市第三中学 · 校友录</div>
  <p style="color:#999;font-size:13px;margin-bottom:5px">最后登录：2017-10-15</p>
  <div class="search-box">
    <input type="text" id="searchInput" placeholder="输入校友姓名搜索...">
    <button onclick="searchAlumni()">搜索</button>
  </div>
  <p id="searchHint" style="color:#999;font-size:12px;text-align:center;margin-top:10px"></p>
</div>

<!-- 李宜明档案页 -->
<div class="page" id="page-profile">
  <span class="back-link" onclick="goTo('page-search')">← 返回搜索</span>
  <div class="header">李宜明 · 2013届（7班）</div>
  <div class="profile-card">
    <div style="width:80px;height:80px;background:#e8e8e8;border-radius:50%;margin:0 auto 10px;display:flex;align-items:center;justify-content:center;font-size:40px;color:#ccc">👤</div>
    <p><b>性别：</b><span style="color:#ccc">（空白）</span></p>
    <p><b>出生日期：</b><span style="color:#ccc">（空白）</span></p>
    <p><b>就读经历：</b>明川市第三中学（2010-2013）</p>
    <p><b>获奖记录：</b>校级三好学生（2011、2012、2013）</p>
    <p><b>最后登录时间：</b>2013-08-17</p>
    <p><b>个人简介：</b><i>“来日方长。”</i></p>
  </div>
  
  <p style="font-weight:bold;margin:15px 0 5px 0">校友留言（共17条）</p>
  <div class="comment"><strong>张珂</strong> <small>2017-09-03</small><br>突然想起你了。昨天路过三中，操场在翻修，把你当年跑最后一棒的那个跑道挖掉了。我在围挡外面站了很久……宜明，你还好吗？</div>
  <div class="comment"><strong>王蕊</strong> <small>2017-07-14</small><br>同学聚会大家又提到你了。老班说你是他教过最省心的学生。有人问你现在在做什么，没有人知道……我坐在角落里没说话，因为我想不起来你的声音是什么样的了。</div>
  <div class="comment"><strong>陈远</strong> <small>2017-04-01</small><br>愚人节。想起来高中有一年今天，有人说你转学了。全班都信了……你当时是真的觉得好笑吗？还是只是配合我们笑一下？算了，当我没说。</div>
  <div class="comment"><strong>匿名用户</strong> <small>2016-12-24</small><br>平安夜。高中的时候你给全班送了苹果，每人一个，包装纸都不一样。有人说是你自己包的……我把那个苹果放在宿舍桌上放到寒假，走的时候它没烂，只是表皮皱了一点。</div>
  <div class="comment"><strong>赵启明</strong> <small>2016-09-01</small><br>新生报到日。看到一群穿校服的高中生从校门出来，突然就想起你穿着校服的样子。然后我发现我想不起来你校服上有没有别校牌……</div>
  <div class="comment"><strong>刘佳怡</strong> <small>2016-06-07</small><br>高考日。七年前的今天我们也高考。考完数学你站在走廊上，好多人围着你问最后一道大题答案。你说了一个数字。我问你确定吗，你笑了笑没说话。后来出分，那个数字是对的……</div>
  <div class="comment"><strong>匿名用户</strong> <small>2016-03-21</small><br>我梦见你了。梦里的你坐在教室最后一排，低着头写东西。我想走过去看你写什么，但你一直在写……你抬起头看我，说：我在写我。然后就醒了。</div>
  <div class="comment"><strong>孙昊</strong> <small>2015-10-31</small><br>万圣节。你高二那年万圣节，班里有人提议扮鬼。你说，不用扮，我就是。大家都笑了，觉得你在讲笑话。我现在想起来，觉得那可能不是一个笑话。</div>
  <div class="comment"><strong>匿名用户</strong> <small>2015-08-17</small><br>你的最后登录时间是两年前的今天。两年了。你去哪儿了？</div>
  <div class="comment" style="background:#fff9e6"><strong>李宜明</strong> <small>2015-08-17</small><br>我没走啊。<br><small style="color:#999">（11条回复：？？？ 你在哪 你真的在吗 回复我……）</small></div>
  <div class="comment"><strong>匿名用户</strong> <small>2015-06-18</small><br>最近看到一个帖子，是三中校园论坛上的。帖子标题挺有意思的，叫“<span class="link" onclick="goTo('page-forum')">完美的人，还是人吗</span>”。我看了看内容，不知道怎么就想到你了。你要是有空也去看看。</div>
</div>

<!-- 校园论坛页 -->
<div class="page" id="page-forum">
  <span class="back-link" onclick="goTo('page-profile')">← 返回校友录</span>
  <div class="header">三中校园论坛</div>
  <p style="color:#999;font-size:11px;margin-bottom:10px">最后活跃：2015-06-18</p>
  <div class="forum-post">🔒 晚自习后音乐教室的钢琴声<br><small>您没有权限访问该板块</small></div>
  <div class="forum-post">🔒 女生宿舍四楼尽头的镜子<br><small>该帖已被删除或不存在</small></div>
  <div class="forum-post">🔒 旧教学楼地下室的回声<br><small>该板块仅对注册会员开放</small></div>
  <div class="forum-post">🔒 我在监控里看到的东西<br><small>该帖已被锁定</small></div>
  <div class="forum-post">🔒 升旗仪式上不要闭眼<br><small>您所在的用户组无法查看</small></div>
  <div class="forum-post open" onclick="goTo('page-thread')" style="margin-top:15px">
    📄 <b>完美的人，还是人吗</b><br><small>匿名用户 · 2015-06-18 02:17 · 24条回复</small>
  </div>
</div>

<!-- 论坛帖子页 -->
<div class="page" id="page-thread">
  <span class="back-link" onclick="goTo('page-forum')">← 返回论坛</span>
  <div class="header">完美的人，还是人吗</div>
  <p style="font-size:13px;color:#555;margin-bottom:10px"><b>匿名用户</b> · 2015-06-18 02:17</p>
  <p style="font-size:14px;margin-bottom:15px;line-height:2">讨论一个问题。<br><br>如果一个人长得刚好让人记不住五官，说话的声音刚好让人无法分辨男女，说的话永远正确但永远不会被记住原话，做的每一件事都完美得无可挑剔——那这个人，还是人吗？<br><br>或者说，有什么东西需要借用“人”这个壳子，但又不太会装，于是装得太完美了，反而露出了破绽？<br><br>我没有在说任何人。只是问。</p>
  <hr>
  <div class="forum-reply"><b>1楼 匿名用户：</b>你是在说李宜明吧。</div>
  <div class="forum-reply"><b>2楼 匿名用户：</b>谁？</div>
  <div class="forum-reply"><b>3楼 匿名用户：</b>1楼说的那个名字，我好像认识，又好像不认识。我打出来的时候手指抖了一下。</div>
  <div class="forum-reply"><b>4楼 匿名用户：</b>你们有发现吗？这个人的名字没有偏旁部首提示性别。我们学校起名字有规律吗？</div>
  <div class="forum-reply"><b>5楼 匿名用户：</b>我查了一下，宜是合适，明是光亮。这个名字不像父母起的，像被安排的。</div>
  <div class="forum-reply"><b>6楼 匿名用户：</b>歪个楼，我有一个疑问。这个人到底坐第几排？我想不起来。</div>
  <div class="forum-reply"><b>7楼 匿名用户：</b>中间靠窗。不，最后一排。不，是讲台旁边。我真的不记得了。</div>
  <div class="forum-reply"><b>8楼 匿名用户：</b>不是不记得，是每次想起来都不一样。我翻过毕业照，毕业照上根本——</div>
  <div class="forum-reply"><b>9楼 匿名用户：</b>毕业照上怎么了？</div>
  <div class="forum-reply"><b>10楼 匿名用户：</b>没什么。</div>
  <div class="forum-reply"><b>11楼 匿名用户：</b>你们有这种感觉吗？在教室的时候你从来没有主动想起过这个人。但只要有人提起来，你就觉得这个人好像一直就在你旁边坐着。只是你没看见。</div>
  <div class="forum-reply"><b>12楼 匿名用户：</b>我没看见，还是我不敢看见？</div>
  <div class="forum-reply"><b>13楼 匿名用户：</b>我不敢看见。</div>
  <div class="forum-reply"><b>14楼 匿名用户：</b>我也。</div>
  <div class="forum-reply"><b>15楼 匿名用户：</b>去年同学聚会，所有人都在，就这个人不在。但照片拍出来，人数是对的。</div>
  <div class="forum-reply"><b>16楼 匿名用户：</b>什么照片？哪次聚会？</div>
  <div class="forum-reply"><b>17楼 匿名用户：</b>你在说什么聚会？我们没有聚会过。</div>
  <div class="forum-reply"><b>18楼 匿名用户：</b>15楼你是谁？</div>
  <div class="forum-reply"><b>19楼 匿名用户：</b>别问了。</div>
  <div class="forum-reply" style="background:#fff9e6;padding:6px"><b>20楼 <span class="link" onclick="goTo('page-weibo')">李宜明</span></b> · 2015-06-18 03:41<br>这个帖子很有意思。谢谢推荐我的那位同学。</div>
  <div class="forum-reply"><b>21楼 匿名用户：</b>？？？？？？？</div>
  <div class="forum-reply"><b>22楼 匿名用户：</b>你在？？？</div>
  <div class="forum-reply"><b>23楼 匿名用户：</b>这个人真的存在？？？</div>
  <div class="forum-reply"><b>24楼 匿名用户：</b>我点进你主页了。你头像是空的。你个人简介只写了一句话。你关注了零个人。你有零个粉丝。你发过零条帖子。但你注册时间是2010年9月1日。你在线时间累计超过两千个小时。你在看什么？你看什么看了两千个小时？？？</div>
</div>

<!-- 微博页 -->
<div class="page" id="page-weibo">
  <span class="back-link" onclick="goTo('page-thread')">← 返回论坛帖子</span>
  <div style="text-align:center;padding:10px 0">
    <div style="width:60px;height:60px;background:#e0e0e0;border-radius:50%;margin:0 auto 8px"></div>
    <p style="font-weight:bold;font-size:15px">@用户已注销-20130817</p>
    <p style="color:#999;font-size:11px">0关注 · 0粉丝 · 1条微博</p>
    <p style="color:#999;font-size:11px;margin-top:5px"><i>“我看着呢。”</i></p>
  </div>
  <hr>
  <div style="background:#fff;border:1px solid #e8e8e8;border-radius:6px;padding:15px;margin:10px 0">
    <p style="font-size:13px;line-height:2">
      家里的电子锁坏了。<br>
      换了一个。<br>
      新密码是一个日期。<br>
      不是我的生日。<br>
      不是任何人的生日。<br>
      是我想不起来的那一天。<br><br>
      如果哪天我忘了密码，就去问问那个还记得的人。
    </p>
    <small style="color:#999">2013-08-17 23:59</small>
    <div style="background:#f5f5f5;padding:8px;margin-top:8px;border-radius:4px;font-size:12px;color:#666">
      <b>已注销用户：</b>你放心，我会一直记得。<br><small>2013-08-18 00:00</small>
    </div>
  </div>
  <input class="input-box" type="text" placeholder="输入密码" id="pwdInput">
  <p class="hint">* 密码是一个日期</p>
</div>

</div>

<script>
function goTo(pageId){
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  document.getElementById(pageId).classList.add('active');
  window.scrollTo(0,0);
}
function searchAlumni(){
  const val=document.getElementById('searchInput').value.trim();
  if(val==='李宜明'){
    goTo('page-profile');
  }else if(val===''){
    document.getElementById('searchHint').innerText='';
  }else{
    document.getElementById('searchHint').innerText='未找到相关校友。';
  }
}
</script>
</body>
</html>
