# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (game auto-saved)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *ahh*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Yani bu hikayeden çıkarılacak sonuç neydi?

`hong({body:"one_up", eyes:"annoyed"})`

h: Ne *öğrendik*? *Ben* aptaldım, "arkadaşlarım" *beni* kullanıyordu, ve neredeyse ölüyorduk.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Evet, hastane faturalarından bahsetmiyorum bile.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Evet, karaciğer hasarından bahsetmiyorum bile.](#act4a_liver)
{{/if}}

[Evet, bu en kötü senaryoydu.](#act4a_worst)

[Evet, ben haklıydım.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Doğru. Sigorta planımın "aptal olmayı" kapsadığını sanmıyorum.

`hong({eyes:"annoyed", mouth:"normal"});`

b: Ama yine de... hayatta kaldık!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Kesinlikle ömrümüzden birkaç yıl eksilttik...

`bb({eyes:"surprise"});`

b: Ama en azından hala bir yaşam umudumuz var! Hayatta kaldık!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: Ve an azından...

h: Hm?

`bb({eyes:"surprise"});`

b: Hayatta kaldık!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Ama... Sen de haklıydın.

`hong({eyes:"surprise"});`

h: Hm?

`bb({eyes:"normal"});`

b: Ben kurt diye ağlayan kurttum, ve sen – haklı olarak – bana inanmadın.

`bb({eyes:"surprise_r"});`

b: Ve en azından, hayatta kaldık!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Her şeye rağmen, hala buradayız.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Az önce ölüme yakın bir deneyim yaşadığımızı düşünürsek oldukça sakin görünüyorsun.
{{/if}}

{{if !_.INJURED}}
h: Az önce ölüme *yakın* bir deneyim yaşadığımızı düşünürsek oldukça sakin görünüyorsun.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Eh, diğer her şeyi kıyasladığında daha az korkunç yapıyor. Ayrıca bu beni de düşündürdü.

`bb({eyes:"normal", mouth:"normal"});`

b: Eğer seninle savaşırsam iyi olmaz, çünkü bu seni korumuyor...

h: Ama benim seninle savaşmam *da* kötü, çünkü bu seni daha da bağırtıyor...

`bb({eyes:"normal_r"})`

b: o zaman, belki...

`bb({eyes:"normal"})`

h: Belki savaşmamız gerekmez.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: Ben Büyük Kötü Kurt değilim. Ama ben bir muhafız-kurt da değilim.

`bb({eyes:"sad_d"})`

b: Ben hırpalanmış bir barınak köpeğiyim.

`bb({eyes:"sad"})`

b: Zor şeyler atlattık. Belki travma ya da ihmal edilmek, bu yüzden bazen aşırı tepki verir ve giderim:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: HAV HAV HAV HAV HAV

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: *Korkak* bir köpek olmak istemiyorum! Seni korumak istiyorum! İyi bir köpek olmak istiyorum!

`bb({eyes:"sad", mouth:"normal"});`

b: İnsan... bu kurdu evcilleştirmeye yardım edecek misin?

`hong({eyes:"sad"})`

h: Ben... deneyeceğim.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Tamam. Duygularla sağlıklı ilişkiler kurmalıyız. İlişkilerin iletişime ihtiyacı var. Bu yüzden, iletişim kuralım.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: Önümüzdeki beş dakika kulağa çok sevimsiz gelecek ama başarana kadar deneyelim.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Sevgili içimdeki kurt... nasıl hissediyorsun?

n2: TOPLAM KULLANILAN KORKULAR:

n2: *İNCİNMEK* {{_.attack_harm_total}}, *SEVİLMEMEK* {{_.attack_alone_total}}, *KÖTÜLENMEK* {{_.attack_bad_total}}

n2: İLK KONUŞMAK İSTEDİĞİN KORKU HANGİSİ? (DİĞERLERİNİ SONRA YAPABİLİRSİN)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Bizim incineceğimizden korkuyorum.](#act4_harm)

[Yalnız kalacağımızdan korkuyorum.](#act4_alone)

[Kötü biri olduğumuzdan korkuyorum.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Fiziki güvenliğini korumak istiyorum,

`bb({eyes:"sad_d"})`

b: Ama *bütün dünya* tehlikeli görünüyor. Çok fazla felaket ve kötülükle dolu.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Bilmem, bundan sonra ne söyleyeceğini seçmek *bana* yeter. *Sen* ne diyorsun, insan?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Tekrar, sana dönersek insan, Ne düşünüyorsun?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Başka düşüncelerin var mı, insan?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Haklısın. O zaman birbirimizi koruyalım.](#act4_harm_skills)

[Kendimizi daha fazla tehlikeye maruz bırakalım.](#act4_harm_exposure)

[Teşekkür ederim.](#act4_thanks) `_.thanks_for = "fiziksel güvenliğim";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Ama... nasıl? Benim dişlerim ve pençelerim var ama ben sadece metaforum.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Kendimizi korumayı mı öğreneceğiz? Birbirini koruyan bir topluluğa mı katılacağız? Genel sağlığımızı ve kişisel sınırlarımızı mı iyileştireceğiz?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Belki, ama...

[Nereden başlayacağız?](#act4_harm_skills_start)

[Eğer hâlâ işe yaramazlarsa?](#act4_harm_skills_work)

[Ya "güvenlik" konusunda aşırıya kaçarsak?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: Yapılacak çok şey var, kendimiz hakkında düzeltmemiz gereken çok şey var. Nereden *başlıyoruz*?

`hong({ body:"shrug", eyes:"surprise" })`

h: Şimdi işe koyuluyoruz.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Eh?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Şu an iyi bir iletişim pratiği yapıyoruz. Bu daha az yanlış pozitif ile tehlikeyi daha iyi tespit etmemize yardımcı olur,

`hong({ eyes:"surprise" });`

h: Ve *bu* bizi incinmekten koruyacak!

`hong({ eyes:"normal", mouth:"normal" });`

h: Bu nedenle: bu *bir* kendini savunma eğitimidir.

`bb({ eyes:"normal_r" })`

b: Huh. Daha fazlasını bekliyordum:

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: Doğru, kendimizi %100 korumanın bir yolu yok...

`hong({ body:"one_up" });`

h: Ama %1'lik bir iyileştirme bile bir anlamı var, değil mi?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Sen bardağı %99 boş değil, %1 dolu olarak görüyorsunuz.

`bb({ eyes:"normal" });`

h: Eğer bir çölde mahsur kaldıysan o suyun hâlâ değeri vardır.

`bb({ eyes:"closed" });`

b: Pekala. O zaman dibine kadar içerim.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Yani, bunca zaman benim uyarılarımı görmezden gelme sebebin *benim* güvenlik konusunda aşırıya kaçmamdı! 

`bb({ body:"normal", eyes:"normal" })`

h: Haklısın. Güvenliği ölçülü şekilde yapmak isteriz. Her şeyi ölçülü şekilde yapmalıyız.

`bb({ eyes:"suspect" })`

b: Pardon, *HER ŞEYİ* Mİ?

`hong({ eyes:"annoyed" })`

h: *Mâkul sayıdaki şeyleri* ölçülü yapmalıyız.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Sözlerinde tekrarlı bir şekilde tutarlı olduğun için teşekkür ederim.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *NE*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Demek istediğim, diyelim ki köpek gök gürültüsünden korkuyor.

`hong({ body:"hands_1" });`

h: Eğitmenlerin kullandığı bir numara, gök gürültüsü kısık bir sesle kaydedilir ve köpeğe sakinleşmesi için ödül olarak verilir.

`hong({ body:"hands_2" });`

h: Birkaç gün boyunca eğitmen, köpek gök gürültüsü korkusunu yenene kadar sesi azar azar yükseltir.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Buna mazur kalma teorisi denir!

`hong({ body:"point", eyes:"normal" });`

h: Köpek olduğundan beri, senin için de geçerli, değil mi? Tüm memeliler aynı ya savaş-ya kaç tepkisine sahiptir.

`hong({ body:"normal" });`

[Ya *fazla* duyarsızlaştırırsak?](#act4_harm_exposure_overboard)

[Ya *gerçek* bir tehlikeye maruz kalırsak?](#act4_harm_exposure_hurt)

[Ben bir kurtum, köpek değil.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: Ben de sana evcilleştirilip sevimli bir yavru köpek olana kadar nezaket ve sabır göstereceğim.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Aaaw.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: Korkunuzu *tamamen* kapatırsanız neler olduğunu gördük - kendinizi *gerçekten* tehlikeli durumlara sokarsınız.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Ayrıca, *fazla* duyarsızlaştırma bizi psikopatlara dönüştürmez mi?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Yakında enfiye cinayeti pornosu izlerken kendimize ikramlarda bulacağız!

`hong({ eyes:"annoyed" })`

h: Bence... bununla gök gürültüsü arasında ince bir çizgi var.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Ama tam olarak *neresi*, insan? *Neresi?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: Bilmiyorum. Ama *sen* bana yardım edebilirsin!

`hong({ eyes:"normal", body:"normal" })`

h: Seninle çalışarak ve tartışarak o çizgiyi çizeceğiz.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Tamam. Ama benim çizebileceğim başparmaklarım yok, bu yüzden çizimi sen yapmalısın.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: Örneğin: biz o lanet olasıca *çatıdan* atladık!
{{/if}}

{{if !_.INJURED}}
b: Örneğin: biz neredeyse o lanet olasıca *çatıdan* atlayacaktık!
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Haklısın. Bazen fazla ileri *gidilebilir*.

`hong({ eyes:"normal" });`

h: Ama bu yüzden, eğer maruz bırakma terapisi yaparsak, küçük başlayacağız ve yukarı doğru küçük adımlar atacağız.

h: *Gerçek* tehlikeye çarpmadan hemen önce dururuz.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Evet, yüksek sesli gök gürültüsü duymakla, uzun sivri bir şapkayla fırtınada durmak arasındaki çizgiyi belirliyorum.

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: Bekle, hissettiklerimin lehinde veya aleyhinde görüşün yok mu? Sadece... "teşekkür ederim" mi?

`hong({ eyes:"surprise", body:"shrug" })`

h: Evet! {{_.thanks_for}} hakkında endişelendiğin için teşekkür ederim.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Sen iyi misin?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Bana daha önce hiç *teşekkür ederim* dememiştin.

`hong({ mouth:"smile" });`

h: Aw seni büyük, tüylü, panik kurt.

(#act4_something_else)

# act4_thanks_2

h: Aşırı tepki versen bile, {{_.thanks_for}} hakkında ilgilendiğin için minnetarım.

`bb({ eyes:"annoyed" })`

b: Bekle... Bu korkular hakkında konuşmaktan kaçınmak için sadece "teşekkür ederim" demiyorsunuz, değil mi?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Şey, işler karmaşık ve her zaman hazır cevaplarım olmuyor.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Normalde hayat size önceden hazırlanmış 3 diyalog yanıtı listesi vermez.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Ama şimdilik, en azından teşekkür edebilirim.

b: Pekala, beni sabırla dinlediğin için de teşekkür ederim.

`bb({ eyes:"closed" });`

b: Seni küçük tüysüz memeli.

(#act4_something_else)

# act4_thanks_3

h: Havlaman beni korkutsa bile, {{_.thanks_for}} hakkında korumaya çalışıyorsun.

`bb({ eyes:"smile_r" });`

b: Pekala, beni böyle pohpohlamaya devam edersen internet bizim hakkımızda tuhaf fikirler edinecek.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h:Hadi ama, ben lise çağında savunmasız bir çocuğum ve sen büyük, korkunç bir kurtsun. En kötüsü ne-

`hong({ eyes:"normal", body:"point" });`

h: Aslında, buna cevap verme.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: O derin, insani ait olma ihtiyacını karşıladığından emin olmak istiyorum....

`bb({ eyes:"sad_u" });`

b: Ama eğer birileri bizi - *gerçek* bizi- tanısaydı, hepsini korkutup kaçırırdık diye endişeleniyorum.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Bilmiyorum, artık ne söyleyeceğimi seçmek *bana* yeter. *Sen* ne diyorsun, insan?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Tekrar, sana dönersek insan. Ne düşünüyorsun?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Başka düşüncelerin var mı, insan?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Katılıyorum: hadi sosyal hayatımız üzerinde çalışalım.](#act4_alone_skills)

[Bence insanlar bizi seviyor.Hadi bunu ortaya çıkaralım. ](#act4_alone_experiment)

[Teşekkür ederim.](#act4_thanks) `_.thanks_for = "sosyal aidiyetim";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Soru sorma, dinleme ve empati kurma, açık ve savunmasız olma gibi becerileri pratik yapabilir miyiz?

`hong({ eyes:"normal_l" });`

h: Veya arkadaşlarla zaman planlamak, düzenli olarak buluşmalara gitmek gibi daha iyi sosyal alışkanlıklar?

`hong({ body:"one_up" });`

h: Ayrıca reddedilme konusunda daha rahat olmayı öğrenebiliriz.

`hong({ eyes:"normal" });`

h: Ya da insanların bizi reddetmediğini, sadece yorgun olduklarını veya Dinlenen ^Kaltak^ Yüzüne sahip olduklarını öğrenebiliriz.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Çok fazla seçenek var. Ama, "sosyal becerileri öğrenmek" hakkında...

[Bu *çıkar amaçlı* değil mi?](#act4_alone_skills_manipulative)

[Bu bizi *manipüle etmeyi* kolaylaştırmaz mı?](#act4_alone_skills_manipulated)

[Ya hâlâ başarısız olursak?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Kurbanlarının duygularını okuyabilen seri katiller "empati" konusunda harika değiller mi?

`bb({ eyes:"annoyed" });`

b: Charles Manson arkadaşlar kazanmadı mı ve insanları etkilemedi mi?

`hong({ eyes:"annoyed", body:"chin" });`

h: Evet, haklısın.

h: "Sosyal beceriler", insanları gerçekten *önemsemiyorsak* hiçbir şey ifade etmez.

`hong({ body:"normal" });`

h: Kısaca, sadece ^oruspu çocuğu^ olma.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: İşte tam orada motive edici bir poster yazısı.

`hong({ body:"shrug", mouth:"narrow" });`

h: “^Oruspu Çocuğu^™ Olma.”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: İnsanlar ayaklarını üzerimize silerken Lütfen ve Teşekkürler diyerek Hoş Geldiniz paspası olacağız!

`bb({ mouth:"scream", eyes:"scream" })`

b: Çok fazla ^kıç^ öpeceğiz ki, kahverengi ruj sürüyormuşuz gibi görünecek!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Haklısın."Sosyal beceriler" yalnızca başkalarını memnun etmekle ilgili olamaz, aynı zamanda *sınırlar* belirlemekle de ilgili olmalıdır.

`hong( body:"one_up" });`

h: Evimizi ayakta tutacak duvarlarımız yoksa başkalarını evimize davet edemeyiz.
```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: Ayrıca... re: o ruju aklımda canlandırdım da... *ıyy??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Başarısız olabiliriz. Aslında, başarısız *olacağız*.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: Ve bu iyi! Başarısızlık, herkesin ilk olarak öğrenmesi gereken bir şeydir!

`hong({ body:"normal", eyes:"normal" });`

h: O zaman birlikte başarısız olalım, tamam mı?

`bb({ eyes:"normal_r" });`

b: Tabii, sanırım... en kötü senaryo, şehirden gidip yeni bir kimlik alabiliriz.

`bb({ eyes:"normal" });`

h: Evet, sanırım bu günlerde sadece iki bitcoine mâl oluyor.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Tecrübe kazanabiliriz!

`hong({ body:"chin" });`

h: Bir arkadaşa takılmak için ping atabiliriz, eski bir dostla yeniden bağlantı kurabiliriz, hâttâ baristayla sohbet bile edebiliriz.

`hong({ body:"normal" });`

h: Sanırım sandığımızdan daha sevimli olduğumuzu görebiliriz.

`bb({ eyes:"annoyed" });`

[Ya bunlar küçük, ucuz "kazançlar" ise?](#act4_alone_experiment_cheap)

[Ya bu başkalarına yükse?](#act4_alone_experiment_burden)

[Ama bu *gerçek* biz değiliz!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Eğer yüzeysel bir gülümseme takınırsak, asla kimseyle gerçekten bağlantı kuramayız,

`bb({ eyes:"super_sad" });`

b: *Ama* eğer içimizi açarsak, diğer insanlar içimizdeki tüm pisliği görecek!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Yuvarlan.

b: Ne.

`hong({body:"hands_1"})`

h: Köpekler sevgi ve güven göstermek istediklerinde, göbeklerini açığa çıkararak kendilerini savunmasız hale getirirler.

`hong({body:"one_up"})`

h: Belki *henüz* savunmasız olacak kadar güvende değiliz ama yeterli eğitimle,

`hong({body:"normal", eyes:"surprise"})`

h: Bir gün insanlara gerçek bizi gösterebiliriz - tamamen berbat, tamamen insan.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Bana bir ziyafet verirsen yuvarlanırım.

`bb({ eyes:"normal", mouth:"normal" });`

h: Hayır.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Baristaya "merhaba" demek, Sosyal Kelebek Olimpiyatları'nda tam olarak altın madalya performansı değil.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Sadece *bizim* için!

`hong({ body:"one_up", eyes:"annoyed" });`

h:Sosyal arenada tüy siklet bile değiliz, daha çok... kuark ağırlığı gibiyiz.

`hong({ body:"normal", eyes:"normal" });`

h: Küçük, ucuz kazançlarla başlamamız gerekiyorsa, öyle olsun. 1000. adımdan önce 1. basamağı tırmanmanız gerekiyor.

b: Evet! Belki "Merhaba" dedikten sonra, şöyle devam edebiliriz...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Nasılsınız?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Daha fazla olmaz!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Belki barista sadece biraz kahve yapmak istiyor, sosyal becerilerimizin kötü olup olmadığını görmek için *deney* olmak istemiyor.

`bb({ eyes:"annoyed" })`

h: Eh, eğer *bir yük olduğumuz* ortaya çıkarsa...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Bunu bilmek de güzel!

`hong({ eyes:"normal" });`

h: Daha sonra, insanlara neyin rahat olduğunu önetkin olarak nasıl soracağımızı, başkalarının sınırlarını bilmeyi ve saygı duymayı öğrenebiliriz.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Bilirsiniz, danışman broşürlerinde gördüğümüz tüm o "kişiler arası beceriler" saçmalık.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Daha iyi bir insan olma yolundaki moral refahını savunmak istiyorum.

`bb({ eyes:"sad_d" })`

b: Ama derinlerde bir yerdeymiş gibi geliyor, temelde çok... kırılmışız.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: Ve bana berbat olmadığımızı söyleme. Bir *çatıdan* atladık.
{{/if}}

{{if !_.INJURED}}
b: Ve sakın bana berbat olmadığımızı söyleme. Neredeyse bir *çatıdan* atlıyorduk.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: Bilmiyorum, artık ne diyeceğimi seçmek *bana* yeter. *Sen* ne diyorsun, insan?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Yine sana dönelim, insan. Sen ne düşünüyorsun?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Başka düşüncelerin var mı, insan?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Yani biz bozulduk. Hadi bizi düzeltelim.](#act4_bad_fix)

[Yani biz bozulduk. Bunu kabul etmeliyiz.](#act4_bad_accept)

[Teşekkür ederim.](#act4_thanks) `_.thanks_for = "Moral refahım";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Yavaş yavaş daha iyi alışkanlıklar edinebilir, hayatımızı değer verdiğimiz şeylerle daha uyumlu hale getirebiliriz.

`hong({body:"one_up"});`

h: Ve gerekirse, bir terapist veya danışman gibi profesyonel yardım alabiliriz.

`hong({body:"normal"});`

h: Bizi düzeltmenin yolları var.

[Ya hepsini düzeltemezsek?](#act4_bad_fix_cant)

[Ya *çok* fazla düzeltirsek?](#act4_bad_fix_too_much)

[Profesyonel yardım almaya gücümüz yetmez.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Evet, sanırım haklısın.

h: Hepsini düzeltemeyiz.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ahhh biliyordum her zaman bozuk kalacağız!

`hong({eyes:"surprise"});`

h: Ama en azından *daha az* bozuk olabiliriz.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Yaralar zamanla iyileşir ama asla geçmezler. Sorun değil.

`bb({eyes:"annoyed_r"});`

b: Sanırım. Bunun dışında,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Yaralar *seksidir.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Lütfen, bunu yapma.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Bunu kabul etmek mide bulandırıcı ama... bir parçam bu rahatsızlığa sahip olmayı *istiyor*.

`bb({ eyes:"angry" })`

b: Yani, onsuz, *sıkıcı* olmayacak mı?

`bb({ eyes:"sad_r", body:"one_up" })`

b: Bozukluk olmadan sanatımız bayat ve yavan olmaz mı?
`bb({ eyes:"sad_u", body:"two_up" })`

b: Bozukluk olmadan, bozukluğu olan arkadaşlarımızla bağlantı kuramaz mıyız?
`bb({ eyes:"sad", body:"chest" })`

b: Hayattan memnun kalırsak, kendimizi harika şeyler yapmaya zorlamayı bırakır mıyız?
`hong({ MOUTH_LOCK:true })`

h: ...

h: Eğer korkarsak... "korkuların bitmesi"...

h: Korkularımızın biteceğini sanmıyorum.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Oh, Evet! Vay! Ne büyük bir rahatlama!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: Doktorun sadece "*bu seni nasıl hissettiriyor?*" dediğini duymak için saatte 100 dolar ödüyorum diye endişeliyim. 

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Mm-hmm. Bu seni nasıl hissetiriyor?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Evet, bu tamamen makul bir endişe.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: Ve akıl sağlığının pek çok insan için uygun olmaması gerçekten berbat.

`hong({ eyes:"normal", mouth:"normal" });`

h: Yine de bazı ucuz veya ücretsiz seçenekler var:

`hong({ body:"chin" })`

h: Destek grupları, çevrimiçi terapi, öğrenci/kar amacı gütmeyen sağlık merkezleri...

`hong({ body:"hands_1" })`

h: Meditasyon yapmak, iyi uyumak, arkadaşlarla düzenli olarak sohbet etmek, yeni şeyler öğrenmek gibi alışkanlıklar geliştirmek...

`hong({ body:"hands_2" })`

h: Kanıta dayalı psikoterapiler için çalışma kitapları ödünç almak için bir kütüphaneye gitmek...

`hong({ body:"one_up" })`

h: Bu oyunun sonunda kaynakların tam listesi var!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Peki *o* dördüncü duvar pek uzun sürmedi.

`hong({ body:"point" });`

h: Bazı şeyler anlatı geleneğinden daha önemlidir. Ruh sağlığı gibi.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Yani, terapistlerin söylediği bu değil mi? Tüm duygularınızı, olumsuz olanları bile kabul ediyor musunuz?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Bekle.

["Kabul etmek" yani *vazgeçmek mi*?](#act4_bad_accept_give_up)

["Kabul etmek" yani *razı olmak* mı?](#act4_bad_accept_approve)

["Kabul etmek" yani *ciddiye almak* mı?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Sence Martin Luther King, "Otobüsün önünde oturamayız, hadi *kabul edelim*" diyebilir miydi?

`bb({ eyes:"angry_r", body:"two_up" });`

b: Kendi Kendine Yardım Sanayi Kompleksi neden beyaz bayrak sallamanın *derin bir bilgelik* olduğunu düşünüyor?

`bb({ eyes:"annoyed", body:"normal" });`

h: Bence terapistler kötü şeyleri "kabul etmek" anlamına gelir: onların var olduğunu ve değiştirilmesinin zor olduğunu kabul etmek,

h: Ama illâki değişim sözünden vazgeçmek değil.

`bb({ eyes:"suspect" });`

b: O zaman terapistler *onaylamalı*, *kabul etmemeli*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Evet, düşününce "kabul etmek" biraz kafa karıştırıcı.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Peki, *onaylıyorum.*

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Sanki bozuk olmamız *iyi* bir şey mi? Hayır!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Akıl hastalığını romantikleştiren tüm o salak Hollywood senaristleri pisliklerle dolu!
`bb({ eyes:"angry", body:"two_up" });`

b: Akıl hastası olmak *berbat!* İnsanların *hayatlarını* çalıyor! Bunu neden "kabul edelim"?!

`bb({ body:"normal" });`

h: Bence terapistler duygularımızı "kabul etmek" anlamına gelir: onlara karşı sabırlı ol.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Tıpkı bataklıkta mücadele etmenin sizi nasıl daha hızlı batırdığı ve çözümün sabırla dümdüz uzanmak olduğu gibi,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Sana karşı savaşmak, korkum, çatıdan atlamama neden oldu.
{{/if}}

{{if !_.INJURED}}
h: Sana karşı savaşmak, korkum, neredeyse çatıdan atlamama sebep olacaktı.

`hong({ body:"normal", eyes:"normal" });`

h: Bunun yerine çözüm, şu anda yaptığımız şeyi yapmaktır – savaşmak değil, sabırla birlikte olmaktır.

`bb({ eyes:"annoyed" });`

b: O zaman "kabul et" gibi sorunlu bir kelime yerine *bunu* demeliler.

`hong({ body:"chin", eyes:"annoyed" });`

h: Evet, biraz düşününce, "kabul etmek" berbat bir şey.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: "kabul etmeyi" kabul etmiyorum.

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Ama zaten beni ciddiye almadığını *biliyoruz*.

`bb({ eyes:"sad_u", body:"two_up" });`

b: Bütün *sorun* sana yardım etmek istemem ama bunu yapmak için kelimeleri kullanmakta berbatım!

`bb({ eyes:"sad", body:"normal" });`

h: Bence terapistler duygularınızı "kabul etmek" anlamına gelir: "savaşmayın ya da onları görmezden gelmeyin."

`hong({ eyes:"surprise", body:"one_up" });`

h: Sizi dinlemek için *sizinle* çalışın ama söylediklerinizi %100 gerçek olarak algılamayın.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: O zaman terapistler "kabul et" gibi belirsiz, kafa karıştırıcı bir kelime yerine *bunu* söylemelidir.

`hong({ body:"chin", eyes:"annoyed" });`

h: Sanırım onlar da kelimeleri kullanmakta berbatlar.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Neyse, konuşmak istediğin başka bir şey var mı?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Peki, dertli kalbinde başka bir şey var mı?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Bizim incineceğimizden korkuyorum.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Yalnız kalacağımızdan korkuyorum.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Kötü biri olduğumuzdan korkuyorum.](#act4_bad)
{{/if}}

[Hayı, şuanlık iyiyim.](#act4c_prelude)

# act4_something_else_2

h: Tamam, sanırım artık tüm korkularımız hakkında konuştuk.

b: Evet, sadece üç korku vardı.

h: Evet, kesinlikle üç.

b: Pratik.

(#act4c)

# act4c_prelude

h: İyi sohbetti, takım.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: Bu bir *oyun* değil, biliyorsun.

`bb({eyes:"angry_d", body:"one_up"})`

b: Duygularınızla sağlıklı bir ilişki kurmak, ekrandaki düğmelere tıklamak kadar kolay değildir.

`bb({eyes:"sad", body:"normal"})`

b: *Gerçekten anlaşabilir miyiz?

b: *Bir ekip olarak birlikte çalışabilir miyiz?

`hong({eyes:"sad", body:"one_up"})`

h: Şey,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: A-affedersiniz...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: Ö-öğ-öğle yemeğindee seninle oturmamın bir sakıncası var mı?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *Bu* senin hoşlandığın kişi mi? Neden psikopat bir seri katil gibi yalnız oturuyorlar?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Hoşlandığın kişiye onlarla oturabilir misin diye mi soruyorsun?, Kulağa ne kadar *muhtaç* geldiğini biliyor musun?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *Bu* senin hoşlandığın kişi mi? Onların huzurlarını ve sesizliğini bozduk! Öyle bir yüküz ki!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: Ben-yani-, bu sorun değilse, ben sadece...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Bekle, seni partide görmedim mi?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Evet tabi ki! Buraya gel.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Üzgünüm, şu anda yalnız kalmaya ihtiyacım var.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Evet, kanepedeydin! İlk partiye gittiğimde oradaydın.

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Panik atak geçirip ev sahibine yumruk attığım yer.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Panik atak geçirip ağlayarak dışarı çıktığım yer.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Biraz bekle insan, onları rahatsız ediyor olabiliriz.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, seni olay yerine koymak istemiyorum!

`publish("act4", ["hong_to_alshire",4]);`

h2: Sadece dostça bir yüzü hatırladım, hepsi bu.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH BİLİYORDUM! ONLAR TEHLİKELİ PANİK-ATAK PSİKOPATLAR!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH İLK İZLENİMİ OLARAK "TRAVMAMA TANIK OLDU" DEDİ! BU, BİZDEN NEFRET ETTİLER DEMEKTİR!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH BİRİLERİNİ TRAVMATİK BİR OLAYI HATIRLATTIK. SADECE VARLIĞIMIZ BAŞKALARINA ZARAR VERİR.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Biraz bekle insan, onlar rahat görünmüyorlar.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, elbette baskı yok!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Sadece söylüyorum, istersen burada oturabilirsin.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: *ÇOK* DOSTU OLUYORLAR! TIPKI SERİ KATİL TED BUNDY GİBİ!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: SADECE GÜZEL OYNUYORLAR! KİMSE *GERÇEKTEN* BİZE YAKIN OLMAK İSTEMİYOR!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH HER ZAMAN BAŞKALARINI HUZURSUZ HİSSETTİRİYORUZ! DÜNYA ÜZERİNDEKİ BİR LEKEYİZ!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Biraz bekle insan, onları rahatsız ediyor olabiliriz.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, kaba olmak istememiştim!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Sadece duygularımı işlemek için biraz zamana ihtiyacım var. Lütfen bunu kişisel bir reddetme olarak algılamayın.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: NE HASTA, BÜYÜK DÜŞÜNCELER İŞLENİYORLAR?! BU PSİKOPATIN KALBİNİ HANGİ KARANLIK İSTEKLER DOLUYOR?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: KİŞİSEL OLARAK REDDEDİLDİK! ASLA SEVİLMEYECEĞİZ!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: DUYGUSAL İŞLEMLERİNİ KESTİK! ŞİMDİ SONSUZA KADAR TRAVMATİK OLACAKLAR VE HEPSİ BİZİM SUÇUMUZ!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: KAÇ KAÇ KAÇ KAÇ KAÇ KAÇ KAÇK KAÇ KAÇ KAÇ KAÇ KAÇ KAÇ KAÇ KAÇ

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: Huh. Bu tuhaftı.. Kafalarından neler geçtiğini merak ediyorum.

`publish("act4", ["hong_closer", 2]);`

h: Her neyse, ne diyordun?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Uh, unuttum? Takım olmak ve çalışmakla ilgili bi şeylerdi?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Sanki duygularınız *savaş suçlusu*ymuş gibi duygularınızla "barış" yapmanız gerektiğini söylüyorlar.

`publish("act4", ["bb_closer", 7]);`

b: Ama sadece barıştan *daha fazlasını* yapmamızı istiyorum! *müttefik* olmamızı istiyorum!

`publish("act4", ["bb_closer", 3]);`

b: İyi bir bekçi köpeği olmak istiyorum. Tıpkı açlık ve susuzluğun fiziksel ihtiyaçlarınız için alarm olması gibi,

`publish("act4", ["bb_closer", 8]);`

b: *Psikolojik* ihtiyaçlarınız için alarm olmak istiyorum – güvenlik, ait olma, iyilik ihtiyaçlarınız.

`publish("act4", ["bb_closer", 1]);`

b: Ama... İşimi berbat ediyorum, bu yüzden beni eğitmene ihtiyacım var.

`publish("act4", ["bb_closer", 4]);`

b: Ben "her zaman geçerli" veya "her zaman mantıksız" değilim. Ben sadece... elimden geleni yapıyorum. Yani lütfen,

`publish("act4", ["bb_closer", 30]);`

b: Sana yardım etmeme yardım et!

`publish("act4", ["bb_closer", 6]);`

b: Yine de, yaşlı bir köpeğe yeni numaralar öğretmek biraz zaman alacaktır. Belki *yıllar.*

`publish("act4", ["bb_closer", 3]);`

b: Ve bazen nüksedeceğim, eski alışkanlıklarıma kayacağım.

`publish("act4", ["bb_closer", 2]);`

b: Gölgelere havlayacağım. Seni kelimelerle korkutacağım. Hatta size bazı şeylerin... bazı rahatsız edici görüntülerini gösterebilirim.

`publish("act4", ["bb_closer", 9]);`

b: Üzgünüm! Ben hırpalanmış bir barınak köpeğiyim! Hırpalanmış köpekler bazen yatağınıza kaka yapar!

`publish("act4", ["bb_closer", 4]);`

b: Ama eğer bana karşı sabırlıysan... sadece kal ve benimle otur...

`publish("act4", ["bb_closer", 8]);`

b: Belki bu kurdu evcilleştirebilirsin.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[İyi köpek.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[İyi insan.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: AAAAA SEN HÂLÂ YALNIZ YİYORSUN, ONBEŞ SİGARA AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA YEMEK YERKEN HALA VERİMLİ DEĞİLSİN BİZ TOPLUM PARAZİTLERİYİZ AAAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA SEN DAHA FAZLA BEYAZ EKMEK YİYORSUN AAAAA
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: HAV HAV HAV HAV HAV

(#credits)
