<!DOCTYPE html>
<html>
<title>天氣資訊</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<link rel="stylesheet" href="https://www.w3schools.com/lib/w3-theme-black.css">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.3.0/css/font-awesome.min.css">

<body>
   <nav class="w3-sidebar w3-bar-block w3-card w3-animate-left w3-center" style="display:none" id="mySidebar">
    <span style="font-size:30px;" ><p>系統功能</p></span>
     <span style="font-size:30px;"><button class="w3-bar-item w3-button" onclick="w3_close()">Close<i class="fa fa-remove"></i></button></span>
   
     <a href="jwplayer.html"  target='_blank'><span style="font-size:18px;" ><p class="w3-bar-item w3-button">電腦版直播系統</p></span></a>
     <a href="NewCell.html"  target='_blank'><span style="font-size:18px;"><p class="w3-bar-item w3-button">手機版直播系統</p></span></a>
     <a href="https://tianyan.ddns.net/rec"  target='_blank'><span style="font-size:18px;"><p class="w3-bar-item w3-button">直播記錄觀賞</p></span></a>
     <a href="NewWeather.php"  target='_blank'><span style="font-size:18px;"><p class="w3-bar-item w3-button">天氣查詢系統</p></span></a>
     <a href="map.html"  target='_blank'><span style="font-size:18px;"><p class="w3-bar-item w3-button">地圖定位系統</p></span></a>
   </nav>

   <header class="w3-container w3-theme w3-padding" id="myHeader">
    <i onclick="w3_open()" class="fa fa-bars w3-xlarge w3-button w3-theme"></i> 
    <div class="w3-center">
    </div>
  </header>




<div class="w3-display-container" style="margin-bottom:50px">
  <img src="3.jpg" style="width:100%">
  <div class="w3-display-bottomleft w3-container w3-amber w3-hover-orange w3-hide-small"
   style="bottom:10%;opacity:0.7;width:70%">
  <h2><b>This Is Weather Informations~<br>Have a nice day!</b></h2>
</div>
</div>

<div class="w3-row w3-container" style="margin:50px 0">

<hr>

<form name="myForm" action="NewWeather.php" method="POST">
縣市：
<select name="country" id="country" size=1 onChange="renew(this.selectedIndex);">
	<option value="鄉鎮選取">縣市選取</option>
    <option value="基隆市">基隆市</option>
	<option value="台北市">台北市
	<option value="新北市">新北市
	<option value="桃園市">桃園市
	<option value="台中市">台中市
    <option value="台南市">台南市
    <option value="高雄市">高雄市
    <option value="新竹縣">新竹縣
	<option value="新竹市">新竹市
    <option value="苗栗縣">苗栗縣
    <option value="彰化縣">彰化縣
    <option value="南投縣">南投線
    <option value="雲林縣">雲林縣
    <option value="嘉義縣">嘉義縣
    <option value="嘉義市">嘉義市	
    <option value="屏東縣">屏東縣   
    <option value="台東縣">台東縣
    <option value="花蓮縣">花蓮縣
    <option value="宜蘭縣">宜蘭縣
    <option value="澎湖縣">澎湖縣
    <option value="金門縣">金門縣
    <option value="連江縣">連江縣
</select>

鄉鎮：
<select name="member" id="member" size=1>
	<option value="">請由左方選取縣市
</select>
 <input type="submit" value="確定送出">
</form>

<hr>


</div>

<script>
// Side navigation
function w3_open() {
    var x = document.getElementById("mySidebar");
    x.style.width = "100%";
    x.style.fontSize = "40px";
    x.style.paddingTop = "10%";
    x.style.display = "block";
}
function w3_close() {
    document.getElementById("mySidebar").style.display = "none";
}



// Accordions
function myAccFunc(id) {
    var x = document.getElementById(id);
    if (x.className.indexOf("w3-show") == -1) {
        x.className += " w3-show";
    } else { 
        x.className = x.className.replace(" w3-show", "");
    }
}

// Slideshows
var slideIndex = 1;

function plusDivs(n) {
slideIndex = slideIndex + n;
showDivs(slideIndex);
}

