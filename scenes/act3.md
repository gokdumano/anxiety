# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Sağlığına!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *Ah* bu ilaç gibi geldi.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: İşi biliyorsun, ufaklık...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Özellikle, sağ ve sol amigdalalarıma iyi geldi.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Bana gençliğimi hatırlatıyorsun. Kafamdaki hayvan tarafından acı çektiğim zamanları...

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: İyilik yaptığım için ve benim canavarı öldürdüğüm gibi seninkini de öldürmene yardım edebildiğim için minnettarım.
```
publish("act3",["roofhunter",2]);
```

r: Hey, küçük bir soru: Doğruluk mu cesa--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: CESARETLİK!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Haha! Harika.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Tamam. Aşağıdaki açık mavi yüzme havuzunu görüyor musun?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Evet? Altı kat aşağıdaki mi?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Atla oraya.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Bekle, ne?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: Hayvanın sızlanmaya başladı, değil mi?

```
publish("act3",["roofhunter",23]);
```

r: *Oh hayıııır bu tehlikeli, bunu yapmaaaa.*

```
publish("act3",["roofhunter",22]);
```

r: Ama tam da bu yüzden ölüme inat heyecanlara ihtiyacımız var.! Kop kop! Anı Yaşa! Bir fahişenin ^kıç^ından kokaini çek, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: O hayvana ^sürtük^lüğü hakkında ^sik^lemediğimizi göster! Atla oraya.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Uh, ama bazen, um... korku da bir sebep...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: Üzgünüm, kendini kötü hissetmenin *iyi* olduğunu savunan McMindfulness propagandasına mı kapıldın?

```
publish("act3",["roofhunter",17]);
```

r: Bu dünyayı yöneten ^pislikler^ geri kalanımıza anksiyete ve depresyon veriyor,

```
publish("act3",["roofhunter",18]);
```

r: O zaman TED Talks'ta bize delirmeyi kabul etmemizi ve kafamızın içindeki o sadist iblisi kucaklamamızı söyleyin!

```
publish("act3",["roofhunter",6]);
```

r: Ufaklık, O hayvanın bizim gibi insanlarını *incittiğini* *sen* de biliyorsun. O bizim gibilere *acı çektiriyor*.

```
publish("act3",["roofhunter",19]);
```

r: O bizim arkadaşımız değil. O kuduruk bir canavar, ya sakinleştirilmesi gerekiyor,

```
publish("act3",["roofhunter",20]);
```

r: Ya da *kafasına kurşun sıkılması*.

```
publish("act3",["roofhunter",27]);
```

r: Aksi takdirde, onun kazanmasına izin vereceksin.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: Hayır. Yanılıyorsun.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: Kazanmasına izin vermeyeceğim.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: ^Siktir^ harika! İnanıyorum sana, bebeğim! Öldür onu! <3

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: hayır hayır hayır hayır

n: BU BÖLÜMÜN İKİ AYRI SONU VAR. BİRİSİ *ÇOK, ÇOK KÖTÜ.*

b: HAYIR HAYIR HAYIR HAYIR HAYIR HAYIR HAYIR

n: AKILLICA SEÇ. İNSANINI KORU.

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAA

`bb({ mouth:"normal" });`

n: İYİ ŞANSLAR.

```
Game.clearText();
bb({ eyes:"start" });
```

