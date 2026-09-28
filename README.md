<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>FindWorker</title>

<style>
*{
  box-sizing:border-box;
  margin:0;
  padding:0;
}

body{
  font-family:Arial, sans-serif;
  background:#f5f7fb;
  color:#172033;
}

.app{
  max-width:480px;
  min-height:100vh;
  margin:auto;
  background:#ffffff;
}

/* HEADER */
.header{
  padding:22px 20px 18px;
  background:linear-gradient(135deg,#0d47a1,#1976d2);
  color:white;
  border-radius:0 0 28px 28px;
}

.logo{
  font-size:27px;
  font-weight:800;
}

.tagline{
  margin-top:5px;
  font-size:13px;
  opacity:.9;
}

/* SEARCH */
.search{
  margin-top:20px;
  background:white;
  border-radius:15px;
  padding:13px 15px;
  display:flex;
  align-items:center;
  gap:10px;
  box-shadow:0 8px 25px rgba(0,0,0,.12);
}

.search input{
  width:100%;
  border:0;
  outline:none;
  font-size:14px;
}

/* CONTENT */
.content{
  padding:22px 18px 90px;
}

.title{
  font-size:20px;
  font-weight:800;
  margin-bottom:15px;
}

.categories{
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:12px;
}

.category{
  background:#f7f9fd;
  border:1px solid #e7ebf3;
  border-radius:17px;
  padding:16px 8px;
  text-align:center;
  cursor:pointer;
  transition:.2s;
}

.category:hover{
  transform:translateY(-3px);
  box-shadow:0 8px 20px rgba(0,0,0,.08);
}

.icon{
  font-size:28px;
  margin-bottom:7px;
}

.category span{
  font-size:12px;
  font-weight:700;
}

/* NEARBY */
.nearby{
  margin-top:28px;
}

.worker{
  margin-top:12px;
  padding:16px;
  border:1px solid #e8ebf2;
  border-radius:18px;
  display:flex;
  align-items:center;
  gap:13px;
  background:white;
  box-shadow:0 5px 18px rgba(0,0,0,.05);
}

.worker-img{
  width:52px;
  height:52px;
  border-radius:50%;
  background:#e8f1ff;
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:25px;
}

.worker-info{
  flex:1;
}

.worker-info h3{
  font-size:15px;
}

.worker-info p{
  font-size:12px;
  color:#70798a;
  margin-top:4px;
}

.rating{
  color:#f59e0b;
  font-size:12px;
  margin-top:5px;
}

.view{
  background:#0d47a1;
  color:white;
  border:0;
  padding:9px 12px;
  border-radius:10px;
  font-size:11px;
  font-weight:bold;
}

/* BOTTOM NAV */
.nav{
  position:fixed;
  bottom:0;
  width:100%;
  max-width:480px;
  height:65px;
  background:white;
  border-top:1px solid #e7eaf0;
  display:flex;
  justify-content:space-around;
  align-items:center;
}

.nav-item{
  text-align:center;
  font-size:11px;
  color:#7b8494;
}

.nav-item.active{
  color:#0d47a1;
  font-weight:bold;
}

.nav-icon{
  font-size:20px;
  margin-bottom:3px;
}
</style>
</head>

<body>

<div class="app">

  <div class="header">

    <div class="logo">FindWorker</div>

    <div class="tagline">
      Find trusted workers near you
    </div>

    <div class="search">
      🔍
      <input
        type="text"
        placeholder="What service do you need?"
      >
    </div>

  </div>


  <div class="content">

    <div class="title">
      What do you need?
    </div>

    <div class="categories">

      <div class="category">
        <div class="icon">🔧</div>
        <span>Electrician</span>
      </div>

      <div class="category">
        <div class="icon">🚰</div>
        <span>Plumber</span>
      </div>

      <div class="category">
        <div class="icon">❄️</div>
        <span>AC Repair</span>
      </div>

      <div class="category">
        <div class="icon">🪚</div>
        <span>Carpenter</span>
      </div>

      <div class="category">
        <div class="icon">🎨</div>
        <span>Painter</span>
      </div>

      <div class="category">
        <div class="icon">🧹</div>
        <span>Cleaner</span>
      </div>

      <div class="category">
        <div class="icon">📱</div>
        <span>Mobile Repair</span>
      </div>

      <div class="category">
        <div class="icon">💻</div>
        <span>Computer</span>
      </div>

      <div class="category">
        <div class="icon">🚗</div>
        <span>Mechanic</span>
      </div>

    </div>


    <div class="nearby">

      <div class="title">
        Nearby Workers
      </div>

      <div class="worker">

        <div class="worker-img">🔧</div>

        <div class="worker-info">
          <h3>Electrician</h3>
          <p>Available service provider</p>
          <div class="rating">⭐ New Provider</div>
        </div>

        <button class="view">
          View
        </button>

      </div>


      <div class="worker">

        <div class="worker-img">🚰</div>

        <div class="worker-info">
          <h3>Plumber</h3>
          <p>Nearby service provider</p>
          <div class="rating">⭐ New Provider</div>
        </div>

        <button class="view">
          View
        </button>

      </div>

    </div>

  </div>


  <div class="nav">

    <div class="nav-item active">
      <div class="nav-icon">🏠</div>
      Home
    </div>

    <div class="nav-item">
      <div class="nav-icon">🔎</div>
      Search
    </div>

    <div class="nav-item">
      <div class="nav-icon">📋</div>
      Requests
    </div>

    <div class="nav-item">
      <div class="nav-icon">👤</div>
      Profile
    </div>

  </div>

</div>

</body>
</html>
