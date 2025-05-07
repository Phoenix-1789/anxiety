# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PLAY!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Okay prima di iniziare come vorresti leggere?

`publish("show_options_bottom")`

# intro-start-2

n3: Ora, iniziamo la nostra storia...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: QUESTO È UN UMANO

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

n: E QUESTA È L'ANSIA DELL'UMANO

n: _TU_ SEI L'ANSIA

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: No, no, no, non ti sto ascoltando. Guarderò il mio telefono

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: LA TUA MISSIONE È PROTEGGERE L'UMANO DAL *PERICOLO*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Gasp! Stai scrollando via la tua vita su Twitter! Di nuovo!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Sì mi chiedo proprio perchò non sto seduta e basta ad ascoltare i miei pensieri più spesso.

`hong({eyes:"neutral"});`

n: VELOCE, AVVISALA DEL *PERICOLO*

```
bb({eyes:"look"});
```

[Oh no, guarda a quell'orrenda notizia di cronaca!](#act1d_news)

[Oh no, quel tweet potrebbe riferirsi a *noi?*](#act1d_subtweet)

[Hey, una GIF di un gatto che beve del latte](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Heh sì, è carin--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: I GATTI NON DIGERISCONO IL LATTE E SIAMO DELLE PERSONE ORRENDE PER TROVARE CARINO L'ABUSO SUGLI ANIMALI

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



