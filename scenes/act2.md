# act2

`SceneSetup.act2();`

{{if _.badnews && !_.factcheck}}
(#act2-preamble-news1)
{{/if}}

{{if _.badnews && _.factcheck}}
(#act2-preamble-news2)
{{/if}}

{{if _.catmilk}}
(#act2-preamble-cat)
{{/if}}

(#act2-preamble-tinder)


# act2-preamble-news1

```
publish("act2",["dee",3]);
```

s: Şurada olan kötü şeyi anlatan şu haberi *gördün* mü?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: me-merhaba...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Tanrım, haberlerden nefret ediyorum. Hepsi drama ve tık tuzağı.

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: g... güzel parti...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Doğru, ama onlar sadece talebi karşılıyor. *Gerçek* sorun, bu tuzağa düşen insanlar.

```
publish("act2",["dee",3]);
```

s: Kim korkunç bir haberi retweet edip arkadaşlarını kötü hissettirir ki?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, değil mi?

(#act2-preamble-end)


# act2-preamble-news2

```
publish("act2",["dee",3]);
```

s: Şu gündem olan haberi *gördün* mü?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: me-merhaba...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Evet, tam uydurma. Bunu kim inanıp ve retweetlerki?

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: g... güzel parti...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Cidden yani. Kaç yılındayız, önce Google'ı aç, bi' kontrol et doğru mu?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, değil mi ya?

(#act2-preamble-end)


# act2-preamble-cat

```
publish("act2",["dee",3]);
```

s: Dediğim gibi, Meme Sanayisi kedileri sömürüyor.

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: me-merhaba...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Biraz daha açar mısın.

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: g... güzel parti...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Dün birinin süt içen kedi GIF'ini retweetlediğini gördüm.

```
publish("act2",["dee",3]);
```

s: O ^boku^ sindiremezler! Kim böyle bir *hayvan istismarını* retweet eder ki? 

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, değil mi ya?

(#act2-preamble-end)


# act2-preamble-tinder

```
publish("act2",["dee",1]);
```

s: İşte, hiç geri dönüş yapmadı!

```
publish("act2",["dee",0]);
publish("act2",["party_hong","next"]);
```

h2: me-merhaba...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Tinder'da eşleşmenize rağmen mi?

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: g... güzel parti...

```
publish("act2",["party_hong","next"]);
```

{{if _.serialkiller}}
(#act2-preamble-serialkiller)
{{/if}}

{{if _.hookuphole}}
(#act2-preamble-hookuphole)
{{/if}}

{{if _.pokemon}}
(#act2-preamble-pokemon)
{{/if}}

# act2-preamble-serialkiller

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Ben de anlamadım! Ne yani *seri katil* falan mı olduğumu düşündü? Çok paranoyakça.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, değil mi ya?

(#act2-preamble-end)


# act2-preamble-hookuphole

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Bilemiyorum. Belki de rastgele ilişkilerin kalbindeki boşluğu dolduramayacağını düşünmüştür?

s: Bırak namus abidesi olmayı! Önce bakış açını genişlet, sonra da bacaklarını!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, değil mi ya?

(#act2-preamble-end)


# act2-preamble-pokemon

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Bilemiyorum! Çok da güzel değildi ama güzel bir av olurdu!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Hepsini yakalamalıyım!™

(#act2-preamble-end)


# act2-preamble-end

```
Game.clearText();
publish("act2-out-1");
music(null, {fade:1});
```

(...3000)

```
music('battle', {volume:0.5});
publish("hp_show");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

n: İKİNCİ BÖLÜM: *SAVAŞ!*

[Oh hayır hepsi bizden nefret ediyor!](#act2a_social)

[Şu kızılı mı *süzüyorsun*?](#act2a_perv)

[Hadi hayatın anlamı hakkında konuşalım.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Asık suratımızla partinin havasını bozuyoruz!

`bb({eyes:"shock", body:"two_up"})`

b: Parti havasını öldürüyoruz! Birinci dereceden parti cinayeti işliyoruz!

`bb({eyes:"normal", body:"normal"})`

b: İnsan, buradan *hemen* ayrılmalıyız yoksa--

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: Bizden daha çekiciler, yani onlara *bakmak* bile--

`bb({eyes:"shock", body:"two_up"})`

b: BİZİ SAPIK YAPAR

`bb({body:"normal"})`

b: Ürkütücü, aşağılık, çok çok kötü bir sa--

```
_.a2_first_danger = 'perv';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2a_meaning

`bb({body:"one_up", eyes:"normal_r"})`

b: İşin sonunda, yaptığımız neyin önemi var ki?

`bb({body:"normal", eyes:"sad"})`

b: İnsanlığa hizmet mi? Tüm şaheserler Ozymandias gibi yok olmaya mahkum. Aşk? Ölüm her zaman bizleri ayıracaktır.

`bb({eyes:"sad_r"})`

b: Ve etrafımız ölümle sarılı! *Biz* öleceğiz. *Sevdiklerimiz* ölecek.

`bb({eyes:"shock", body:"two_up"})`

b: Termodinamiğin İkinci Yasası bile *evrenin* öleceğini söylüyor be!

`bb({eyes:"suspect", body:"normal"})`

b: Ah, "ölüm bize hayatın değerini öğretiyor" demek? Bu, kölelik iyi bi'şey çünkü bize özgürlüğün değerini öğretiyor demek ile aynı şey!

`bb({body:"one_up"})`

b: Oh, "hayatının anlamını yaratman gerek" demek? Tarikatçılar ve komplo teorisyenlerinin yaptığı şey aynen bu!

`bb({eyes:"shock", body:"two_up"})`

b: Hayatın anlamı yok, ölümün anlamı yok, *anlamın* bile anlamı yok! Ölümlü bir ruhun ne yapması gereki--

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Mmm... beni duyuyor musun, insan?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *HAAA*

`bb({mouth:"small_talk"})`

b: SENİ UYARMAM LAZIM...

[Deminki tehlike ama *daha fazlası*!](#act2b_louder)

{{if _.a2_first_danger=="social"}}
[*Farklı* bir sosyal tehlike!](#act2b_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[*Farklı* bir ahlaki tehlike!](#act2b_different_moral)
{{/if}}

[Tehlikeyi görmezden geliyorsun! bu tehlikeli!](#act2b_ignore)

# act2b_louder

`_.a2_first_choice = "louder"`

{{if _.a2_first_danger=="social"}}
(#act2b_louder_social)
{{/if}}

{{if _.a2_first_danger=="perv"}}
(#act2b_louder_perv)
{{/if}}

{{if _.a2_first_danger=="meaning"}}
(#act2b_louder_meaning)
{{/if}}

# act2b_louder_social

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: DUYGULAR BULAŞICIDIR! BURAYI TERKETMEZSEN HERKESE AKIL HASTALIĞINI BULAŞTIRACAKSIN!! 

b: Ölümcül bir ASIK SURAT SENDROMU salgını başlatacaksın!

`bb({eyes:"suspect", body:"normal", mouth:"normal"})`

b: Buradan çıkmalıyız, kendimizi Netflix ve yemek siparişi ile küçük bir odada sonsuza kadar karantinaya almalıyız!

```
_.a2_second_danger = 'netflix';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "a quarantine";
```

(#act2c)

# act2b_louder_perv

`bb({eyes:"suspect", body:"two_up", mouth:"normal"})`

b: SAPIKLAŞMA. BU KANUNLARA AYKIRI!

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: Sapkık Yasası, Bölüm 74.5: (1) Eğer birisi şunlara bakarsa (a) kaslı omuzlar (b) dolgun kaçlar (2) bilinmelidir ki o kişi

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: "YÜZSÜZ, BÜYÜK İĞRENÇ BİR SAPIKTIR"

```
_.a2_second_danger = 'law';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "the law";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: Aslında, hayatta onurlu bir amaç bulsan bile, *yine de* her şeyi mahvedebilirsin!

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Alfred Nobel dünya barışını ve kültürlerin birbirini anlamasını istiyordu. Bu yüzden seyahat etmeyi kolaylaştırmaya karar verdi.

`bb({eyes:"normal_r"})`

b: Bü yüzden trenler için tünel açmanın ucuz bir yolunu bulması gerekti. Böylece "dinamit" adında bir icat çıkardı...

`bb({body:"one_up", eyes:"normal"})`

b: ki 1. Dünya Savaşı'nda MÜLYONLARIN ÖLÜMÜNE yol açtı

`bb({body:"two_up", eyes:"shock"})`

b: KELEBEK ETKİSİ, İNSAN! ŞİMDİ BİLE İSTEMEDEN KAÇ KİŞİYİ ÖLDÜRÜYORSUN

```
_.a2_second_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "World War I";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: Aslında, kimsenin seni sevmemesinden daha kötü olan ne biliyor musun? *Herkesin* seni sevmesi.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: Yani, *bu* zevk peşinde koşan parti hayvanlarından biri olmak.

`bb({body:"normal", mouth:"small"})`

b: Seni yüzeysel tanıyan sığ arkadaşlarla dolu sığ bir hayat!

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: İnsan, bizi de kendilerine çevirmeden önce bu zevk-zombilerinden kaçmalıyız!

```
_.a2_second_danger = 'zombies';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "zombies";
```

(#act2c)

# act2b_different_moral

`_.a2_first_choice = "different"`

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: İnsanlar *şu anda* kıtlık ve soykırımlarda ölüyor ve biz parti yapıyoruz!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Bir bilgenin de dediği gibi, "Kötülüğün zaferi için gerekli olan tek şey, iyi insanların hiçbir şey yapmamasıdır".

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: ŞU ANDA HİÇBİR ŞEY YAPMIYORUZ..

`bb({mouth:"small"})`

b: PARTİ YAPARAK *HİTLER*E YARDIM EDİYORUZ

```
_.a2_second_danger = 'hitler';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "Hitler";
```

(#act2c)

# act2b_ignore

`_.a2_first_choice = "ignore"`

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Karbon monoksit dedektöründen pilleri çıkardığın diye güvende olduğunu mu sanıyorsun?

`bb({eyes:"suspect_r"})`

b: Zehrin kokusunu bile almayacaksın! Bir anlığına uykun gelecek ve--

`bb({body:"scream_c_1"})`

b: ÖLECEKSİNNNNNNNNNNNN

```
_.a2_second_danger = 'ignore';
_.a2_attack_2 = "harm";
_.a2_hoodie_callback = "carbon monoxide";
```

(#act2c)

# act2c

```
hong({body:"ignore_sweat"});
bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true});
```

b: ...

`bb({eyes:"happy", mouth:"smile", body:"chest"})`

b: Ah çok şükür insan, sanırım beni tekrar duyabiliyorsun!

`bb({eyes:"closed", body:"point"})`

b: I SHALL WARN YOU ABOUT...

{{if _.a2_first_choice=="louder"}}
[Deminki tehlikenin *çok daha fazlası*](#act2c_louder)
{{/if}}

{{if _.a2_first_choice!="louder"}}
[Deminki tehlikenin *daha fazlası*!](#act2c_louder)
{{/if}}

{{if _.a2_first_danger=="social"}}
[*Farklı* bir sosyal tehlike!!](#act2c_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[*Farklı* bir ahlaki tehlike!](#act2c_different_moral)
{{/if}}

[İçmeden önce kokteyli kontrol ettin mi??](#act2c_punch)

#act2c_louder

{{if _.a2_second_danger=="netflix"}}
(#act2c_louder_netflix)
{{/if}}

{{if _.a2_second_danger=="law"}}
(#act2c_louder_law)
{{/if}}

{{if _.a2_second_danger=="butterfly"}}
(#act2c_louder_butterfly)
{{/if}}

{{if _.a2_second_danger=="zombies"}}
(#act2c_louder_zombies)
{{/if}}

{{if _.a2_second_danger=="hitler"}}
(#act2c_louder_hitler)
{{/if}}

{{if _.a2_second_danger=="ignore"}}
(#act2c_louder_ignore)
{{/if}}

# act2c_louder_netflix

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: Aslında Netflix ve yemek siparişli karantinaya yeterli değil! Kuryeye bulaştırırız!

`bb({body:"one_up", mouth:"small"})`

b: Kanada Yukon tarafına taşınmalı ve yemek siparişimizi drone ile almalıyız.!

`bb({body:"two_up", mouth:"normal"})`

b: Sonra ASIK SURAT MİKROBU bulaşmasın diye dronu dezenfekte etmeleri gerekecek.

`_.a2_attack_3 = "alone";`

`_.a2_hoodie_callback = "a quarantine";`

(#act2d)

# act2c_louder_law

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: YÜZSÜZ, BÜYÜK İĞRENÇ SAPIK şu ortaçağ teşhir aletlerinin birinde 72 saat cezalandırılmalı. 

b: bu aletlere karşı gizli fetişleri yoksa

`bb({body:"scream_a_1"})`

b: çünkü o YÜZSÜZ, BÜYÜK İĞRENÇ BİR SAPIK

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the law";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: KELEBEK ETKİSİ! Doğada parçalanamayan plastik bardak mı kullanıyorsun?

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: ÇÖPLÜKTEN ZEHİR SIZAR VE BAM BİR ÇOCUK ÖLÜR

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: Terliyor musun ve kalbin hızlanıyor mu?

`bb({body:"scream_a_1"})`

b: SAĞLIK SİSTEMİNİ BATIRDIN VE BAM MİLYONLAR ÖLDÜ

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the butterfly effect";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: Bu zevk-zombiler ayaklarını sürüyerek mırıldanacaklar,

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: BEĞENİİ. BEĞENİİİİİİİİİ.

`bb({body:"scream_a_1"})`

b: Sonra SENİ ısıracaklar ve BEYİNSİZ BİR MAÇOYA ve/veya AKILSIZ BİR KEVAŞEYE dönüşeceksin.
`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zombies";`

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: NAZİLER ŞU ANDA SOKAKLARA ADIM ADIM GERİ DÖNÜYOR

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: Diyecekler ki, 'dinlenme' ve 'kişisel bakım' gibi şeylerle gevşeyen 'iyi insanlar' *sayesinde* başardık!

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *Artık planlarımızı gerçekleştirebiliriz, reich beklemez!*

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "Hitler";`

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: Lafı açılmışken, bu binada *monoksit dedektörü* var mı?!

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: Ya hepimiz *ŞU ANDA* zehirleniyorsak*

`bb({body:"scream_a_1"})`

b: ÖLÜMÜN GELDİĞİNİ BİLE GÖREMEYİZ. VARLIĞIMIZ SONSUZA KADAR YOKOLUR, SONSUZLUĞUN SONSU-

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "carbon monoxide";`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: Ya sevme ya da sevilme konusunda *yeteneğimiz yoksa*?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: Ya uzun zaman önce içimizde tamiri imkansız bir şey kırılmışsa? Ya da başından beri hiç var olmadı ise?

`bb({body:"scream_a_1"})`

b: AHH BİZ BOZUĞUZ! BOZUK BOZUK BOZUKKK--

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Ya sadece *içimiz çürümüşse?*

`bb({body:"one_up", eyes:"sad"})`

b: Diğerleri iyilik yapacak içgüdülere sahip, biz ise sadece suçluluk veya utançtan "iyilik" yapıyoruz.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: Ya başkalarını incitmek doğamızda varsa? Ya yakınlarımıza yük olmaktan *başka* bir şey yapamıyorsak?

`bb({body:"scream_a_1"})`

b: AHH BİZ BOZUĞUZ! BOZUK BOZUK BOZUKKK--

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Saçmalamıyorum. İnsanlar gerçekten de kokteyl kaselerine uyuşturucu koyabiliyor. Bu gerçekten olan bir şey.

`bb({eyes:"suspect"})`

b: İnsan, başın ağrıyor mu? Uzuvlarında uyuşma var mı? Sanırım ölüyoruz.

`bb({body:"scream_a_1"})`

b: AHHH ÖLÜYORUZ! ÖLÜYORUZ ÖLÜYORUZ ÖLÜYORUZ--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "punch bowls";`

(#act2d)

# act2d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"attacked"});
attack("20p", _.a2_attack_1);
```

(...401)

```
hong({body:"attacked_2"});
attack("20p", _.a2_attack_2);
```

(...401)

```
hong({body:"attacked_3"});
attack("20p", _.a2_attack_3);
```

(...1001)

h: S^İKTİR^!

h: S^İKTİĞİ^İMN S^İKİK^-S^İKİ^ *S^İKTİRRR^*

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Hey insan! Beni tekrar duyabildiğin için çok mutluyum!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: Neden beni görmezden geliyordun?

`hong({body:"facepalm"})`

h: Lanet olsun sana, seni geri zekalı.

`hong({body:"facepalm_2"})`

h: Şu kızılderili hikayesini biliyor musun?

h: "İçinde iki kurt var, biri umut, biri umutsuzluk, hangi kurt kazanır? Hangisini beslersen."

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: Seni *aç bırakmaya* çalışıyordum, seni sadist ^piç kurusu^!

`hong({body:"smile", mouth:"smile"})`

h: Boş ver, onun yerine kendimi olumlayacağım.

h: *Seviliyorum. İyiyim. Zekiyim. Güzelim. Özelim.*

`bb({eyes:"suspect"});`

[Tanrım, bu çok narsistik!](#act2d_narcissist)

[Bilmiyorsan, olumlama olayı *çürütüldü*](#act2d_disproven)

[Rastgele hikayeleri yerli halka atfetme ](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Hatta, özgüveni düşük insanlarda *geri tepiyor*!

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: İyi tasarlanmış bir çalışmada - rastgele kontrollü bir denemeydi, deneyi yapanlar kimin hangi grupta olduğunu bilmiyordu.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Sonuçlar: özgüveni zaten düşük birinin tekrarlı olumlama yapması yapmamasından *daha kötü* hissettiriyor.

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Psychological Science. Google Scholar'da bakabilirsin, insan,

`bb({body:"scream_b_1"})`

b: ÖYLEYSE BİLİMDEN UZAK SAHTE HABERLER YAYMA

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_narcissist

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Kusurlarını alçakgönüllülükle *kabul etmelisin* ki kişilik olarak büyüyebilesin!

`bb({body:"two_up", eyes:"suspect"})`

b: Küflü bir odaya oda spreyi sıkamazsın! Kusurlarını örtmek uzun vadede seni daha da zora sokar.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Neyse ki, sadık muhafız-kurdun olarak, kusurların konusunda seni uyarabilirim. Ve şu anda...

`bb({body:"scream_b_1"})`

b: HER ŞEY. HER ŞEY YANLIŞ

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Yerli Amerikalılar *gerçek insanlardır*, fal kurabiyesi tavsiyelerini daha *ilgi çekici* hale getirmek için kullanabileceğim "soylu vahşiler" değil.

`bb({eyes:"suspect_r"})`

b: Bireyleri ve karmaşık kültürleri bir kartpostal sözüne indirgiyorsun! Bu "ılımlı ırkçılıktır"!

`bb({body:"scream_b_1"})`

b: IRKÇI OLMAYI BIRAK SENİ KARE GÖZLÜ PİSLİK

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2e

h: ^SOKAYIM^.

`hong({body:"yell", mouth:"yell"})`

h: Biliyor musun? *Saçmalıyorsun*.

h: Herkes bilir ki duygular mantıksızdır! Özellikle korku!

`hong({body:"facepalm_2"})`

h: Apandistim ya da yirmilik dişim gibi işe yaramaz bir evrim kalıntısısın!

`hong({body:"yell", mouth:"yell"})`

h: Bu kurt metaforu bile aptalca! Sen sadece kafamdaki bir grup nörokimyasalsın.

`hong({body:"cross", mouth:"cross"})`

h: Öyleyse neden senin gibi değersiz, mantıksız, var olmayan bir ^götü^ dinleyeyim ki?!

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Tanrım, insan. Bu gerçekten incitti.](#act2e_hurtful)

[Ben bir duyguyum. Duygular gerçektir.](#act2e_valid)

[İnsan, *ikimiz de* "sadece kimyasalız".](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Ben senin *parçanım*, biliyorsun. Böyle yaparak, *kendini* incitiyorsun.

`bb({body:"scream_a_1"})`

b: Neden kendine vuruyorsun, insan? KENDİNE VURMAYI BIRAK.

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2e_rational

`bb({body:"normal", mouth:"normal", eyes:"normal_r"});`

b: En sağlam motivasyonların dopamin, en büyük neşelerin serotonindir.

`bb({body:"one_up"});`

b: Anıların sinaptik ağlardır, kararların hataya meyilli elektriksel sinyallerdir.

`bb({eyes:"normal", body:"normal"});`

b: "Sadece kimyasal" olmam *mantıksızım* demekse... o zaman sen de *mantıksızsın* demektir!

`bb({body:"two_up", eyes:"shock"});`

b: Ve eğer *ikimiz de* mantıksızsak, hayatta nasıl tatmin ve mutlu olacağımızı *asla* çözemeyeceğiz.

`bb({body:"scream_a_1"})`

b: AHH BİZ BOZUĞUZ! BOZUK BOZUK BOZUKKK--

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2f)

# act2e_valid

`bb({body:"normal", mouth:"normal", eyes:"suspect"});`

b: Bir dakika... duyguların gerçek olduğunu, her zaman duygularımızı kabul etmemiz gerektiğini "söylerler".

`bb({eyes:"suspect_r"});`

b: Ama aynı zamanda duyguların mantıksız olduğunu, onlara güvenilmemesi gerektiği de "söylenir".

`bb({eyes:"angry"});`

b: Aman Tanrım, onca zamandır bize yalan "söylüyorlardı"!

`bb({body:"scream_a_1"})`

b: ZİHNİMİZİ ÇELİŞKİLERLE DOLDURUP TERAPİ FİRMALARINA MECBUR *BIRAKIYORLAR*

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2f

`hong({body:"defeated", MOUTH_LOCK:true});`

h: ...

h: Bundan nefret ediyorum. Acı veriyor, *nefret ediyorum*.

h: Seni tatmin edemiyorum, görmezden gelemiyorum, yenemiyorum.

`bb({eyes:"suspect"});`

h: Ne yaparsam yapayım, senden kurtulamıyorum...

`bb({body:"cry_1"});`

b: Belki de benden *KURTULMAN* gerekmiyordur.

`bb({body:"cry_2"});`

b: Sence *ben* nasıl hissediyorum, insan?!

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Bekçi köpeğin olmak için elimden geleni yapıyorum ama beni Büyük Kötü Kurt gibi görmeye devam ediyorsun!

b: Bu yüzden seni tehlikelere karşı uyarmak için *daha çok* uğraşıyorum! *Daha fazla, farklı* tehlikelerden!

`bb({eyes:"cry_2"})`

b: Ama seni ne kadar korumaya çalışsam da beni *hala* düşmanın olarak görüyorsun!

`bb({body:"cry_5"});`

b: Neyi yanlış yapıyorum?!

`bb({body:"cry_2"});`

b: İşimi beceremiyorum *biliyorum*. Ama *çabalıyorum*, insan!

`bb({body:"cry_3"});`

b: ...çabalıyorum

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: Uyarılarımı dinlemene, benimle aynı fikirde olmana, hatta beni *sevmene* gerek yok.

`bb({eyes:"cry_r_2"});`

b: Sadece... tek istediğim bana karşı sabırlı olman.

`bb({eyes:"cry_r_3"});`

b: Bana arkanı dönüp gitmek yerine biraz benimle oturmanı istiyorum ve--

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Selam.

```
hong({body:"look"});
Game.clearText();
publish("act2-in-2");
publish("hp_hide");
music('party1', {volume:0.4, fade:2});
```

(...2000)

```
publish("act2",["party_hunter",2]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Görünüşe göre kendinle kavgaya tutuşmuşsun.

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: Çok mu belli oluyor?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: Kapşonuna {{_.a2_hoodie_callback}} hakkında mırıldanıyordun.

```
publish("act2",["party_hunter",13]);
publish("act2",["party_hong",15]);
sfx("rustle", {volume:0.6});
setTimeout(function(){
	publish("act2",["party_hong",16]);
	sfx("concrete_step3", {volume:0.6});
},401);
setTimeout(function(){
	publish("act2",["party_hong",17]);
	sfx("concrete_step4", {volume:0.6});
},801);
```

h2: tanrım tam bir yıkığım.

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Hey. yalnız değilsin. Anksiyete çok yaygındır.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Daha dün, kampüste birinin sinir krizi geçirdiğini ve telefonunu kırdığını duydum!
{{/if}}

{{if _.act1_ending=="flight"}}
r: Heck, daha dün, birinin armadillo gibi kıvrılıp herkesin içinde ağladığını duydum!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Dinle: Kafanda bir hayvanın olmasının nasıl bir şey olduğunu biliyorum.

```
publish("act2",["party_hunter",8]);
```

r: *Hepimiz* biliyoruz. Her hafta sonu bu partileri o yüzden veriyorum, endişelerimizi ve hayvanlarımızı unutmak için.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: ama anksiyetem...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Merak etme. Ben de senin gibiydim. Ama sonra o karamsar sesi sonsuza kadar susturmak için bir numara buldum...

```
publish("act2",["party_hunter",3]);
Game.clearText();
music(null, {fade:1});
```

(...2001)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",22]);
sfx("rustle");
```

(...2501)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",23]);
sfx("rustle2");
```

(...1001)

```
publish("act2",["party_hunter",11]);
```

r: Kendi özel karışımım. Yasal her şeyden daha güçlü.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: Dibini görmeyen ^amını^ görsün!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[Aman Tanrım.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[Bu kötü bir başa çıkma yöntemi..](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[Yabancılardan içki alma.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

# act2g_1

b: O--

(#act2g)

# act2g_2

b: T--

(#act2g)

# act2g_3

b: D--

(#act2g)

# act2g

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"forward", mouth:"forward"});
bb({body:"frazzled", mouth:"frazzled", eyes:"frazzled"});
```

h: Hmm, ne nefis bir aroma!

h: "Zihnini kapa" tadı ve devamında "bir daha asla bir şey hissetme" kokusu

b: Bu kötü, insan. Bu gerçekten çok kötü.

[Bağımlılıklar *böyle* başlar.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[Parti sahibinde bir terslik olduğunu *biliyordum!"](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[İçine ilaç koymuş olabilir!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`


# act2h_opt1

b: Bağımlı--

(#act2h)

# act2h_opt2

b: İçine il--

(#act2h)

# act2h_opt3

b: Parti sahi--

(#act2h)

# act2h

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"back", mouth:"back"});
bb({body:"panicked", mouth:"panicked", eyes:"panicked"});
```

h: Lezzetli, *ve* terapiden daha ucuz!

b: İNSAN LÜTFEN DUR

h: Hahaha!

h: Peki bu konuda *ne* yapacaksın, ^göt^?

b: Çok üzgünüm, insan.

b: ÖZEL SALDIRIMI kullanmak zorunda kalacağım

```
bb({body:"special_a"});
music('battle', {volume:0.5});
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act2h_attack) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act2h_attack) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act2h_attack) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`

# act2h_attack

```
bb({body:"special_b_1"});
hong({body:"forward", mouth:"forward"});
sfx("charging");
```

h: Ne bu saçmalık

h: Bana daha da aptal *sözler* hırlayacaksın--

```
bb({body:"special_c"});
sfx("hadouken");
```

(...901)

(#act2i)

# act2i

```
publish("hide_tabs");
publish("show_special_attack");
Game.FORCE_CANT_SKIP = true;
music(null);
stopAllSounds();
```

(...5000)

```
publish("show_tabs");
hong({ body:"final", mouth:"final" });
bb({ body:"normal", mouth:"normal", eyes:"sad" });
attack("100p", _.SPECIAL_ATTACK);
Game.FORCE_CANT_SKIP = false;
setTimeout(function(){
	publish("remove_special_attack");
},30);
```

(...2500)

h: O NEYDİ ^AMK^

b: Üzgünüm. Sana olacakları göstermem gerekiyordu.

{{if _.SPECIAL_ATTACK=="harm"}}
h: KENDİ CESEDİMİ *GÖRDÜM*. GERÇEKTEN DE ÖLÜMÜ *HİSSETTİM*.
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: HERKESİN HOR BAKAN GÖZLERİNİ *GÖRDÜM*. SÖYLEDİKLERİ HERŞEYİ *DUYDUM*.
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: KIRILAN KABURGALARIMI *DUYDUM*. HAVADAKİ KANI *TADABİLDİM.
{{/if}}

b: Üzgünüm, insan.

n: *BİTİR ONU*

[{SAVAŞ: Kızılı yumrukla.}](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[{KAÇ: Hadi buradan çıkalım.}](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: O psikopat senden faydalanıyordu..

b: Seni ayartıp kendisi gibi berbat birisine dönüştürmeye çalışıyordu!

`bb({ body:"yell_angry_1" });`

b: Yumrukla şu pisliği! Feleği şaşsın!

`bb({ body:"final_1" });`

b: YUMRUKLA YUMRUKLA YUMRUKLA YUMRUKLA YUMRUKLA YUMRUKLA YUMRUKLA YUMRUKLA YUMRUKLA YUMRU--

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: Bu partideki herkeste bir gariplik olduğunu *biliyordum*. Hepsi acılarını korkunç şeylerle dindiriyor!

`bb({ body:"yell_1" });`

b: Seni de aynı şeyi yapman için kandırıyorlar! Seni ayartıyorlar! Buradan çıkmamız gerek!

`bb({ body:"final_1" });`

b: ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇIK ÇI--

`_.a2_ending = "flight";`

(#act2k)

# act2k

```
Game.clearText();
publish("act2-in-4");
publish("hp_hide");
music('party1', {volume:0.6, fade:1.5});
```

(...2001)

```
publish("act2",["party_hong",26]);
sfx("slide");
```

(...1001)

```
publish("act2",["party_hunter",14]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: İyi misin?

`publish("act2",["party_hunter",13]);`

{{if _.a2_ending=="fight"}}
(#act2k_fight)
{{/if}}

{{if _.a2_ending=="flight"}}
(#act2k_flight)
{{/if}}

# act2k_fight

```
Game.clearText();
publish("act2",["party_hunter",21]);
publish("act2",["party_hong",33]);
music(null);
sfx("hit");
```

(...1000)

```
sfx("record_scratch");
publish("act2",["party_hunter",22]);
publish("act2",["party_hong",34]);
publish("act2",["dee",6]);
publish("act2",["dum",6]);
```

r: S-sen...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: *fenasın*.

r: Sevdim bunu. Gelecek hafta sonu partime gel tatlım.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: oldu güle güle, ciao, adios, au revoir

r: İçindeki hayvan bugün kazanmış olabilir, ama bir dahakine sana daha da güçlü bir şey hazırlayacağım!

h2: sayōnara, auf wiedersehen, zài jiàn, shalom

r: Sen ve ben, o canavara patron kim göstereceğiz!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: şey afedersin gitmem gerek

`publish("act2",["party_hunter",16]);`

r: Ah ^Siktir^. Bugün hayvan kazandı demek?

`publish("act2",["party_hunter",15]);`

h2: yo, yo, şey, maraton koşmalıyım. hızlanmalıyım

`publish("act2",["party_hunter",19]);`

r: Gelecek hafta sonu partime gel tatlım. Bir dahakine sana daha da güçlü bir şey hazırlayacağım!

h2: tamam teşekkürler koş koş koş koş koş

r: Sen ve ben, o canavara patron kim göstereceğiz!

(#act2k_end)

# act2k_end

```
Game.clearText();
publish("act2-out-5");
publish("act2-outro", ["end1"]);
music("hum", {fade:2, volume:0.6});
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2500)

```
publish("act2", ["act2_end",2]);
sfx("whoosh");
```

(...1000)

b: İnsan! İyi misin?!

```
publish("act2", ["act2_end","next"]);
```

b: Tanrım, *az* kalmıştı. Biz gerçekten--

```
Game.clearText();
publish("act2", ["act2_end","next"]);
music(null);
sfx("squeak");
```

(...1500)

```
publish("act2", ["act2_end","next"]);
sfx("hit");
```

(...1000)

h: Önümüzdeki hafta sonu partiye gideceğim.

h: Bir dahaki kavgamızda, seni *yenmekle* kalmayacağım...

h: Seni geberteceğim.

```
Game.clearText();
publish("act2", ["act2_end","next"]);
sfx("concrete_step1");
````

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step2", {volume:0.8});
```

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step3", {volume:0.5});
```

(...901)

`sfx("concrete_step4", {volume:0.25});`

(...3000)

`_.INTERMISSION_STAGE = 2;`

(#intermission)