[İnsan, atlarsan ÖLEBİLİRSİN!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Yaptığın aptalca ve zarar verici!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Bu sapıklar senin gerçek arkadaşların değil!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: İ--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Y--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: B--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Biliyor musun?, sana inanabilirdim... eğer zibilyon kere denemiş olmasaydın.

h: Sen kurt diye ağlayan kurtsun.

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Bunu sen de denedin.

b: İnsan, lütfen...

`hong({ eyes:"look_right" });`

h: Oh *üzgünüm* Big Pharma kendi kendime ilaç almamı onaylamıyor.

h: Bana bak ^pislik^, *hepimizin* kendi çenesini kapatmanın bir yolu var.

`hong({ body:"look_up", eyes:"look_up" });`

h: Bazı insanlar kendilerini çalışmaya bırakır.

`hong({ body:"look_down", eyes:"look_down" });`

h: Bazı insanlar kendilerini seks, uyuşturucu ve facebook sayfalarını yenilemeye bırakır.

`hong({ body:"normal", eyes:"look_right" });`

h: Bazı insanlar ise kendilerini diğer insanlara bırakır. 

`hong({ eyes:"angry" });`

h: Ben de kendimi bu yüzme havuzuna bırakacağım.

[Sarhoşsun ve yüzme havuzu ALTI KAT AŞAĞIDA!](#act3_bad_1_harm)

[Kahretsin, Bana böyle mi teşekkür ediyorsun?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Tamam, kabul ediyorum. Batırdım.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Suya düşsen bile, *en iyi ihtimalle* yüzey gerilimi kaburgalarını kıracak ve sana bir sarsıntı verecek!

h: Eh.

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Bir keresinde Rus bir çocuğun bunu Youtube'da yaptığını gördüm.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: Be- Affedersin, *teşekkür* mü?

`bb({ eyes:"angry" });`

b: İşte tam da bu yüzden *varım!*. İnsanlara kendilerini korumak konusunda güvenilmez!

b: Hayatım boyunca senin o aptal ^kıç^ını korumaya çalıştım ve şimdi sen at--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: heh.

`hong({ body:"laugh_2" })``

h: hahahaha

`hong({ body:"laugh_3" })``

h: HAHAHAHAHAHA

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: Oh WOW! Bu yüzyılın en küçümseyici hareketiydi!

`hong({ body:"yell_2" });`

h: Evet, seni ^bok^ yığını! Her şeyi mahvettin!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Başka söylenecek söz var mı, Efendi Besbelli?

[Ama benden intikam almak çözüm değil!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Ama bu sefer *kesinlikle*  haklıyım!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Seni incittim.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Duygularınla daha iyi bir ilişki kurmalısın, onları su ile boğm--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```q

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: Lütfen, şişeyi yerine koy ve gide--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: lütfen... yapma...

h: Enerji barın oldukça düşük görünüyor, kurt.

h: Eğer senin yerinde olsaydım, Seçtiğim kelimelere dikkat ederdim.

`bb({ eyes:"normal" });`

[İyi. Seni korumaktan yoruldum.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Her zaman ben haklıydım.](#act3_bad_2_right)

[Özür dilerim.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: O zaman, git ve atla. Bak bakalım umrumda mı?

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Tamam o zaman. Haydi şerefe.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: BEKLE HAYIR BU TERS PSİKOLOJİYDİ, SÖYLEDİKLERİMİN *TERSİNİ* YAPMAN GERE--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: *Kendini* tehlikeye atıyorsun. Arkadaş dediklerin *seni* kullanıyor ve *sen* de onları kullanıyorsun.
`bb({ eyes:"sad" });`

b: Lütfen, insan... Neden bana inanmıyorsun?!

h: Çünkü sen *bana* asla inanmadın.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Diğer muhafız-kurtların onları sabırla eğitmek, birlikte çalışmayı *öğrenmek* için zaman harcayan insanları var,

b: Muhafız kurtların insanları korumaya çalıştıkları için nefret etmesindense! Neden sen sade--

`bb({ eyes:"normal" });`

h: Yanlış cevap.

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *"Korkulacak tek şey korkunun kendisidir."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Endişelenme, mutlu ol!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Şimdiki bilge halk hemfikir: negatif duygular *kötüdür!*

`hong({ eyes:"less_angry" });`

h: Ah! Bu yüzden onlara *negatif* denir!

b: insan... lütfen...

`hong({ eyes:"normal" });`

h: Bir süre önce, dedim ki: “Sadece bütün acıdan kurtulmak istiyorum.”

h: İstediğimi aldım. Artık acı, korku veya anxiety hissetmiyorum...

h: Artık hiç bir şey hissetmiyorum.
`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Seni başka hiçbir şeyin incitemeyeceğinden emin olmaya çok kafaya takmıştım, acıyı *benim* yarattığımı fark edememiştim.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: HAYIR. ^SİKTİR^.

`hong({ body:"yell_1" });`

h: ^KAHRETSİN^. Gerçekten anlaman bu kadar uzun mu sürdü?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Bizi çok fazla beladan kurtarabilirdin, seni koca şişko aptal. Neden daha önce fark etmedin?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...sen... *üzgünsün*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Neden *özür diliyorsun?*

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[Üzgünüm iyi bir koruyucu değildim.](#act3_good_3_protector)

[Üzgünüm sana saygı duymadım.](#act3_good_3_respect)

[Özür dilerim.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Üzgünüm berbat bir insanım var!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Üzgünüm sana saygı duymadım.](#act3_good_3_respect)

[Üzgünüm seni incittim.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: Seni gerçek *tehlikelerden* korumak benim görevim, Oysa ben arabalara ve postacılara havlamaya devam ettim.

`bb({eyes:"sorry_up"});`

b: Gölgelerde havladım. Çok havladım.

`bb({eyes:"sorry"});`

b: Beni susturmak istemekte çok haklısın.

`bb({eyes:"sorry_down"});`

b: .

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: *Senin* sağdık koruyucu köpeğin olmam gerekirdi ama *bana* itaat etmen gerekiyormuş gibi davrandım.

`bb({eyes:"sorry_up"});`

b: Bir koruyucu ile hapis gardiyanı arasında fark vardır ve ben çizgiyi aştım.

`bb({eyes:"sorry_down"});`

b: Özür dilerim.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Seni incinmekten korumaya çalışmak konusunda çok takıntılıydım., *Seni* incittiğimi fark etmeyi asla bırakmadım.

`bb({eyes:"sorry_up"});`

b: Kötü bir köpektim.

`bb({eyes:"sorry_down"});`

b: Özür dilerim.

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: Evet, neyse bu aptal bir fikirdi.

h: Bunu sadece sen beni mahvettin diye yaptım, ve, ben de seni mahvettim.

h: Hadi bu turu berabere sayalım, tamam mı?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Tamam.

h: Tamam.

n: *BAĞ*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: Oh *hadi ama*. O hayvanın sana yaptıklarından sonra, *pes mi edeceksin?*

r: Sorun nedir, ufaklık? *Korktun mu?*

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Evet.

h2: Korktum.

`publish('hong-next')`

h2: Ve sorun değil!

`publish('hong-next')`

h2: Korkmak sorun değil.

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: Did they just lock the door?

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: hayır...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: hayır hayır

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: HAYIR!

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
