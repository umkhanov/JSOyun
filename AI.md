# AI Kullanımı <br>

Kullanılan Yapay Zeka Araçları :<br>
ChatGPT (OpenAI)<br>
Claude AI <br>

Promptlar ve Alınan Cevaplar :<br>

**Soru 1:** <br>
Canvas üzerinde karakterin yerçekimi etkisiyle düşmesini nasıl sağlayabilirim?<br>

Cevap:<br>
Karakterin y konumunu her karede belli bir hızla arttırarak yerçekimi etkisini simüle edebilirsin. <br><br>
Örnek:<br>
javascript:<br>
<pre>let gravity = 0.5;
let velocityY = 0;

function update() {
    velocityY += gravity;
    character.y += velocityY;
}</pre>

<br>——————————————————————————————————————————————————————————<br>

**Soru 2 :** <br>
"JavaScript Canvas kullanarak basit bir platform oyunu yapmak istiyorum. 
<br>Oyuncu karakteri sürekli sağa hareket edecek ve yolda boşluklar olacak. 
<br>Bu boşlukları doldurmak için sürüklenebilir bloklar kullanacağım.
<br>Temel yapıyı nasıl kurmalıyım?"<br><br>
Cevap:<br>
"Canvas tabanlı bir platform oyunu için şu temel yapıyı öneriyorum:

Canvas Kurulumu: 800x600 boyutunda bir canvas oluşturun<br>
Component Sistemi: Oyun nesneleri için genel bir component fonksiyonu yazın<br>
Game Loop: setInterval ile sürekli güncellenen bir oyun döngüsü<br>
Koordinat Sistemi: X ekseninde sürekli kaydırma efekti için speedX kullanın<br>

Temel yapı şöyle olabilir:<br>
javascript : <br>
<pre>var myGameArea = {
    canvas : document.createElement("canvas"),
    start : function() {
        this.canvas.width = 800;
        this.canvas.height = 600;
        this.context = this.canvas.getContext("2d");
        this.interval = setInterval(updateGameArea, 20);
    }
};</pre><br>
Component fonksiyonunuzda update() ve newPos() metodları olsun."

<br>——————————————————————————————————————————————————————————<br>

**Soru 3 :** <br>
"Oyunuma arkaplan müziği ve efekt sesleri eklemek istiyorum. <br>HTML5 Audio API'sini nasıl kullanmalıyım? Ses dosyalarını nasıl kontrol edebilirim?"<br><br>
Cevap:<br>

JavaScript'te kontrol<br>

<pre>// Arkaplan müziği başlat<br>
document.getElementById("bgMusic").play();

// Efekt sesi çal
function playSound(soundId) {
    let sound = document.getElementById(soundId);
    sound.currentTime = 0; // Başa sar
    sound.play();
}

// Ses seviyesi ayarla
sound.volume = 0.3; // 0.0 - 1.0 arası</pre><br>
Oyun bittiğinde müziği durdurmayı unutmayın: 
<pre>bgMusic.pause(); 
bgMusic.currentTime = 0;</pre>

<br>——————————————————————————————————————————————————————————<br>

**Diğer sorular :**
Dosyaya yazdıklarımın dışında yapay zekaya başka küçük sorular da sordum.
