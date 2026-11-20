# believers-in-Christ-
a worldwide Christian 

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#087a45">
<title>Believers in Christ</title>
<style>
:root {
  --green:#087a45;
  --bright:#16c76a;
  --bg:#f1f7f3;
  --card:#ffffff;
  --text:#173b2b;
  --muted:#718078;
  --line:#dce9df;
}
body.dark {
  --bg:#07150e;
  --card:#10251a;
  --text:#f1fff5;
  --muted:#a4b8aa;
  --line:#294536;
}
* {box-sizing:border-box}
body {
  margin:0;
  font-family:Arial,sans-serif;
  background:var(--bg);
  color:var(--text);
  padding-bottom:85px;
}
header {
  background:linear-gradient(130deg,#034b2c,#087a45);
  color:white;
  padding:24px 18px;
  border-radius:0 0 25px 25px;
}
.top {
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:12px;
}
.logo {font-size:23px;font-weight:bold}
.tagline {color:#c8f5d8;margin-top:5px}
.profile {
  width:43px;height:43px;border-radius:50%;
  background:#d5f6df;color:#087a45;
  display:grid;place-items:center;font-weight:bold;
}
main {padding:18px}
.page {display:none}
.page.active {display:block}
h2 {font-size:22px}
.card {
  background:var(--card);
  border:1px solid var(--line);
  border-radius:18px;
  padding:17px;
  margin:13px 0;
}
.grid {
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:12px;
}
.tile {
  background:var(--card);
  border:1px solid var(--line);
  border-radius:17px;
  padding:22px 10px;
  text-align:center;
  font-size:16px;
  cursor:pointer;
}
.tile span {display:block;font-size:28px;margin-bottom:10px}
button {
  border:0;
  border-radius:12px;
  padding:12px 16px;
  background:var(--green);
  color:white;
  font-size:14px;
  cursor:pointer;
}
button.secondary {
  background:var(--bg);
  color:var(--text);
  border:1px solid var(--line);
}
input {
  width:100%;
  padding:14px;
  border-radius:12px;
  border:1px solid var(--line);
  background:var(--bg);
  color:var(--text);
  font-size:15px;
}
.chat-row {
  display:flex;
  align-items:center;
  gap:12px;
  padding:14px 4px;
  border-bottom:1px solid var(--line);
  cursor:pointer;
}
.avatar {
  width:48px;height:48px;border-radius:50%;
  background:#d8f5e2;color:#087a45;
  display:grid;place-items:center;
  font-weight:bold;font-size:18px;
  flex-shrink:0;
}
.chat-info {flex:1;min-width:0}
.chat-info strong {display:block;margin-bottom:5px}
.muted {color:var(--muted);font-size:13px}
.chat-window {
  display:flex;
  flex-direction:column;
  height:65vh;
}
.messages {
  flex:1;
  overflow-y:auto;
  padding:10px 0;
}
.message {
  max-width:83%;
  padding:12px;
  border-radius:15px;
  background:var(--bg);
  margin:9px 0;
  font-size:15px;
  overflow-wrap:anywhere;
}
.message.mine {
  background:#d7f5e2;
  color:#123c26;
  margin-left:auto;
}
body.dark .message.mine {
  background:#185b37;color:white;
}
.message small {display:block;margin-top:7px;color:var(--muted)}
.message-actions {
  display:flex;gap:7px;flex-wrap:wrap;margin-top:8px;
}
.message-actions button {
  padding:5px 9px;font-size:12px;
}
.composer {
  display:flex;gap:8px;align-items:center;
  padding-top:12px;border-top:1px solid var(--line);
}
.composer input {flex:1;min-width:0}
.pinned {
  background:#e4f8eb;color:#145d35;
  padding:10px;border-radius:10px;
  margin-bottom:10px;font-size:13px;
}
body.dark .pinned {background:#173e29;color:#d7f5e2}
.theme-options {display:flex;gap:9px;flex-wrap:wrap}
.theme-dot {
  width:35px;height:35px;border-radius:50%;
  border:3px solid var(--line);
}
nav {
  position:fixed;bottom:0;left:0;right:0;
  background:var(--card);
  border-top:1px solid var(--line);
  display:flex;justify-content:space-around;
  padding:11px 3px;
  z-index:5;
}
nav button {
  background:transparent;color:var(--muted);
  padding:7px 9px;font-size:12px;
}
nav button.selected {color:var(--green);font-weight:bold}
.hidden {display:none!important}
.section-title {display:flex;justify-content:space-between;align-items:center}
</style>
</head>
<body>

<header>
  <div class="top">
    <div>
      <div class="logo">✝ Believers in Christ</div>
      <div class="tagline">Faith • Fellowship • Service</div>
    </div>
    <div class="profile">SP</div>
  </div>
</header>

<main>

<!-- HOME -->
<section id="home" class="page active">
  <div class="card">
    <h2>Welcome to our community!</h2>
    Grow in faith, connect with believers and serve together.
  </div>

  <h2>Your Dashboard</h2>
  <div class="grid">
    <div class="tile" onclick="showPage('chats')">
      <span>💬</span>Chats
    </div>
    <div class="tile" onclick="showPage('friends')">
      <span>👥</span>Friends
    </div>
    <div class="tile" onclick="showPage('group')">
      <span>🤝</span>Believers in Christ Group
    </div>
    <div class="tile" onclick="showPage('programs')">
      <span>📅</span>Programmes
    </div>
    <div class="tile" onclick="showPage('programs')">
      <span>🕒</span>Timetable
    </div>
    <div class="tile" onclick="showPage('bible')">
      <span>📖</span>Bible
    </div>
    <div class="tile" onclick="showPage('announcements')">
      <span>📢</span>Announcements
    </div>
    <div class="tile" onclick="showPage('profile')">
      <span>👤</span>My Profile
    </div>
  </div>

  <div class="card">
    <h3>Verse of the day</h3>
    <p>“For I know the plans I have for you...”</p>
    <strong>Jeremiah 29:11</strong>
  </div>
</section>

<!-- CHATS -->
<section id="chats" class="page">
  <div class="section-title">
    <h2>Chats</h2>
    <button onclick="newChat()">+ New chat</button>
  </div>
  <input id="chatSearch" placeholder="Search conversations..." oninput="filterChats()">

  <div class="card">
    <div class="section-title">
      <strong>Personal theme</strong>
      <button class="secondary" onclick="showPage('themes')">Change</button>
    </div>
    <p class="muted">Choose how your conversations look.</p>
  </div>

  <div id="chatList">
    <div class="chat-row" data-name="believers in christ group" onclick="openChat('Believers in Christ Group',true)">
      <div class="avatar">BIC</div>
      <div class="chat-info">
        <strong>Believers in Christ Group</strong>
        <span class="muted">Welcome everyone!</span>
      </div>
      <span class="muted">Group</span>
    </div>
    <div class="chat-row" data-name="sarah" onclick="openChat('Sarah',false)">
      <div class="avatar">S</div>
      <div class="chat-info">
        <strong>Sarah</strong>
        <span class="muted">God bless you!</span>
      </div>
      <span class="muted">Private</span>
    </div>
    <div class="chat-row" data-name="daniel" onclick="openChat('Daniel',false)">
      <div class="avatar">D</div>
      <div class="chat-info">
        <strong>Daniel</strong>
        <span class="muted">See you at fellowship.</span>
      </div>
      <span class="muted">Private</span>
    </div>
  </div>
</section>

<!-- CONVERSATION -->
<section id="conversation" class="page">
  <div class="section-title">
    <button class="secondary" onclick="showPage('chats')">← Back</button>
    <h2 id="chatTitle">Conversation</h2>
    <button class="secondary" onclick="showPage('themes')">🎨</button>
  </div>

  <div class="card chat-window">
    <div id="pinnedArea"></div>
    <div id="messages" class="messages">
      <div class="muted">Your conversation starts here.</div>
    </div>
    <div id="replyNotice" class="muted"></div>
    <div class="composer">
      <input id="messageInput" placeholder="Write a message..." onkeydown="if(event.key==='Enter')sendMessage()">
      <button onclick="sendMessage()">Send</button>
    </div>
    <div class="muted">📎 Attachments and calls will be connected in a later development stage.</div>
  </div>
</section>

<!-- THEMES -->
<section id="themes" class="page">
  <h2>Personal Chat Theme</h2>
  <p>Choose a theme for your own chats.</p>
  <div class="card">
    <div class="theme-options">
      <button onclick="setTheme('green')">Green</button>
      <button onclick="setTheme('blue')" style="background:#1769aa">Blue</button>
      <button onclick="setTheme('purple')" style="background:#7542a8">Purple</button>
      <button onclick="setTheme('sunset')" style="background:#c75b39">Sunset</button>
      <button class="secondary" onclick="toggleDark()">Light / Dark</button>
    </div>
  </div>
  <button class="secondary" onclick="showPage('chats')">Back to chats</button>
</section>

<!-- FRIENDS -->
<section id="friends" class="page">
  <h2>Friends</h2>
  <div class="card">Connect with other believers and grow together.</div>
  <input placeholder="Search members...">
  <div class="chat-row"><div class="avatar">S</div><strong>Sarah</strong></div>
  <div class="chat-row"><div class="avatar">D</div><strong>Daniel</strong></div>
  <div class="chat-row"><div class="avatar">J</div><strong>Joshua</strong></div>
</section>

<!-- GROUP -->
<section id="group" class="page">
  <h2>Believers in Christ Group</h2>
  <div class="card">
    <h3>Community fellowship</h3>
    <p>Share messages, encourage one another and grow in faith.</p>
    <button onclick="openChat('Believers in Christ Group',true)">Open group chat</button>
  </div>
  <div class="card">
    <strong>Group information</strong>
    <p class="muted">Pinned messages, group members and announcements will be available here.</p>
  </div>
</section>

<!-- PROGRAMMES -->
<section id="programs" class="page">
  <h2>Programmes & Timetable</h2>
  <div class="card">
    <h3>Community programmes</h3>
    <p>View upcoming activities and ministry assignments.</p>
    <p class="muted">Programme management will be connected to member accounts later.</p>
  </div>
  <div class="card">
    <h3>Weekly timetable</h3>
    <p>Monday — Fellowship</p>
    <p>Wednesday — Bible study</p>
    <p>Friday — Prayer and worship</p>
    <p>Sunday — Main service</p>
  </div>
</section>

<section id="bible" class="page">
  <h2>Holy Bible 📖</h2>
  <div class="card">Bible reading, daily verses, reading plans and translations will be added here.</div>
</section>

<section id="announcements" class="page">
  <h2>Announcements</h2>
  <div class="card">Community news and important updates will appear here.</div>
</section>

<section id="profile" class="page">
  <h2>My Profile</h2>
  <div class="card">
    <div class="avatar">SP</div>
    <h3>Simon Peter</h3>
    <p class="muted">Believers in Christ member</p>
    <button class="secondary" onclick="showPage('themes')">Personal settings</button>
  </div>
</section>

</main>

<nav>
  <button id="nav-home" class="selected" onclick="showPage('home')">⌂<br>Home</button>
  <button id="nav-chats" onclick="showPage('chats')">💬<br>Chats</button>
  <button id="nav-bible" onclick="showPage('bible')">📖<br>Bible</button>
  <button id="nav-announcements" onclick="showPage('announcements')">🔔<br>Alerts</button>
  <button id="nav-profile" onclick="showPage('profile')">👤<br>Profile</button>
</nav>

<script>
let currentChat = "";
let isGroup = false;
let replyText = "";
let chatMessages = {};
let pinnedMessages = {};
let currentTheme = "green";

function showPage(id) {
  document.querySelectorAll(".page").forEach(p=>p.classList.remove("active"));
  document.getElementById(id).classList.add("active");
  document.querySelectorAll("nav button").forEach(b=>b.classList.remove("selected"));
  let nav = document.getElementById("nav-"+id);
  if(nav) nav.classList.add("selected");
}

function openChat(name,group) {
  currentChat=name;
  isGroup=group;
  document.getElementById("chatTitle").textContent=name;
  if(!chatMessages[name]) chatMessages[name]=[];
  if(!pinnedMessages[name]) pinnedMessages[name]=[];
  renderMessages();
  showPage("conversation");
}

function sendMessage() {
  let input=document.getElementById("messageInput");
  let value=input.value.trim();
  if(!value || !currentChat) return;
  chatMessages[currentChat].push({
    text:value,
    reply:replyText,
    mine:true,
    pinned:false,
    reaction:""
  });
  input.value="";
  replyText="";
  document.getElementById("replyNotice").textContent="";
  renderMessages();
}

function renderMessages() {
  let area=document.getElementById("messages");
  let messages=chatMessages[currentChat]||[];
  area.innerHTML="";
  messages.forEach((m,i)=>{
    let div=document.createElement("div");
    div.className="message"+(m.mine?" mine":"");
    let text=document.createElement("div");
    text.textContent=m.text;
    div.appendChild(text);
    if(m.reply) {
      let reply=document.createElement("small");
      reply.textContent="Replying to: "+m.reply;
      div.appendChild(reply);
    }
    if(m.reaction) {
      let reaction=document.createElement("small");
      reaction.textContent="Reaction: "+m.reaction;
      div.appendChild(reaction);
    }
    let actions=document.createElement("div");
    actions.className="message-actions";
    let replyBtn=document.createElement("button");
    replyBtn.textContent="↩ Reply";
    replyBtn.onclick=()=>replyTo(m.text);
    actions.appendChild(replyBtn);

    let reactBtn=document.createElement("button");
    reactBtn.textContent="❤️ React";
    reactBtn.onclick=()=>{m.reaction=m.reaction?"":"❤️";renderMessages()};
    actions.appendChild(reactBtn);

    let pinBtn=document.createElement("button");
    pinBtn.textContent=m.pinned?"Unpin":"📌 Pin";
    pinBtn.onclick=()=>{m.pinned=!m.pinned;renderMessages()};
    actions.appendChild(pinBtn);

    let deleteBtn=document.createElement("button");
    deleteBtn.textContent="Delete";
    deleteBtn.className="secondary";
    deleteBtn.onclick=()=>{chatMessages[currentChat].splice(i,1);renderMessages()};
    actions.appendChild(deleteBtn);

    div.appendChild(actions);
    area.appendChild(div);
  });
  let pins=messages.filter(m=>m.pinned);
  let pinArea=document.getElementById("pinnedArea");
  pinArea.innerHTML="";
  if(pins.length) {
    let p=document.createElement("div");
    p.className="pinned";
    p.textContent="📌 Pinned messages: "+pins.map(m=>m.text).join(" • ");
    pinArea.appendChild(p);
  }
  area.scrollTop=area.scrollHeight;
}

function replyTo(text) {
  replyText=text;
  document.getElementById("replyNotice").textContent="Replying to: "+text;
  document.getElementById("messageInput").focus();
}

function setTheme(theme) {
  currentTheme=theme;
  let colors={
    green:["#087a45","#16c76a"],
    blue:["#1769aa","#4ba3ef"],
    purple:["#7542a8","#a979dc"],
    sunset:["#c75b39","#ed9862"]
  };
  document.documentElement.style.setProperty("--green",colors[theme][0]);
  document.documentElement.style.setProperty("--bright",colors[theme][1]);
  showPage("chats");
}

function toggleDark() {
  document.body.classList.toggle("dark");
}

function filterChats() {
  let q=document.getElementById("chatSearch").value.toLowerCase();
  document.querySelectorAll("#chatList .chat-row").forEach(row=>{
    row.style.display=row.dataset.name.includes(q)?"flex":"none";
  });
}

function newChat() {
  let name=prompt("Enter the member or group name:");
  if(name && name.trim()) openChat(name.trim(),false);
}
</script>
</body>
</html>
