# **Quest Translator** (World of Warcraft addon) #
[![](http://images40.fotosik.pl/470/cd7cd6dd1facda41.gif)](http://code.google.com/p/quest-translator#Polski) [![](http://images49.fotosik.pl/486/892274e5b8e0f500.gif)](http://code.google.com/p/quest-translator#English) [![](http://images40.fotosik.pl/470/c0105441bed4fe07.gif)](http://code.google.com/p/quest-translator#Japanese) [![](http://images37.fotosik.pl/1199/31316bdd405196c3.jpg)](http://code.google.com/p/quest-translator#Italiano)

Link to sililar addon: [WowTranslator](http://code.google.com/p/wow-translator/)

NOTE: Comments and error reports please sent to: **platine . wow @ gmail . com** . . . . . . . . . Latest available version: [3.03](http://code.google.com/p/quest-translator/downloads/list) - [2513](http://code.google.com/p/quest-translator/downloads/list)

New version 4.01 for Vanilla Wow (classic 1.12.1) is available here:  http://lingvo.top.098.pl/wow/QuestTranslator_4.01_PL_2513.zip


&lt;BR&gt;



&lt;BR&gt;


# [![](http://images40.fotosik.pl/470/cd7cd6dd1facda41.gif)](http://code.google.com/p/quest-translator/) Polski #
Ten dodatek do World od Warcraft wyświetla przetłumaczony tekst questu bezpośrednio w oknie questu lub w oddzielnym oknie obok. Pracuje w oknie QuestLog, a także podczas rozmowy z NPC.


&lt;BR&gt;


QuestTranslator powstał w grudniu 2010r. i został zainspirowany dodatkiem **QuestJapanizer** (wersja: 0.5.8, autor: **lalha**), który wyświetla przetłumaczony na język japoński tekst questów zawartych w QuestLogu. QuestTranslator rozszerza jego funkcje, wyświetlając tekst questów w dowolnym (wcześniej przygotowanym) języku oraz wyświetla tłumaczenie tekstu questu od razu podczas rozmowy z NPC oferującym dany quest (czyli przy akceptacji pobrania questu, jego postępu lub oddawaniu gotowego questu). Tłumaczenia wyświetlane są bezpośrednio w oknie z oryginalnym tekstem (zastępując go) lub w oddzielnym okienku obok oryginalnego okna z questem, jak pokazano na poniższych zdjęciach:

![![](http://images38.fotosik.pl/1512/ecd53ae050702064m.jpg)](http://images38.fotosik.pl/1512/ecd53ae050702064.jpg) ![![](http://images37.fotosik.pl/1484/d7ccfcbb6c12abaem.jpg)](http://images37.fotosik.pl/1484/d7ccfcbb6c12abae.jpg) ![![](http://images50.fotosik.pl/1531/3915edeeeacd3881m.jpg)](http://images50.fotosik.pl/1531/3915edeeeacd3881.jpg) ![![](http://images40.fotosik.pl/1514/e08b01f7c5a9b6eam.jpg)](http://images40.fotosik.pl/1514/e08b01f7c5a9b6ea.jpg) ![![](http://images49.fotosik.pl/1476/8e32469be74fb7b8m.jpg)](http://images49.fotosik.pl/1476/8e32469be74fb7b8.jpg) ![![](http://images37.fotosik.pl/504/9184ba52491cc306m.jpg)](http://images37.fotosik.pl/504/9184ba52491cc306.jpg)

Okno z tłumaczeniem można wyłączyć klikając na przycisk przełącznika "QTR" umieszczony w prawym-górnym rogu okna QuestLog. Kolejne kliknięcie na ten przycisk przywraca wyświetlanie okna z tłumaczeniem. Okno to można też dowolnie przesuwać na ekranie w miejsce bardziej pasujące graczowi. Komendą /qtr można wejść do konfiguracji dodatku.

![![](http://images35.fotosik.pl/365/785a52fd71480f33m.jpg)](http://images35.fotosik.pl/365/785a52fd71480f33.jpg)

Najważniejszym plikiem tego dodatku jest baza tłumaczeń questów w danym języku, czyli plik **QuestData\_xx.lua** . Zawiera wszyskie podstawowe sekcje questu (Zadanie, Szczegółu, Postęp, Zakończenie, Tłumacz), a także dodatkowe informacje w języku tłumaczenia, jak np. nagłówki sekcji. Plik ten zapisany jest przeważnie w formacie UTF-8, dzięki temu możliwe jest korzystanie z obszernej biblioteki czcionek znaków narodowych (diakrytycznych) danego języka zawartych w pliku **ipagui.ttf** . Takie rozwiązanie pozwala na prawidłowe wyświetlanie znaków narodowych dowolnego języka w oknie z tłumaczonym tekstem questu.


&lt;BR&gt;



&lt;BR&gt;


### Instalacja ###
Instalacja dodatku polega na pobraniu archiwum dodatku z działu _Download_, rozpakowaniu go i skopiowaniu całego folderu dodatku do katalogu **Interface\AddOns\** . Jeśli grę zainstalowano w folderze np. **C:\Program Files\World of Warcraft** , to dodatek QuestTranslator należy przekopiować do folderu: **C:\Program Files\World of Warcraft\Interface\AddOns\** jak na poniższym zdjęciu.

![![](http://images45.fotosik.pl/531/59f097cb1662dcbfm.jpg)](http://images45.fotosik.pl/531/59f097cb1662dcbf.jpg)



&lt;BR&gt;


### Deinstalacja ###
Deinstalacja dodatku polega na usunięciu katalogu QuestTranslator z folderu **Interface\AddOns\** .


&lt;BR&gt;



&lt;BR&gt;


### Przystosowanie dodatku do swojej wersji gry ###
Dodatek QuestTranslator został napisany z  wykorzystaniem podstawowych funkcji gry World of Warcraft i może pracować w dowolnej jego wersji. W przypadku zmiany aktualnej wersji gry (np. wczytania nowego Uaktualnienia - Patcha) trzeba dostosować dodatek do tej zmiany. Najprostszym rozwiązaniem jest wyłączenie kontroli zgodności dodatków z wersją gry poprzez wybranie na ekranie startowym postaci przycisku AddOns i zanaczenie funkcji (Load **out of date** AddOns). Inną, bardziej polecaną metodą jest drobna modyfikacja wpisu w pliku QuestTranslator.toc dodatku określającego używaną wersję gry.

![![](http://images38.fotosik.pl/523/f28bd08a8881e7afm.jpg)](http://images38.fotosik.pl/523/f28bd08a8881e7af.jpg)
![![](http://images35.fotosik.pl/365/ce94d519691c1cdem.jpg)](http://images35.fotosik.pl/365/ce94d519691c1cde.jpg)

Wykonujemy edycję tego pliku i zmieniamy wpis wersji interfejsu na zgodną według wykazu poniżej.

| **wersja gry** | **wpis w pliku TOC** |
|:---------------|:---------------------|
| 5.3.0 - 5.3.x  | 50300                |
| 4.3.0 - 4.3.x  | 40300                |
| 4.2.1 - 4.2.2  | 40200                |
| 4.0.1 - 4.0.6  | 40000                |
| 3.3.0 - 3.3.5  | 30300                |
| 2.4.0 - 2.4.3  | 20400                |



&lt;BR&gt;

Spolszczenie questów do gry World of Warcraft. Wow questy po polsku.

&lt;BR&gt;


Osoby chętne do pomocy w tłumaczeniu proszone są o kontakt (mail podany na początku strony).


&lt;BR&gt;



&lt;BR&gt;



---



&lt;BR&gt;


# [![](http://images49.fotosik.pl/486/892274e5b8e0f500.gif)](http://code.google.com/p/quest-translator/) English #
This WoW-AddOn displays in a separate window the translated text for the quest. He works next to the window QuestLog, as well as during conversations with NPCs.


&lt;BR&gt;


QuestTranslator was created in December 2010 and was inspired by addon **QuestJapanizer** (Version: 0.5.8, author: **lalha**), which displays the translated text into Japanese in QuestLog quests. QuestTranslator extends its functionality by displaying text quests in any (previously prepared) language translation of the text and displays the quest right away when talking to the NPC offering the quest (the quest for acceptance of the download, its progress or passing the final quest). Translations are displayed direct into original quest frame (replacing it with a translation) or in a separate window next to the original window with the quest, as shown in the pictures below (the photo shows a pseudo-translation into English):

![![](http://images35.fotosik.pl/365/5fdc6b931556d260med.jpg)](http://images35.fotosik.pl/365/5fdc6b931556d260.jpg)
![![](http://images45.fotosik.pl/531/0ade11700bfa3589m.jpg)](http://images45.fotosik.pl/531/0ade11700bfa3589.jpg)

A window with a translation can be disabled by clicking the toggle button "QTR" in the right-upper corner of QuestLog frame. Next click on this button restores the window with the translation. This window can also freely move on the screen in a place more suitable to the player.

![![](http://images49.fotosik.pl/529/eda6df46f8cb4f87m.jpg)](http://images49.fotosik.pl/529/eda6df46f8cb4f87.jpg)

The most important file of this addon is a database of translations of quests in a given language - file **QuestData\_xx.lua**. However there Contains basic sections quest (task Details, Progress, Complete, Translator), as well as additional information in translation, such as section headings. This file is usually saved in UTF-8, so that it is possible to use the extensive library of fonts, national characters (diacritics) of the language contained in the file **ipagui.ttf**. This allows the correct display of national characters of any language in the window with the translated text quest.


&lt;BR&gt;



&lt;BR&gt;


### Installation ###
The installation consists of downloading the addon from the archive section _Download_, unpacked it and copied the entire folder of addon to the directory **Interface\AddOns\**. If the game is installed in a folder such as **C:\Program Files\World of Warcraft**, then addon QuestTranslator be copied into the folder: **C:\Program Files\World of Warcraft\Interface\AddOns\** as the picture below:

![![](http://images45.fotosik.pl/531/59f097cb1662dcbfm.jpg)](http://images45.fotosik.pl/531/59f097cb1662dcbf.jpg)



&lt;BR&gt;


### Uninstallation ###
Uninstalling the addon is removed from the folder directory QuestTranslator **Interface\AddOns\** .


&lt;BR&gt;



&lt;BR&gt;


### Adapting addon to its version of the game ###
The Addon QuestTranslator is written using the basic functions of the game World of Warcraft and can work in any version. If you change the current version of the game (for example, to load the new updates - patch) need to adjust the allowance for this change. The simplest solution is to disable monitoring of compliance with the additive version of the game by selecting the start screen, a button AddOns and selection function (Load **out of date** AddOns). Another recommended method is a more minor modification of an entry in the file QuestTranslator.toc appendix down the version of the game.

![![](http://images38.fotosik.pl/523/f28bd08a8881e7afm.jpg)](http://images38.fotosik.pl/523/f28bd08a8881e7af.jpg)
![![](http://images45.fotosik.pl/531/af6ea7173bd25b80m.jpg)](http://images45.fotosik.pl/531/af6ea7173bd25b80.jpg)

We edit this file and change the entry in the compatible versions of interface as listed below:

| **version of the game** | **TOC file entry** |
|:------------------------|:-------------------|
| 5.3.0 - 5.3.x           | 50300              |
| 4.3.0 - 4.3.x           | 40300              |
| 4.2.1 - 4.2.2           | 40200              |
| 4.0.1 - 4.0.6           | 40000              |
| 3.3.0 - 3.3.5           | 30300              |
| 2.4.0 - 2.4.3           | 20400              |



&lt;BR&gt;



&lt;BR&gt;



---



&lt;BR&gt;


# [![](http://images40.fotosik.pl/470/c0105441bed4fe07.gif)](http://code.google.com/p/quest-translator/) Japanese #

別のウィンドウでこのアドオンWorld of Warcraftのクエストが表示されますに翻訳されたテキスト。


&lt;BR&gt;


QuestTranslatorはQuestJapanizerを添加することによって触発された（バージョン：0.5.8、著者：lalha）がクエストをquestlogで日本語に翻訳されたテキストが表示されます。 QuestTranslatorは、提供にNPCにクエスト（ダウンロード、その進捗状況や最終的な探求を渡すの受け入れのための探求）話すとき、すぐに（事前に準備された）すべてのクエスト内のテキストを表示することにより、テキストと表示されますクエストの言語への翻訳を、その機能を拡張しています。翻訳は、独立したウィンドウとして下の写真に示すように探求して元のウィンドウの横に表示されています：

![![](http://images49.fotosik.pl/529/88b5881cf39eb0a0m.jpg)](http://images49.fotosik.pl/529/88b5881cf39eb0a0.jpg)
![![](http://images37.fotosik.pl/505/a5d09159f20fed40m.jpg)](http://images37.fotosik.pl/505/a5d09159f20fed40.jpg)

翻訳とウィンドウが右上隅のquestlogのトグルボタン"QTR"をクリックして無効にすることができます。このボタンを復元で[次へ]をクリック翻訳でウィンドウを表示します。このウィンドウには、自由な場所複数の選手に適した方法で画面上に移動することができます。

![![](http://images40.fotosik.pl/513/bd6cc057194abe83m.jpg)](http://images40.fotosik.pl/513/bd6cc057194abe83.jpg)

追加する最も重要なファイルは、特定の言語、またはファイルQuestData\_xx.luaのクエストの翻訳のデータベースです。しかし、基本的なセクションクエスト（タスクの詳細を、進歩、完全、翻訳者）だけでなく、セクションの見出しなどの翻訳の追加情報を、そこが含まれている。このファイルは、通常は、フォント、国別文字（ダイアクリティカルマーク）ファイルipagui.ttfに含まれている言語の大規模なライブラリを使用することが可能ですので、UTF-8で保存されます。これは、翻訳されたテキストクエストのウィンドウ内の任意の言語の国別文字が正しく表示されることができます。


&lt;BR&gt;



&lt;BR&gt;


### インストール ###
アドインでは、第\_Download\_のフェッチの関係のインストールは、unpackは、フォルダ\*Interface\AddOns\の添加剤をフォルダ全体をコピーしてください。
ゲームは\*C:\Program Files\World of Warcraft\*のようなフォルダにインストールされている場合は、このほかにQuestTranslatorは、下の写真のようにフォルダ\*C:\Program Files\World of Warcraft\Interface\AddOns\**のにコピーされます。**

![![](http://images45.fotosik.pl/531/59f097cb1662dcbfm.jpg)](http://images45.fotosik.pl/531/59f097cb1662dcbf.jpg)



&lt;BR&gt;


### のアンインストール ###
添加剤をアンインストールフォルダディレクトリQuestTranslator **Interface\AddOns\**のから削除されます


&lt;BR&gt;



&lt;BR&gt;


### ゲームのそのバージョンに加えての適応 ###
QuestTranslator追加は、基本的な関数worldofwarcraftゲームを使って書かれていますすべてのバージョンで作業することができます。あなたは（新しい更新プログラムをロードするために、例えば、-パッチ）は、ゲームの現在のバージョンを変更する場合は、この変更引当金を調整する必要があります。最も簡単な解決策は、開始画面で、ボタンやアドオンzanaczenie関数（Load **out of date** AddOns）はを選択することで、ゲームの添加剤のバージョンの遵守の監視を無効にすることです。もう一つの推奨される方法は、ゲームのバージョンダウンファイルQuestTranslator.toc付録内のエントリのマイナーな変更です。我々は、このファイルを編集して、下記のようにインターフェイスの互換性のあるバージョンのエントリを変更します。

![![](http://images38.fotosik.pl/523/f28bd08a8881e7afm.jpg)](http://images38.fotosik.pl/523/f28bd08a8881e7af.jpg)
![![](http://images47.fotosik.pl/531/31d512f811b227e6m.jpg)](http://images47.fotosik.pl/531/31d512f811b227e6.jpg)

| **ゲームのバージョン** | **ファイル内のエントリ TOC** |
|:--------------|:-------------------|
| 5.3.0 - 5.3.x | 50300              |
| 4.3.0 - 4.3.x | 40300              |
| 4.2.1 - 4.2.2 | 40200              |
| 4.0.1 - 4.0.6 | 40000              |
| 3.3.0 - 3.3.5 | 30300              |
| 2.4.0 - 2.4.3 | 20400              |



&lt;BR&gt;



&lt;BR&gt;



---



&lt;BR&gt;


# [![](http://images37.fotosik.pl/1199/31316bdd405196c3.jpg)](http://code.google.com/p/quest-translator/) Italiano #
Questo WoW-AddOn viene visualizzato in una finestra separata il testo tradotto per la ricerca. Lavora accanto al questlog finestra, così come durante le conversazioni con gli NPC. La prima versione è stata aggiunta nel dicembre 2010.

![![](http://images43.fotosik.pl/1244/d1bc069baf00081fmed.jpg)](http://images43.fotosik.pl/1244/d1bc069baf00081f.jpg)

Una finestra con una traduzione può essere disattivato cliccando sul pulsante di commutazione "QTR" in alto a destra della cornice questlog. Successivamente clicca su questo pulsante ripristina la finestra con la traduzione. Questa finestra può anche muoversi liberamente sullo schermo in un luogo più adatto per il giocatore.

![![](http://images49.fotosik.pl/529/eda6df46f8cb4f87m.jpg)](http://images49.fotosik.pl/529/eda6df46f8cb4f87.jpg)

< Ciò che serve è una persona che conosce la lingua italiana ha aggiunto alla stesura della descrizione in questa pagina. >


&lt;BR&gt;



&lt;BR&gt;



---



&lt;BR&gt;