function showDivs(n) {
  var x = document.getElementsByClassName("mySlides");
  if (n > x.length) {slideIndex = 1}    
  if (n < 1) {slideIndex = x.length} ;
  for (i = 0; i < x.length; i++) {
     x[i].style.display = "none";  
  }
  x[slideIndex-1].style.display = "block";  
}

showDivs(1);

// Progress Bars
function move() {
  var elem = document.getElementById("myBar");   
  var width = 5;
  var id = setInterval(frame, 10);
  function frame() {
    if (width == 100) {
      clearInterval(id);
    } else {
      width++; 
      elem.style.width = width + '%'; 
      elem.innerHTML = width * 1  + '%';
    }
  }
}
</script>



</body>
</html>

<script>
department=new Array();
department[0]=["選擇都市"];
department[1]=["仁愛區","中正區","信義區","中山區","安樂區","暖暖區","七堵區"];//基隆市
department[2]=["中正區","大同區","中山區","松山區","大安區","萬華區","信義區","士林區","北投區","內湖區","南港區","文山區"];	//台北市
department[3]=["板橋區","新莊區","中和區","永和區","土城區","樹林區","三峽區","鶯歌區","三重區","蘆洲區","五股區","泰山區","林口區","八里區","淡水區","三芝區","石門區","金山區","萬里區","汐止區","瑞芳區","貢寮區","平溪區","雙溪區","新店區","深坑區","石碇區","坪林區","烏來區"];	// 新北市
department[4]=["桃園區","中壢區","平鎮區","八德區","楊梅區","蘆竹區","大溪區","龍潭區","龜山區","大園區","觀音區","新屋區","復興區"];	//桃園市		
department[5]=["中區","東區","南區","西區","北區","北屯區","西屯區","南屯區","太平區","大里區","霧峰區","烏日區","豐原區","后里區","石岡區","東勢區","新社區","潭子區","大雅區","神岡區","大肚區","沙鹿區","龍井區","梧棲區","清水區","大甲區","外埔區","大安區","和平區"];//台中市
department[6]=["中西區","東區","南區","北區","安平區","安南區","永康區","歸仁區","新化區","左鎮區","玉井區","楠西區","南化區","仁德區","關廟區","龍崎區","官田區","麻豆區","佳里區","西港區","七股區","將軍區","學甲區","北門區","新營區","後壁區","白河區","東山區","六甲區","下營區","柳營區","鹽水區","善化區","大內區","山上區","新市區","安定區"]//台南市
department[7]=["楠梓區","左營區","鼓山區","三民區","鹽埕區","前金區","新興區","苓雅區","前鎮區","旗津區","小港區","鳳山區","大寮區","鳥松區","林園區","仁武區","大樹區","大社區","岡山區","路竹區","橋頭區","梓官區","彌陀區","永安區","燕巢區","田寮區","阿蓮區","茄萣區","湖內區","旗山區","美濃區","內門區","杉林區","甲仙區","六龜區","茂林區","桃源區","那瑪夏區"];//高雄市
department[8]=["竹北市","竹東鎮","新埔鎮","關西鎮","湖口鄉","新豐鄉","峨眉鄉","寶山鄉","北埔鄉","芎林鄉","橫山鄉","尖石鄉","五峰鄉"];//新竹縣
department[9]=["東區","北區","香山區"];
department[10]=["苗栗市","頭份市","竹南鎮","後龍鎮","通霄鎮","苑裡鎮","卓蘭鎮","造橋鄉","西湖鄉","頭屋鄉","公館鄉","銅鑼鄉","三義鄉","大湖鄉","獅潭鄉","三灣鄉","南庄鄉","泰安鄉"];//苗栗縣
department[11]=["彰化市","員林市","和美鎮","鹿港鎮","溪湖鎮","二林鎮","田中鎮","北斗鎮","花壇鄉","芬園鄉","大村鄉","永靖鄉","伸港鄉","線西鄉","福興鄉","秀水鄉","埔心鄉","埔鹽鄉","大城鄉","芳苑鄉","竹塘鄉","社頭鄉","二水鄉","田尾鄉","埤頭鄉","溪州鄉"];//彰化縣
department[12]=["南投市","埔里鎮","草屯鎮","竹山鎮","集集鎮","名間鄉","鹿谷鄉","中寮鄉","魚池鄉","國姓鄉","水里鄉","信義鄉","仁愛鄉"];//南投縣
department[13]=["斗六市","斗南鎮","虎尾鎮","西螺鎮","土庫鎮","北港鎮","林內鄉","古坑鄉","大埤鄉","莿桐鄉","褒忠鄉","二崙鄉","崙背鄉","麥寮鄉","臺西鄉","東勢鄉","元長鄉","四湖鄉","口湖鄉","水林鄉"]//雲林縣
department[14]=["太保市","朴子市","布袋鎮","大林鎮","民雄鄉","溪口鄉","新港鄉","六腳鄉","東石鄉","義竹鄉","鹿草鄉","水上鄉","中埔鄉","竹崎鄉","梅山鄉","番路鄉","大埔鄉","阿里山鄉"];//嘉義縣
department[15]=["東區","西區"];
department[16]=["屏東市","潮州鎮","東港鎮","恆春鎮","萬丹鄉","長治鄉","麟洛鄉","九如鄉","里港鄉","鹽埔鄉","高樹鄉","萬巒鄉","內埔鄉","竹田鄉","新埤鄉","枋寮鄉","新園鄉","崁頂鄉","林邊鄉","南州鄉","佳冬鄉","琉球鄉","車城鄉","滿州鄉","枋山鄉","霧臺鄉","瑪家鄉","泰武鄉","來義鄉","春日鄉","獅子鄉","牡丹鄉","三地門鄉"];//屏東縣
department[17]=["臺東市","成功鎮","關山鎮","長濱鄉","池上鄉","東河鄉","鹿野鄉","卑南鄉","大武鄉","綠島鄉","太麻里鄉","海端鄉","延平鄉","金峰鄉","達仁鄉","蘭嶼鄉"];//台東縣
department[18]=["花蓮市","鳳林鎮","玉里鎮","新城鄉","吉安鄉","壽豐鄉","光復鄉","豐濱鄉","瑞穗鄉","富里鄉","秀林鄉","萬榮鄉","卓溪鄉"];
department[19]=["宜蘭市","頭城鎮","羅東鎮","蘇澳鎮","礁溪鄉","壯圍鄉","員山鄉","冬山鄉","五結鄉","三星鄉","大同鄉","南澳鄉"];
department[20]=["馬公市","湖西鄉","白沙鄉","西嶼鄉","望安鄉","七美鄉"];
department[21]=["金城鎮","金湖鎮","金沙鎮","金寧鄉","烈嶼鄉","烏坵鄉"];
department[22]=["南竿鄉","北竿鄉","莒光鄉","東引鄉"];
department[23]=["馬公市","湖西鄉","白沙鄉","西嶼鄉","望安鄉","七美鄉"];
function renew(index){
	for(var i=0;i<department[index].length;i++)
		document.myForm.member.options[i]=new Option(department[index][i], department[index][i]);	// 設定新選項
	document.myForm.member.length=department[index].length;	// 刪除多餘的選項
   

}
</script>

