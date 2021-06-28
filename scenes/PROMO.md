# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[BAŞLA!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Başlamadan önce, hangisini daha rahat okuyorsun?

`publish("show_options_bottom")`

# intro-start-2

n3: Pekala, hikayemize başlayalım...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: BU BİR İNSAN

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: BU DA İNSANIN ANKSİYETESİ

n: _SEN_ ANKSİYETESİN

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Hayır. Yok, hayır, dinlemiyorum. Telefonuma bakacağım.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: GÖREVİN İNSANINI *TEHLİKELERDEN* KORUMAK

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Haaa! Hayatını Twitter'da harcıyorsun! Yine!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Evet neden oturup düşüncelerime daha çok kulak vermiyorum acaba.

`hong({eyes:"neutral"});`

n: ÇABUK, ONU *TEHLİKEYE* KARŞI UYAR!

```
bb({eyes:"look"});
```

[Olamaz, şu korkunç habere bak!](#act1d_news)

[Olamaz, bu tweet *bize* bir gönderme mi?](#act1d_subtweet)

[Aaa, süt içen kedi GIF'i](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Hah ne şirin, Ben--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: KEDİLER SÜTÜ SİNDİREMEZ VE HAYVAN İSTİSMARINA GÜLDÜĞÜMÜZ İÇİN KÖTÜ İNSANLARIZ

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



