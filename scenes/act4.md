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

h: Ne *öğrendik*? Ben *aptaldım*, "arkadaşlarım" beni *kullanıyordu*, ve neredeyse *ölüyorduk*.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Hastane faturalarından bahsetmiyorum bile.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Karaciğer hasarından bahsetmiyorum bile.](#act4a_liver)
{{/if}}

[Evet, bu kötü durum senaryosuydu.](#act4a_worst)

[Evet, ben haklıydım.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Doğru. Sigortamın "aptal olmamı" karşılayacağını sanmıyorum.

`hong({eyes:"annoyed", mouth:"normal"});`

b: Ama yine de... kurtulduk!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Kesinlikle hayatımızdan birkaç yıl eksilttik...

`bb({eyes:"surprise"});`

b: Ama en azından hala bir hayatımızı *var*! Hayatta kaldık!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: Ama yine de...

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

b: Ben yalancı çobanlık yapan bir *kurttum*. Ve *gerçek* tehlike geldiğinde doğal olarak bana inanmadın.

`bb({eyes:"surprise_r"});`

b: Ama yine de, hayatta kaldık!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Her şeye rağmen, hala buradayız.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Ölümün eşiğinden döndüğümüzü düşünürsek oldukça sakin görünüyorsun.
{{/if}}

{{if !_.INJURED}}
h: Ölümün eşiğinin *eşiğinden* döndüğümüzü düşünürsek oldukça sakin görünüyorsun.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Eh, diğer her şey nispeten daha az korkunç geliyor artık. Ayrıca beni düşünmeye de itti.

`bb({eyes:"normal", mouth:"normal"});`

b: Seni korumamı engellediği için seninle dövüşmem kötü ise...

h: Ama seninle dövüşmem sadece seni daha da çok bağırttığı için kötüyse...

`bb({eyes:"normal_r"})`

b: o zaman, belki...

`bb({eyes:"normal"})`

h: Belki dövüşmek zorunda değilizdir.

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

b: Ben büyük kötü bir kurt değilim. Ama ben bir muhafız-kurt da değilim.

`bb({eyes:"sad_d"})`

b: Ben hırpalanmış bir barınak köpeğiyim.

`bb({eyes:"sad"})`

b: Zor şeyler atlattık. Adına travma ya da yalnızlık de. Bu yüzden bazen aşırı tepki veriyorum ve:

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

h: Tamam. Duygularla sağlıklı ilişkiler. İlişkilerin iletişime ihtiyacı var. Hadi, iletişim kuralım.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: Bu beş dakika kulağa oldukça zorlama gelecek ama yolun sonunu görene kadar gidelim.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Sevgili içimdeki kurt... nasıl *hissediyorsun*?

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

b: Fiziksel güvenliğini korumak istiyorum,

`bb({eyes:"sad_d"})`

b: Ama *bütün dünya* tehlikeli görünüyor. Çok fazla felaket ve kötülükle dolu.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: *Ben* yeterince konuştum, *sen* ne düşünüyorsun, insan?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Peki ya sen insan, sen ne düşünüyorsun?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Ekleyeceğin bi'şey var mı, insan?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Haklısın. O zaman birbirimizi koruyalım.](#act4_harm_skills)

[Kendimizi tehlikeye daha da maruz bırakalım.](#act4_harm_exposure)

[Teşekkür ederim.](#act4_thanks) `_.thanks_for = "fiziksel güvenliğim";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Ama... nasıl? Dişlerim ve pençelerim var, ama sadece bir metaforum.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Kendimizi korumayı öğrenebiliriz, birbirini koruyan bir topluluğa mı katılabiliriz, sağlığımızı ve kişisel sınırlarımızı iyileştirebiliriz.

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Belki, ama...

[Nereden başlayacağız?](#act4_harm_skills_start)

[Ya yine de başaramazsak?](#act4_harm_skills_work)

[Ya "güvenlik" konusunda aşırıya kaçarsak?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: Yapılacak çok şey var, kendimiz hakkında düzeltmemiz gereken çok şey var. Nereden *başlıyoruz*?

`hong({ body:"shrug", eyes:"surprise" })`

h: Tam da şimdi başlıyoruz.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Ne?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Şu an doğru iletişim pratiği yapıyoruz. Daha kolay tehlikeleri farkedeceğiz, yanlış alarmlar azalacak, 

`hong({ eyes:"surprise" });`

h: Ve *bu* bizi incinmekten koruyacak!

`hong({ eyes:"normal", mouth:"normal" });`

h: Bu nedenle: bu *bir* savunma eğitimi.

`bb({ eyes:"normal_r" })`

b: Huh. Ben daha çok şundan bekliyordum:

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

h: Ama %1'lik bir iyileşme bile bir ilerlemedir, değil mi?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Sen bardağı %99 boş değil, %1 dolu olarak görüyorsun.

`bb({ eyes:"normal" });`

h: Çölde mahsur biri için o suyun hâlâ değeri vardır.

`bb({ eyes:"closed" });`

b: Pekala. Dibini görelim o zaman.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Yani, bunca zaman beni görmezden gelme sebebin *benim* güvenlik konusunda aşırıya kaçmamdı! 

`bb({ body:"normal", eyes:"normal" })`

h: Haklısın. Güvenliğin bile ölçülüsünü isteriz. Her şeyi ölçülü şekilde yapmalıyız.

`bb({ eyes:"suspect" })`

b: Pardon, *HER ŞEYİ* Mİ?

`hong({ eyes:"annoyed" })`

h: *Mâkul sayıdaki şeyleri* ölçülü yapmalıyız.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Sözlerini, birbirini destekler şekilde yaptığın için teşekkürler.

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

h: Buna mazur kalma terapisi denir!

`hong({ body:"point", eyes:"normal" });`

h: Sen de bir köpeksin, sende de işe yaramalı, değil mi? Tüm memeliler aynı davranır, kaç veya savaş.

`hong({ body:"normal" });`

[Ya *fazla* duyarsızlaşırsak?](#act4_harm_exposure_overboard)

[Ya *gerçek* bir tehlikeye maruz kalırsak?](#act4_harm_exposure_hurt)

[Ben bir kurtum, köpek değil.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: Ben de sana evcilleştirilip sevimli bir yavru köpek olana kadar nezaket ve sabır göstereceğim.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Aaay.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: Korkunu *tamamen* kapatırsan neler olduğunu gördük - kendini *gerçekten* tehlikeli durumlara soktun.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Ayrıca, *fazla* duyarsızlaştırma bizi psikopata dönüştürmez mi?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Sonra da kendimizi enfiye cinayeti pornosu izleyerek ödüllendireceğiz!

`hong({ eyes:"annoyed" })`

h: Bence... bununla gök gürültüsü arasında bir çizgi var.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Ama tam olarak *nerede*, insan? *Nerede?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: Bilmiyorum. Ama *sen* bana yardım edebilirsin!

`hong({ eyes:"normal", body:"normal" })`

h: Seninle çalışarak ve tartışarak o çizgiyi çizeceğiz.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Ama benim başparmaklarım yok, bu yüzden çizimi sen yapmalısın.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: Örneğin: o lanet olasıca *çatıdan* atladık!
{{/if}}

{{if !_.INJURED}}
b: Örneğin: o lanet olasıca *çatıdan* neredeyse atlayacaktık!
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Haklısın. Bazen fazla ileri *gidilebilir*.

`hong({ eyes:"normal" });`

h: İşte bu yüzden, maruz bırakma terapisi ile küçük başlayıp yukarı doğru küçük adımlar atacağız.

h: *Gerçek* tehlikeye çarpmadan hemen önce duracağız.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Evet, gök gürültüsü duymakla, uzun sivri bir şapkayla fırtınada durmak arasında bir çizgi çiziyorum.

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

b: Bekle, destekleme veya karşı çıkma yok mu? Sadece... "teşekkür ederim" mi?

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

b: Bekle... Korkular hakkında konuşmaktan kaçmak için "teşekkür ederim" demiyorsun, değil mi?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Şey, işler karmaşık ve her zaman hazır cevaplarım olmuyor.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Hayat sana 3 seçenekten ibaret diyaloglar vermiyor sonuçta.

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

b: Aidiyetlik hissinin karşıladığından emin olmak istiyorum..

`bb({ eyes:"sad_u" });`

b: Ama korkum o ki, eğer birisi bizi - *gerçek* bizi - tanırsa korkup kaçar.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: *Ben* yeterince konuştum, *sen* ne düşünüyorsun, insan?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Peki ya sen insan, sen ne düşünüyorsun?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Ekleyeceğin bi'şey var mı, insan?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Katılıyorum: sosyal hayatımız üzerinde çalışalım.](#act4_alone_skills)

[Bence insanlar bizi seviyor. Hadi deneyelim?](#act4_alone_experiment)

[Teşekkür ederim.](#act4_thanks) `_.thanks_for = "sosyal aidiyetim";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Soru sorma, dinleme ve empati kurma, açık ve savunmasız olma gibi becerileri pratik yapabilir miyiz?

`hong({ eyes:"normal_l" });`

h: Veya arkadaşlarla plan yapmak, düzenli buluşmalara gitmek gibi daha iyi sosyal alışkanlıklar?

`hong({ body:"one_up" });`

h: Ayrıca reddedilmekten daha az etkilenmeyi,

`hong({ eyes:"normal" });`

h: Ya da insanların bizi reddetmediğini, sadece yorgun olduğunu anlamayı öğreniriz

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Çok fazla seçenek var. Ama, "sosyal beceriler öğrenmek" hakkında...

[Bu *manipülatif* değil mi?](#act4_alone_skills_manipulative)

[Bu bizi *manipülatif* birisi yapmaz mı?](#act4_alone_skills_manipulated)

[Ya hâlâ başarısız olursak?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Kurbanlarının duygularını okuyabilen seri katiller "empati" uzmanı değiller mi?

`bb({ eyes:"annoyed" });`

b: Charles Manson arkadaşlar edinip insanları etkilemedi mi?

`hong({ eyes:"annoyed", body:"chin" });`

h: Evet, haklısın.

h: İnsanları *önemsemiyorsak* "sosyal becerilerin" anlamı olmaz.

`hong({ body:"normal" });`

h: Kısacası ^oruspu çocuğu^ olma.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: İşte tam motive edici bir poster başlığı

`hong({ body:"shrug", mouth:"narrow" });`

h: "^Oruspu Çocuğu^™ Olma."

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: İnsanların ayaklarını sildiği, "Lütfen" ve "Teşekkürler" diyen bir kapı paspası olacağız!

`bb({ mouth:"scream", eyes:"scream" })`

b: O kadar ^kıç^ öpeceğiz ki, kahverengi ruj sürmüşüz gibi görünecek!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Evet. "Sosyal beceriler" sadece başkalarını memnun etmek değildir, *sınırlar* belirlemekle de ilgilidir.

`hong( body:"one_up" });`

h: Evimizin kirişleri olmadan başkalarını evimize davet edemeyiz.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: Ayrıca... o ruju aklımda canlandırdım da... *tatsız??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Başarısız olabiliriz. Aslında, başarısız *olacağız*.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: Sıkıntı değil! Yeni bi'şey öğrenmenin ilk adımı başarısızlıktır!

`hong({ body:"normal", eyes:"normal" });`

h: O zaman birlikte başarısız olalım, tamam mı?

`bb({ eyes:"normal_r" });`

b: Tabii, sanırım... en kötü şehirden kaçıp yeni bir kimlik alabiliriz.

`bb({ eyes:"normal" });`

h: Evet, sanırım bu günlerde sadece iki bitcoine mâl oluyor.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Denemeler yapabiliriz!

`hong({ body:"chin" });`

h: Takılmak için gözümüze bir arkadaş takarız, eskilerden birileri ile konuşabiliriz, ya da baristayla.

`hong({ body:"normal" });`

h: Sanırım sandığımızdan daha sevimli olduğumuzu farkedebiliriz.

`bb({ eyes:"annoyed" });`

[Ya bunlar küçük, ucuz "zaferlerse"?](#act4_alone_experiment_cheap)

[Ya bu başkalarına yük olursa?](#act4_alone_experiment_burden)

[Ama ufak muhabbetler *gerçek* biz değiliz!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Boş bir gülümseme takınırsak, asla kimseyle gerçekten bağlantı kuramayız,

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

h: Köpekler sevgi ve güven göstergesi olarak karınlarını savunmasız bırakırlar.

`hong({body:"one_up"})`

h: Belki *henüz* göbeğimizi açacak kadar güvende hissetmiyoruz ama yeterli eğitimle,

`hong({body:"normal", eyes:"surprise"})`

h: Bir gün insanlara gerçek bizi gösterebiliriz - berbat, insan.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Bana bir ödül verirsen yuvarlanırım.

`bb({ eyes:"normal", mouth:"normal" });`

h: Hayır.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Baristaya "merhaba" demek altın madalyalık bir olimpiyat performansı değil.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: *Bizim* için öyle!

`hong({ body:"one_up", eyes:"annoyed" });`

h:Sosyal arenada tüy siklet bile değiliz, daha çok... kuark siklet.

`hong({ body:"normal", eyes:"normal" });`

h: Küçük zaferlerle başlamamız gerekiyorsa, öyle olsun. 1000. adımdan önce elbet 1. adımı atmamız gerek.

b: Evet! Belki "Merhaba" dedikten sonra, şöyle devam edebiliriz...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Nasılsınız?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Fena değil!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Belki barista sosyal beceri *deneğimiz* olmak istemiyordur, sadece kahve yapmak istiyordur.

`bb({ eyes:"annoyed" })`

h: Eh, eğer bir *yük* olduğumuzu farkedersek...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Bunu bilmek de güzel!

`hong({ eyes:"normal" });`

h: İnsanların nasıl rahat olduğunu öğrenmeyi ve başkalarının sınırlarına saygı duymayı öğrenebiliriz.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Bilirsin, danışman broşürlerinde gördüğün o "kişiler arası beceriler" saçmalığı.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Daha iyi bir insan olmanı sağlayacak ahlaki ihtiyaçlarını korumak istiyorum,

`bb({ eyes:"sad_d" })`

b: Ama derinlerde bir yerde, temelde çok... bozuğuz.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: Ve bana bozuk *olmadığımızı* söyleme. Bir *çatıdan* atladık.
{{/if}}

{{if !_.INJURED}}
b: Ve bana bozuk *olmadığımızı* söyleme. Neredeyse bir *çatıdan* atlıyorduk.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: *Ben* yeterince konuştum, *sen* ne düşünüyorsun, insan?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Yine sana dönelim, insan. Sen ne düşünüyorsun?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Ekleyeceğin bi'şey var mı, insan?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Madem bozuğuz, hadi kendimizi düzeltelim.](#act4_bad_fix)

[Madem bozuğuz, hadi bunu kabul edelim.](#act4_bad_accept)

[Teşekkür ederim.](#act4_thanks) `_.thanks_for = "Ahlaki sağlığım";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Yavaş yavaş daha iyi alışkanlıklar edinebilir, hayatımızı hizaya sokabiliriz.

`hong({body:"one_up"});`

h: Ve gerekirse, bir terapist veya danışman gibi bir uzmandan yardım alabiliriz.

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

b: Bunu kabul etmek iğrenç ama... bir parçam bu rahatsızlığa sahip olmak *istiyor*.

`bb({ eyes:"angry" })`

b: Yani, onsuz, *sıkıcı* olmayacak mıyız?

`bb({ eyes:"sad_r", body:"one_up" })`

b: Bu bozukluk olmadan mizacımız bayat ve yavan olmaz mı?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Bozukluk olmadan, bozukluğu olan arkadaşlarımızla bağlantı kuramaz hale gelmeyecek miyiz?

`bb({ eyes:"sad", body:"chest" })`

b: Hayatımızdan memnun olursak, kendimizi daha iyi şeyler yapmaktan alıkoymaz mıyız?

`hong({ MOUTH_LOCK:true })`

h: ...

h: "Korkacak bi'şey kalmamasından" bile korkuyorsak...

h: Korkacak şeylerimiz kolay kolay bitmeyecektir.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Ah, Evet! Vay! Ne büyük bir rahatlama!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Doktor, sadece *bu seni nasıl hissettirdi* sorusuna 870₺/saat ödemek beni kaygılandırıyor."

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Hm-mmm. Peki bu seni nasıl hissettiriyor?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Evet, bu tamamen makul bir endişe.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: Ve akıl sağlığının çoğu kişi için karşılanabilir olmaması gerçekten berbat.

`hong({ eyes:"normal", mouth:"normal" });`

h: Yine de bazı ucuz veya ücretsiz seçenekler var:

`hong({ body:"chin" })`

h: Destek grupları, çevrimiçi terapi, kar amacı gütmeyen sağlık merkezleri...

`hong({ body:"hands_1" })`

h: Meditasyon, iyi uyku, arkadaşlarla düzenli sohbet gibi alışkanlıklar edinmek...

`hong({ body:"hands_2" })`

h: Kütüphaneden, kanıta dayalı psikoterapiler için çalışma kitapları ödünç almak...

`hong({ body:"one_up" })`

h: Bu oyunun sonunda kaynakların tam listesi var!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: *Dördüncü* duvar pek dayanmadı demek.

`hong({ body:"point" });`

h: Bazı şeyler edebi anlatıdan daha önemlidir. Akıl sağlığı gibi.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Terapistler de böyle demiyor mu? Tüm duygularını, olumsuz olanları bile kabul et?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Bekle.

["Kabul etmek" yani *pes etmek* mi?](#act4_bad_accept_give_up)

["Kabul etmek" yani *onaylamak* mı?](#act4_bad_accept_approve)

["Kabul etmek" yani *harfiyen* mi?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Sence Martin Luther King, "Otobüsün önünde oturamamız kötü, hadi *kabul edelim*" der miydi?

`bb({ eyes:"angry_r", body:"two_up" });`

b: Kişisel gelişim duayenleri beyaz bayrak sallamayı neden *derin bir bilgelik* olarak görüyor?

`bb({ eyes:"annoyed", body:"normal" });`

h: Bence "kabul et" ile kastettikleri şey: varlıklarını ve değiştirmesi zor olduklarını kabul et,

h: Ama değişime dair eylemlerde daha başlarken pes etme

`bb({ eyes:"suspect" });`

b: O zaman terapistler *tanı* demeli *kabul et* değil.

`hong({ body:"chin", eyes:"annoyed" });`

h: Evet, düşününce "kabul et" biraz kafa karıştırıcı.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Peki, bunu *tanıyorum.*

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Bozuk olmamız *iyi* bi'şeymiş gibi mi? Hayır!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Akıl hastalıklarını romantikleştiren tüm Hollywood senaristleri beş para etmez!

`bb({ eyes:"angry", body:"two_up" });`

b: Akıl hastası olmak *berbat!* İnsanların *hayatlarını* çalıyor! Bunu neden "kabul edelim"?!

`bb({ body:"normal" });`

h: Bence "kabul et" ile kastettikleri şey: onlara karşı sabırlı ol.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Tıpkı bataklıkta debelenmenin daha hızlı batırdığı ve çözümün sabırla dümdüz uzanmak olduğu gibi,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Seninle savaşmak, korkum, çatıdan atlamama neden oldu.
{{/if}}

{{if !_.INJURED}}
h: Seninle savaşmak, korkum, neredeyse çatıdan atlamama sebep olacaktı.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Bunun yerine, çözüm şu anda yaptığımız şeyi yapmaktır – savaşmak değil, sabırla birlikte olmaktır.

`bb({ eyes:"annoyed" });`

b: O zaman "kabul et" gibi sorunlu bir kelime yerine *bunu* demeliler.

`hong({ body:"chin", eyes:"annoyed" });`

h: Evet, biraz düşününce, "kabul etmek" berbat bir şey.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: "Kabul etmeyi" kabul etmiyorum.

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Ama zaten beni harfiyen dinlememen gerektiği *biliyoruz*.

`bb({ eyes:"sad_u", body:"two_up" });`

b: Bütün *sorun* sana yardım etmek istemem ama bunu yapmak için doğru sözcükleri bulamamam!

`bb({ eyes:"sad", body:"normal" });`

h: Bence "kabul et" ile kastettikleri şey: "ne savaşın ne de gözardı edin."

`hong({ eyes:"surprise", body:"one_up" });`

h: Duygularını dinle, onlarla birlik ol ama dediklerini %100 harfiyen anlama.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: O zaman terapistler "kabul et" gibi belirsiz bir sözcük yerine *bunu* söylemeliler.

`hong({ body:"chin", eyes:"annoyed" });`

h: Sanırım onlar da doğru sözcükleri bulamıyorlar.

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
[İncineceğimizden korkuyorum.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Yalnız kalacağımızdan korkuyorum.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Kötü biri olduğumuzdan korkuyorum.](#act4_bad)
{{/if}}

[Hayır, şimdilik iyiyim.](#act4c_prelude)

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

b: Duygularınla sağlıklı bir ilişki kurmak, ekrandaki düğmelere tıklamak kadar kolay değildir.

`bb({eyes:"sad", body:"normal"})`

b: Gerçekten *anlaşabilir* miyiz?

b: Ekip olarak birlikte *çalışabilir* miyiz?

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

a: Ö-öğ-öğle yemeğinde seninle oturmamın bir sakıncası var mı?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *Bu* hoşlandığın kişi mi? Neden psikopat bir seri katil gibi yalnız oturuyorlar?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Hoşlandığına oturabilir miyim diye sormak mı, kulağa ne kadar *muhtaç* geliyor?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *Bu* hoşlandığın kişi mi? Huzurları bozduk! Öyle bir yüküz ki!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: Ben-yani-, bu sorun değilse, ben sadece...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Bekle, seni partide görmedim mi?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Evet tabii ki! Buraya gel.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Üzgünüm, yalnız kalmaya ihtiyacım var.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Evet, kanepedeydin! İlk partiye gittiğimde oradaydın...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Panik atak geçirip ev sahibine yumruk attığımda.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Panik atak geçirip ağlayarak dışarı çıktığımda.
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

h2: Ah, seni olayın ortasına koymak istemiyorum!

`publish("act4", ["hong_to_alshire",4]);`

h2: Sadece tanıdık bir yüzü hatırladım, hepsi bu.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH BİLİYORDUM! TEHLİKELİ PANİK-ATAK PSİKOPATLAR!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH İLK İZLENİM OLARAK "TRAVMAMA TANIK OLDUN" DEDİ! BU, BİZDEN NEFRET ETTİLER DEMEKTİR!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH TRAVMATİK BİR OLAYI HATIRLATTIK. VARLIĞIMIZ BAŞKALARINA ZARAR VERİYOR.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Biraz bekle insan, rahat değiller gibi.

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
s: *ÇOK* DOSTANE DAVRANIYORLAR! TIPKI SERİ KATİL TED BUNDY GİBİ!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: DOSTANE ROLÜ YAPIYORLAR! KİMSE *GERÇEKTEN* BİZE YAKIN OLMAK İSTEMİYOR!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH HER ZAMAN BAŞKALARINI HUZURSUZ EDİYORUZ! DÜNYA ÜZERİNDEKİ BİR LEKEYİZ!
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

h2: Sadece duygularımı anlamak için biraz zamana ihtiyacım var. Lütfen bunu kişisel algılamayın.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: SAPKIN DÜŞÜNCELER DÜŞÜNÜYOR?! BU PSİKOPATIN KALBİNİ HANGİ KARANLIK İSTEKLER DOLUYOR?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: KİŞİSEL OLARAK REDDEDİLDİK! ASLA SEVİLMEYECEĞİZ!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: DUYGULARINI ANLAMASINI BÖLDÜK! ŞİMDİ SONSUZA KADAR TRAVMATİK OLACAKLAR VE HEPSİ BİZİM SUÇUMUZ!
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

b: Duygularınızla "barışın" diyorlar, sanki duygularımız *savaş suçlusuymuş* gibi.

`publish("act4", ["bb_closer", 7]);`

b: *Barıştan* daha fazlasını istiyorum! *Müttefik* olmamızı istiyorum!

`publish("act4", ["bb_closer", 3]);`

b: Açlık ve susuzluğun fiziksel alarmlar olması gibi iyi bir muhafız-köpek olmak istiyorum

`publish("act4", ["bb_closer", 8]);`

b: *Psikolojik* ihtiyaç alarmın olmak istiyorum – güvende, iyi olmak, ait hissetmek gibi.

`publish("act4", ["bb_closer", 1]);`

b: Ama... İşimde berbatım, bu yüzden beni eğitmene ihtiyacım var.

`publish("act4", ["bb_closer", 4]);`

b: Her zaman "mantıklı" veya "mantıksız" değilim. Sadece... elimden geleni yapıyorum. Yani,

`publish("act4", ["bb_closer", 30]);`

b: Lütfen sana yardım etmeme yardım et!

`publish("act4", ["bb_closer", 6]);`

b: Yaşlı bir köpeğe yeni numaralar öğretmek biraz *zaman* alacaktır. Belki *yıllar.*

`publish("act4", ["bb_closer", 3]);`

b: Ve bazen eski alışkanlıklarımı bırakamayacağım.

`publish("act4", ["bb_closer", 2]);`

b: Gölgelere havlayacağım. Seni sözlerimle korkutacağım. Hatta bazı rahatsız edici görüntüler... gösterebilirim.

`publish("act4", ["bb_closer", 9]);`

b: Üzgünüm! Ben hırpalanmış bir barınak köpeğiyim! Bazen yatağına kaka yapabilirim!

`publish("act4", ["bb_closer", 4]);`

b: Ama eğer bana karşı sabırlı olursan... yanımda kalıp ve benimle oturursan...

`publish("act4", ["bb_closer", 8]);`

b: Belki de bu kurdu evcilleştirebilirsin.

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
