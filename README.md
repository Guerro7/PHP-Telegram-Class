# PHP-Telegram-Class

<h3>Available Functions</h3>

sendMessage - send messages <br>
sendPhoto - send pictures <br>
sendDocument - send files <br>
sendAudio - send audio files <br>
sendVideo - send video files <br>
sendChatAction - chat actions e.g. "typing..." (see description) <br>
kickChatMember - Benutzer aus eine Gruppe kicken <br>
unbanChatMember	- Benutzer entsperren <br>
sendKeyboard - display keyboard <br>
hideKeyboard - fade out keyboard <br>
setWebhook - set Bot webhook <br>
delWebhook - delete Bot webhook <br><br>

<h3>Simple Example</h3>
```ruby
<?php
require_once('class.moonliightz.telegram.php');

$bot = new Telegram(BOT KEY);

$bot->sendMessage(CHAT_ID, "Text");
$bot->sendPhoto(CHAT_ID, "storageplan.png", "Bildunterschrift");
$bot->sendDocument(CHAT_ID, "storageplan.png");
$bot->sendAudio(CHAT_ID, "BVB.mp3", "Interpret", "Titel");
$bot->sendVideo(CHAT_ID, "video.mp4", "Beschreibung");

$bot->sendChatAction(CHAT_ID, 1);

$bot->kickChatMember(CHAT_ID, USER_ID);
$bot->unbanChatMember(CHAT_ID, USER_ID);

$bot->sendKeyboard(CHAT_ID, "Text", array( array( "Zeile1 Test1", "Zeile1 Test2" ), array( "Zeile2 Test3", "Zeile2 Test4" ) ));
$bot->hideKeyboard(CHAT_ID, "Text");

$bot->setWebhook(URL);
$bot->delWebhook();
?>
```
<br>
<h3>Documentation</h3>

<a href="https://moonliightz.de/doc/php-telegram-class/class-Telegram.html">https://moonliightz.de/doc/php-telegram-class/class-Telegram.html</a>