<?php
$user = 'root';
$pass= '';
$db=new mysqli('localhost',$user,$pass,'ex') or die("Unable to connect");
$db->set_charset("utf8");
//----------以上鏈接資料庫----------------------------------------------------------
if(isset($_POST["member"])){
$address = htmlspecialchars($_POST["member"]);
$temp = htmlspecialchars($_POST["country"]);
}
$county1="";
if(isset($_GET['value'])){
$autoAddress=htmlspecialchars($_GET['value']);
$split = str_split($autoAddress,3);
$temp=$split[3].$split[4].$split[5];
$address=$split[6].$split[7].$split[8];
}
if(!isset($temp) || !isset($address)){
	$temp="";
	$address="";
}
if($temp!=null || $address!=null){
  if($temp=="鄉鎮選取"){
   echo"<h1 align='center'>";
   echo "目前位置:請由上方選取縣市";
   echo"</h1>";
  }
  else{
   echo"<h1 align='center'>";
   echo "目前位置:".$temp.$address;
   echo"</h1>";
  }
}

if(isset($temp)){
	if($temp=="高雄市"){
		$county1='GaoXiongData';
	}
	else if($temp=="花蓮縣"){
		$county1='HuaLianData';
	}

	else if($temp=="基隆市"){
		$county1='JiLongData';	
	}
	else if($temp=="金門縣"){
		$county1='JinMenData';
	}
	else if($temp=="連江縣"){
		$county1='LianJiangData';
	}
	else if($temp=="苗栗縣"){
		$county1='MiaoLiData';
	}
	else if($temp=="南投縣"){
		$county1='NanTouData';
	}
	else if($temp=="澎湖縣"){
		$county='PengHuData';
	}
	else if($temp=="屏東縣"){
		$county1='PingDongData';
	}
	else if($temp=="台北市"){
		$county1='TaiBeiData';
	}
	else if($temp=="台東縣"){
		$county1='TaiDongData';
	}
	else if($temp=="台南市"){
		$county1='TaiNanData';
	}
	else if($temp=="台中市"){
		$county1='TaiZhongData';
	}
	else if($temp=="桃園市"){
		$county1='TaoYuanData';
	}
	else if($temp=="新北市"){
		$county1='XinBeiData';
	}
	else if($temp=="宜蘭縣"){
		$county1='YiLanData';
	}
	else if($temp=="雲林縣"){
		$county1='YunLinData';
	}
	else if($temp=="彰化縣"){
		$county1='ZhangHuaData';
	}
	else if($temp=="嘉義縣"or $temp=="嘉義市"){
		$county1='JiaYiData';
	}
	else if($temp=="新竹縣"||$temp=="新竹市"){
		$county1='XinZhuData';
	}
}
if($address!=null){
$sql = "SELECT * FROM $county1 WHERE area ='$address'";
$result = mysqli_query($db,$sql)or die(mysqli_error($db));
if(mysqli_num_rows($result)>0){//mysqli_num_rows($result),如果沒有找到資料回傳0，有資料回傳找到？筆資料。
	while($row = $result->fetch_assoc()){
                             $time=$row['time'];
				$weather=$row['weather'];
				$tem=$row['tem'];
				$TiGan=$row['TiGan'];
				$rain_p=$row['rain_p'];
				$wind=$row['wind'];
				$wind_d=$row['wind_d'];
				$hum=$row['hum'];
		echo "<table align='center' border='2' style='font-size:30px'>";
		echo "<tr><td>觀測時間：</td>";
		echo "<td>".$row['time']."</td></tr>";
		echo "<tr><td>所在區域：</td>";
		echo "<td>".$temp.$row['area']."</td></tr>";
		echo "<tr><td>天氣：</td>";
		echo "<td>".$row['weather']."</td></tr>";
		echo "<tr><td>溫度：</td>";
		echo "<td>".$row['tem']."</td></tr>";
		echo "<tr><td>體感溫度：</td>";
		echo "<td>".$row['TiGan']."</td></tr>";
		echo "<tr><td>降雨幾率：</td>";
		echo "<td>".$row['rain_p']."</td></tr>";
		if($row['wind_d']<4){
			echo "<tr><td style='background:#05EB5A'>";
		}
		else{
			echo "<tr><td style='background:#FF44AA'>";
		}
		echo "蒲福風級：</td>";
		if($row['wind_d']<4){
			echo "<td style='background:#05EB5A'>";
		}
		else{
			echo "<td style='background:#FF44AA'>";
		}
		echo $row['wind_d']."</td></tr>";
		echo "<tr><td>風向：</td>";
		echo "<td>".$row['wind']."</td></tr>";
		if($row['hum']<"60%"){
			echo "<tr><td style='background:#05EB5A'>";
		}
		else{
			echo "<tr><td style='background:#FF44AA'>";
		}
		echo "相對濕度：</td>";
		if($row['hum']<"60%"){
			echo "<td style='background:#05EB5A'>";
		}
		else{
			echo "<td style='background:#FF44AA'>";
		}
		echo $row['hum']."</td></tr>";
	}
	if($wind_d>3||$rain_p>"30%"){
		$answer="不適合飛行";
			}
	else {
		$answer="適合飛行";
			}
              echo "<tr><td>判斷結果：</td>";
              echo "<td>$answer</td></tr>";
              echo "<tr><td>禁航區查詢：</td>";
              echo "<td><a href='map.html'>點我查詢</a></td></tr>";
              echo"</table><br><br>";
}
}
?>
