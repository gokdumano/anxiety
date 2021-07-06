# act1

```
SceneSetup.act1();
```

(...300)

n: VE BU DA İNSANIN ANKSİYETESİ

n: _SEN_ ANKSİYETESİN

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Ah selam! Yine mi buraya döndük?

`hong({eyes:"0_neutral"})`

n: GÖREVİN İNSANINI *TEHLİKEDEN* KORUMAK

`bb({eyes:"look", mouth:"small_lock"})`

n: HATTA, ŞU ANDA BU OYUNU TEKRAR OYNAMAK ONU *TEHLİKEYE* ATIYOR,

n: ÇABUK, UYAR ONU!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: İnsan! Dinle, tehlikedeyiz! Oyuncu...

[...bize yine işkence edecek!](#act1_replay_torture)

[...alternatif bir son bulamayacak!](#act1_replay_alternate)

[...hikayenin akışına uymayacak!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Bizi bir top gibi kıvırıp ağlatacaklar!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Bize telefonunu kırdırıp seni panik atak geçirtecekler!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Bize parti sahibini yumruklat*MA*yacaklar!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Bize sempatik anti-kötü parti sahibini yumruklatacak!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: En azından bu sefer çatıdan atlamayaca--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: BİZİ ÇATIDAN ATLATACAKLAR.
{{/if}}

`bb({body:"fear"});`

b: TÜM BU YENİ KÖTÜ ŞEYLER BAŞIMIZA GELECEK VE SONRASINDA DA BİZ--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Tabii ki, bir *bütün* olarak hikaye aynı, fakat her bölümün iki olası sonu var, ayrıca dallanıp budaklanan diyalog-- 

`bb({body:"fear"});`

b: Oyuncu hayal kırıklığına uğrayacak, sekmeyi kapatıp yazılımımızı silecek ve sonra biz de--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Akışına mı?

`bb({eyes:"normal"});`

b: Hikaye, korkularınla sağlıklı bir ilişki kurabilmek için nasıl *SEÇİM* yapabildiğin hakkındaydı,

`bb({eyes:"normal_right"});`

b: Ama oyunu tekrar oynamak aynı sonu verecek, *SEÇİM*lerinin değersiz olduğu anlamına gelecek,

`bb({eyes:"narrow_eyebrow"});`

b: Dolayısıyla oyunun hikayesi ve mekanikleri arasında bir çelişki oluşacak,

`bb({eyes:"fear"});`

b: Böylece bu hikaye evreni saran örtü yırtılacak,

`bb({body:"fear"});`

b: Ve biz de--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: ÖLECEĞİZZZZZZZZZZZZZZ

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Neyse hadi karaktere geri dönelim.

```
Game.clearText();
```

n4: _ANKSİYETENİN_ FALAN FİLAN _KORKUNA_ EN BENZERİ FALAN FİLAN NASIL GİDİYOR BİLİYORSUN

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Oh harika, kurdum geri döndü. Şahaanee.

`hong({eyes:"0_neutral"})`

n: GÖREVİN İNSANINI *TEHLİKEDEN* KORUMAK

`bb({eyes:"look", mouth:"small_lock"})`

n: HATTA, ŞU ANDA BU SANDVİÇ ONU *TEHLİKEYE* ATIYOR

n: ÇABUK, UYAR ONU!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: İnsan! Dinle, tehlikedeyiz! Tehlike de...

`bb({body:"squeeze"})`

n4: _ANKSİYETENİN_ OYNAMASINA İZİN VER! _KORKUNA_ EN BENZERİNİ SEÇ

(#act1_normal_choice)

# act1_normal_choice

[Öğle yemeğini yalnız yiyoruz! Tekrar!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Yemek yerken üretken değiliz!](#act1a_productive) `bb({body:"squeeze_talk"})`

[O beyaz ekmek bizim için kötü!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Yalnızlığın, günde 15 sigara içmekle aynı derecede erken ölümle ilişkilendirildiğini bilmiyor musun?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Hm, kaynaklarını atıfladığın için sağol ama--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Demek oluyor ki eğer *şimdi* birileriyle takılmazsak-

`bb({body:"panic"})`

b: ÖLECEĞİZZZZZZZZZZZZZZ

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: *SEVİLMEME KORKUSU* KULLANDIN

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Dizüstü bilgisayarını çıkart ve hemen şimdi çalış!

`hong({eyes:"0_annoyed"})`

h: Hm, klavyemde kırıntı olmamasını tercih--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Eğer toplum-bedenine katkıda bulunmuyorsak, o zaman toplum-parazitiyiz!

b: Toplum-bedeni, toplum-parazitlerini öldürmek için ilaç için toplum-doktora gidecek, sonra biz--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ÖLECEĞİZZZZZZZZZZZZZZ

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: *KÖTÜLENME KORKUSU* KULLANDIN

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Bu çalışmalar doğrula--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: İşlenmiş buğday kan şekerimizi yükseltecek, sonra tüm uzuvlarımızı kesmek zorunda kalacaklar ve biz-

`bb({body:"panic"})`

b: ÖLECEĞİZZZZZZZZZZZZZZ

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: *İNCİNME KORKUSU* KULLANDIN

(#act1b)

# act1b

n: SÜPER ETKİLİ

`bb({mouth:"smile", eyes:"smile"});`

b: Gördün mü, insan? Ben senin sadık muhafız-kurdunum!

`bb({body:"pride_talk"});`

b: İçgüdülerine güven! Hislerin her zaman haklıdır!

`bb({body:"pride"});`

n: İNSANININ ENERJİ BARINI SIFIRLA

n: FİZİKSEL + SOSYAL + AHLAKİ İHTİYAÇLARINI KORUMAK İÇİN YAPABİLECEKLERİN:

n: *İNCİNME* KORKUSU #harm#

n: *SEVİLMEME* KORKUSU #alone#

n: *KÖTÜLENME* KORKUSU #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (İPUCU: EN DERİN, EN KARANLIK KİŞİSEL KORKULARINI VURAN SEÇENEKLERİ SEÇ! ~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: Belki de telefonumu kontrol etme zamanım gelmiştir.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: İNSANINI KORU

n: DÜNYADAN. DİĞER İNSANLARDAN. KENDİSİNDEN.

n: İYİ ŞANSLAR

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: BİRİNCİ TUR: *SAVAŞ!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Ha. Facebook'da bu hafta sonu bir parti olduğu söylüyor.

`bb({eyes:"uncertain"});`

b: Bu tuhaf tip *her* hafta sonu parti vermiyor mu?

`bb({eyes:"uncertain_right"});`

b: İçindeki hangi boşluğu doldurmaya çalışıyor? Kafası bayağı karışık olmalı!

`hong({eyes:"surprise"});`

h: Ben de mi davetliyim?

`bb({eyes:"fear", mouth:"normal"});`

b: İyi o zaman!

[Evet de, yoksa yalnızlıktan öleceğiz!](#act1c_loner)

[Hayır de, orası zehirli ilaçlarla dolu!](#act1c_drugs)

[Boş ver, partinin havasını bozarız.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Günde onbeş sigara, insan! ONBEŞ!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: O zaman cenazemize kimse gelmez, küllerimizi okyanusa atarlar, bir balina tarafından yeniliriz,
{{/if}}

{{if !_.fifteencigs}}
b: ve BALINA DIŞKISI oluruz!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: Yani evet o partiye gitmeliyiz!
{{/if}}

{{if _.parasite}}
b: Sadece dizüstü bilgisayarı getir, böylece çalışabiliriz ve toplum-paraziti olmayız.
{{/if}}

{{if _.whitebread}}
b: BEYAZ EKMEK servis etmedikleri sürece.
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: TANRIM. Seni susturacaksa, tamam.

h: Evet diyeceğim.

{{if _.whalepoop}}
b: Balina dışkısı, insan! Balina dışkısı!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: Hatta daha kötüsü... BEYAZ EKMEK
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: O kadar çok meth ve beyaz ekmek alacağız ki, şişman cesedimizi yakma fırınına sığdıramayacaklar!
{{/if}}

{{if !_.whitebread}}
b: O kadar çok uyuşturucu alacağız ki cenazeci vücudumuzun nasıl *zaten* önceden mumyalandığını merak edecek!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Ayrıca partiye gidemeyiz, çalışmamız lazım yoksa korkunç bir toplum-parazitiyiz!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: TANRIM. Seni susturacaksa, tamam.

h: Hayır diyeceğim.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tek yaptığımız, bir köşede yalnızlığın günde 15 sigara kadar öldürücü olduğu konusunda ağlamak.
{{/if}}

{{if _.parasite}}
b: Partilerde yaptığımız tek şey orada bulunmaktansa nasıl üretken olmamız gerektiği konusunda endişelenmek.
{{/if}}

{{if _.whitebread}}
b: Tek yaptığımız sağlıksız yiyecekleri bizi nasıl öldüreceği konusunda endişelenmek.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: ııh acaba neden

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Yani gidersek onları kötü hissettiririz ama davetlerini reddedersek de onları kötü hissettiririz!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: TEK YAPTIĞIMIZ İNSANLARI KÖTÜ HİSSETTİRMEK, BU YÜZDEN KÖTÜ HİSSETMELİYİZ

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ah. Seni susturacaksa, tamam.

h: Daveti görmezden geleceğim.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Neyse. Çok fazla Facebook. Daha sakin, daha az kaygı yaratan bir şeye ihtiyacım var.

`hong({eyes:"neutral"});`

h: Twitter'da yeni neler var?

`bb({eyes:"look"});`

[Olamaz, şu korkunç habere bak!](#act1d_news)

[Olamaz, bu tweet *bize* bir gönderme mi?](#act1d_subtweet)

[Aaa, süt içen kedi GIF'i](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Tanrım, sanki dünya yanıyor gibi değil mi?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Her şey bitiyormuş gibi geliyor, sanki her şey ölüyor ve lanetlendik ve bu konuda yapabileceğimiz hiçbir şey yok.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Hadi o hikayeyi retweet edelim!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Tamam, retweetleyeceğim, lütfen sessiz ol!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Boş ver, Snapchat'e bakalım.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: Bu şifreli bir tweet! Şifreli, şifreli bir tweet!

`hong({eyes:"annoyed"});`

h: Muhtemelen değil mi?

`bb({eyes:"narrow", mouth:"small"});`

b: ama ya hepsi arkamızdan konuşuyorsa

h: Yapmıyo--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: ARKAMIZDAN

`hong({eyes:"sad", mouth:"sad"});`

h: Sanmıyo-

`bb({eyes:"narrow", mouth:"small"});`

b: ama *ya öyleyse*

h: S--

`bb({eyes:"narrow_eyebrow"});`

b: *ya öyleyse*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: ta-mam, Snapchat'i deneyeceğim.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Heh ya bu çok tatlı, retweetle--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: KEDİLER SÜTÜ SİNDİREMEZ VE HAYVAN İSTİSMARINDAN HOŞLANDIĞIMIZ İÇİN KORKUNCUZ

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: ta-mam, Snapchat'i deneyeceğim.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Hah dün geceden fotoğraflar. Demek *bu* haftalık partiler böyle.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Oof, bu kadar kalabalık anksiyetemi tetikliyor.

h: Belki de daveti kabul etmemeliydim?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Cevabımızı mı değiştirelim? Bir pislik gibi?!](#act1e_yes_dontchange)

[Cevabımızı değiştirelim! Çok kalabalık!](#act1e_yes_changetono)

{{if _.subtweet}}
[Evet, tweetde bize gönderme yapıyorlar.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Doğruluğunu kontrol etmeden retweetledik.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Biliyor musun, çok kötü bir duruşun var?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Geleceğimize inanıyorlardı ve şimdi onların güvenine ihanet mi ediyoruz? Yalnız mı ölmek istiyorsun?!

{{if _.fifteencigs}}
b: ONBEŞ. SİGARA
{{/if}}

{{if _.whalepoop}}
b: BALİNA. DIŞKISI.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Kapa çeneni kapa çeneni, gideceğim!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: İzdiham nedir bilmiyor musun??

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: 2003 yılında bir Rhode Island gece kulübünde yangın çıktı ve panikleyen insanlar çıkışları tıkadı, 100 kişi yanarak öldü.

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: BUNUN BAŞIMIZA GELMESİNİ Mİ İSTİYORSUN-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: HAYIR DE HAYIR DE HAYIR DE HAYIR DE HAYIR DE HAYIR DE HA-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Kapa çeneni, kapa çeneni, tamam gitmeyeceğim! Tanrı!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... gerçekten eğlenceli görünüyor.

h: Belki de davete hayır dememeliydim?

`bb({mouth:"normal", eyes:"normal"});`

[Cevabımızı mı değiştirelim? Bir pislik gibi?!](#act1e_no_dontchange)

[Cevabımızı değiştirelim! Yalnız ölme!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Evet, tweetde bize gönderme yapıyorlar.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Doğruluğunu kontrol etmeden retweetledik.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Biliyor musun, çok kötü bir duruşun var?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Herkesin bizden beklentisi

b: ...onları rahat bırakmamız ve partide eğlenmelerine izin vermemiz, senin gibi korkunç bir {{if _.whitebread}}white-bread-munching{{/if}} pislik olma--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Kapa çeneni kapa çeneni, gitmeyeceğim işte!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Kronik yalnızlık, kortizol seviyemizi, kardiyovasküler hastalık ve felç riskimizi artırır!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: ONBEŞ. SİGARA.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Kapa çeneni, kapa çeneni, tamam gideceğim! Tanrı!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Tüm sorunlu tweetlerimiz gün yüzüne çıktı!!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: İfşa edileceğiz, dışlanacağız ve bir at sırtına iple bağlanıp bilgi otoyolundan aşağı sürükleneceğiz!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Neden böylesin?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Dezenformasyon yapıyoruz! Özgür basına olan güveni yok ediyoruz!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Demokrasinin enkazından doğacak faşizmin nedeni biziz!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Neden böylesin?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Sırtında bir kambur mu istiyorsun?! Ekranın doğru eğilmeyi bırak! 

```
bb({body:"meta"});
```

b: Sana da söylüyorum.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Neden böylesin?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... gerçekten eğlenceli görünüyor.

h: Belki de daveti görmezden gelmemeliydim?

`bb({mouth:"normal", eyes:"normal"});`

[Görmezden gelmeye devam et, partiyi berbat edeceğiz.](#act1e_ignore_continue)

[Aslında, evet de.](#act1e_ignore_changetoyes)

[Aslında, hayır de.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: Onları görmezden gelmek biraz kabalık, değil mi?

`bb({eyes:"normal_right"});`

b: Diğer insanlar *bizi* hep görmezden geldi

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: o yüzden ödeştik diyelim.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Eğlenmeme izin mi veriyorsun?

b: Yani, yalnızlık bizi *öldürebilir*.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: Çok kalabalık. Kalabalıklar tehlikelidir.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Her neyse. Yeni Tinder bildirimi.

`bb({eyes:"uncertain"})`

b: Ne, o ilişki uygulaması mı?

`hong({eyes:"annoyed"})`

h: Bu bir ilişki uygulaması değil, yeni insanlarla tanışma--

`bb({eyes:"narrow"})`

b: İlişki uygulaması

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Ah, biri ile eşleştim! Sevimli görünüyor!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Lütfen bunu mahvetm--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: TEHLİKE TEHLİKE TEHLİKE TEHLİKE TEHLİKE

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Başkaları tarafından *kullanılıyoruz*.](#act1f_used_by_others)

[Diğer insanları *kullanıyoruz*.](#act1f_using_others)

[SERİ KATİLLE EŞLEŞTİK](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Rastgele ilişkiler aşağıdaki deliği doldurabilir,

b: ama dolduramadığı delik...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *buradadır*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Mesele şu ki, YALNIZ ÖLECEĞİZ

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Başkalarının cinsel organları senin için yakalanacak Pokémonlar mı?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (pokemon tema müziği)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ İstiyorum ki en ^sürtük^ olayım

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Hiç kimsenin olmadığı kadar-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Bacaklar ve ^kıç^, kıvrımlı göğüsler-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ terli ^penis^ ve toplarıyla!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ ŞEHVET-MON! HEPSİNİ YA--

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Yani diyorum ki manipülatif bir sürüngeniz

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: Seni bir kuyuya kapatacaklar ve şişmanlatmak için beyaz ekmeği zorla besleyecekler ki derini yüzüp giyebilsinler!
{{/if}}

{{if _.parasite}}
b: Seni pomodoro tekniği ile dövecekler ve "DAHA ÜRETKEN OLMALIYDIN SENİ PARAZİT" diyecekler
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Etini kanlı bir konfeti haline getirecekler, bağırsaklarını flamalara çevirecekler ve kanını kokteyl kasesine karıştıracaklar!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Bir parti daveti için BU nasıl?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: bu oyundan çok sıkıldım.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"yalnızlık bizi öldürecek"... {{/if}}
{{if _.parasite}}"biz bir toplum-parazitiyiz"... {{/if}}
{{if _.whitebread}}"onu yeme, bizi öldürür"... {{/if}}
{{if _.subtweet}}"arkamızdan konuşuyorlar"... {{/if}}
{{if _.badnews}}"dünya yanıyor"... {{/if}}
{{if _.hookuphole}}"yalnız öleceğiz"... {{/if}}
{{if _.serialkiller}}"o bir seri katil"... {{/if}}
{{if _.catmilk}}"kediler sütü sindiremez"... {{/if}}
{{if _.pokemon}}^bombok^ bir parodi şarkısı... {{/if}}

h: sadece hayatımı yaşamak istiyorum.

h: Ben sadece tüm bu... acıdan kurtulmak istiyorum.

`bb({eyes:"look_sad"});`

b: Şey... insan...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Her şey güzel olacak.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Sadık bekçi-kurdun olarak, tehlikelere karşı dikkatli olacağım ve seni güvende tutmak için elimden geleni yapacağım.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Söz veriyorum.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Son uygulama. Instagram. Elinde ne var?

`hong({eyes:"sad"});`

h: Bunlar... daha fazla parti fotoğrafı.

`hong({mouth:"sad"});`

h: Herkes çok mutlu görünüyor. Endişeden uzak. Anksiyeteden uzak.

`hong({mouth:"anger"});`

h: Tanrım, neden onlar gibi olamıyorum? Neden *normal* olamıyorum?

`bb({eyes:"normal_right"});`

b: Partilerden SÖZ AÇILMIŞKEN, bu hafta sonu daveti için SON kararım:

`bb({eyes:"normal"});`

[Gitmeliyiz.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Gitmemeliyiz.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Ne y-

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^SİKTİR^.*

`hong({body:"2_you"});`

h: GİT.

(...500)

b: n

(...1500)

`bb({eyes:"wat_2"});`

b: ne?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: O partiye GİDECEĞİM,

{{if _.act1g=="go"}}
h: sen istediğin için DEĞİL, *ben* istediğim için.
{{/if}}

{{if _.act1g=="dont"}}
h: Sırf sen gitmemi istemiyorsun diye.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Kararlarımın kontrolü sende DEĞİL.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Şimdi izin verirsen bu lezzetli sandviçi huzur içinde yiyeceğim.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[AHHHH ÖLECEĞİZ](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH BİZDEN NEFRET EDİYORLAR](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH BİZ KORKUNÇ BİR İNSANIZ](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH ÖLECEĞİZ AAAAAAHHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH BİZDEN NEFRET EDİYORLAR AAAAAAHHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH BİZ KORKUNÇ BİR İNSANIZ AAAAAAHHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: TEBRİKLER

(...500)

n: İNSANININ FİZİKSEL + SOSYAL + AHLAKİ İHTİYAÇLARINI BAŞARIYLA KORUDUN

n: BAK, NE KADAR DA MİNNETTAR!

(...500)

n: ENERJİSİ SIFIR OLDUĞUNA GÖRE, EYLEMLERİNİ DOĞRUDAN KONTROL EDEBİLİRSİN

`bb({mouth:"smile", eyes:"normal"});`

n: BİTİRİCİ HAREKETİNİ SEÇ

`bb({mouth:"small_lock", eyes:"fear"});`

n: *BİTİR ONU*

[{SAVAŞ: Stres dolu telefonunu cezalandır!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{KAÇ: Bir topun içine kıvrıl ve ağla!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Telefonun sana panik atak geçirtiyordu!!

`bb({eyes:"anger"})`

b: Zuckerberg ve şirketi kapitalistleri zenginleştirmek için zihinsel sağlığına saldırıyor!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Telefonunu cezalandır! Yoket! Öldür!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLDÜR ÖLD--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Bütün dünya tehlikelerle dolu!!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Armadillo gibi yap! Kendini korumak için top şeklinde kıvrıl!!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: KIVRIL KIVRIL KIVRIL KIVRIL KIVRIL KIVRIL KIVRIL KIVRIL KIVRIL KIVRIL KIVRIL KIVRIL KIVRIL KIV--

(#act1j)

# act1j

`SceneSetup.act1_outro()`