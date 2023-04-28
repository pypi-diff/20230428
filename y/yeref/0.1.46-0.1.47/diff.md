# Comparing `tmp/yeref-0.1.46.tar.gz` & `tmp/yeref-0.1.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.46.tar", last modified: Tue Apr 25 13:56:56 2023, max compression
+gzip compressed data, was "yeref-0.1.47.tar", last modified: Fri Apr 28 11:35:27 2023, max compression
```

## Comparing `yeref-0.1.46.tar` & `yeref-0.1.47.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-25 13:56:56.913917 yeref-0.1.46/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-25 13:56:56.914094 yeref-0.1.46/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-25 13:56:56.914938 yeref-0.1.46/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-25 13:56:43.000000 yeref-0.1.46/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-25 13:56:56.908894 yeref-0.1.46/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.46/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   162440 2023-04-25 13:55:33.000000 yeref-0.1.46/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   188525 2023-04-24 20:15:25.000000 yeref-0.1.46/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-25 13:56:56.913071 yeref-0.1.46/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-25 13:56:56.000000 yeref-0.1.46/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-25 13:56:56.000000 yeref-0.1.46/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-25 13:56:56.000000 yeref-0.1.46/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-25 13:56:56.000000 yeref-0.1.46/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:35:27.520586 yeref-0.1.47/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-28 11:35:27.520815 yeref-0.1.47/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-28 11:35:27.522379 yeref-0.1.47/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-28 11:35:19.000000 yeref-0.1.47/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:35:27.511388 yeref-0.1.47/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.47/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   249969 2023-04-27 19:38:16.000000 yeref-0.1.47/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   192928 2023-04-27 18:43:33.000000 yeref-0.1.47/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-28 11:35:27.519894 yeref-0.1.47/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-28 11:35:27.000000 yeref-0.1.47/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-28 11:35:27.000000 yeref-0.1.47/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-28 11:35:27.000000 yeref-0.1.47/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-28 11:35:27.000000 yeref-0.1.47/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.46/setup.py` & `yeref-0.1.47/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.46',
+      version='0.1.47',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,10 +39,10 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.46-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.47-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
```

### Comparing `yeref-0.1.46/yeref/l_.py` & `yeref-0.1.47/yeref/l_.py`

 * *Files 23% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     'en': "👩🏽‍💻 No, 0%",
     'es': "👩🏽‍💻 No, 0%",
     'fr': "👩🏽‍💻 Non, 0%",
     'zh': "👩🏽‍💻 没有，0%",
     'ar': "👩🏽‍💻 لا ، 0٪",
 }
 l_creturn_text = {
-    'ru': "✖️ Сбросить настройки по умолчанию (до рекомендуемых) для канала [<b>{0}</b>]?",
+    'ru': "✖️ <b>Сбросить</b> настройки по умолчанию (до рекомендуемых) для канала [<b>{0}</b>]?",
     'en': "✖️ Reset default settings (recommended) for channel [<b>{0}</b>]?",
     'es': "✖️ ¿Restablecer la configuración predeterminada (recomendado) para el canal [<b>{0}</b>]?",
     'fr': "✖️ Réinitialiser les paramètres par défaut (recommandé) pour la chaîne [<b>{0}</b>] ?",
     'zh': "✖️ 重置频道 [<b>{0}</b>] 的默认设置（推荐）？",
     'ar': "✖️ إعادة تعيين الإعدادات الافتراضية (مستحسن) للقناة [<b>{0}</b>]؟",
 }
 l_all_ans = {
@@ -95,20 +95,20 @@
     'en': "👇🏽 <b>Choose</b> a direction",
     'es': "👇🏽 <b>Elige</b> una dirección",
     'fr': "👇🏽 <b>Choisissez</b> une direction",
     'zh': "👇🏽<b>选择</b>方向",
     'ar': "👇🏽 <b>اختر</b> الاتجاه",
 }
 l_about = {
-    'ru': "<b>🦋 Автоворонки & чат-боты в SocialMedia</b> для:\n\n▪️таргета: @ferey_send_bot\n▪️поиска: @ferey_find_bot\n▪️постов: @ferey_post_bot\n▪️автоответов: @ferey_user_bot\n▪️канала: @ferey_chat_bot\n▪️канала: @ferey_channel_bot\n▪️рекламы: @ferey_advert_bot\n\n❗️все боты общедоступны & для общего пользования",
-    'en': "<b>🦋 SocialMedia auto funnels &amp; chatbots</b> for:\n\n▪️target: @ferey_send_bot\n▪️search: @ferey_find_bot\n▪️posts: @ferey_post_bot\n▪️auto-replies: @ferey_user_bot\n▪️channel: @ferey_chat_bot\n▪️ channel: @ferey_channel_bot\n▪️ads: @ferey_advert_bot\n\n❗️all bots are public & public",
-    'es': "<b>🦋 Embudos automáticos de redes sociales y chatbots</b> para:\n\n▪️objetivo: @ferey_send_bot\n▪️búsqueda: @ferey_find_bot\n▪️publicaciones: @ferey_post_bot\n▪️respuestas automáticas: @ferey_user_bot\n▪️canal: @ferey_chat_bot\n▪️ canal: @ferey_channel_bot\n▪️anuncios: @ferey_advert_bot\n\n❗️todos los bots son públicos y públicos",
-    'fr': "<b>🦋 Entonnoirs automatiques et chatbots des médias sociaux</b> pour :\n\n▪️cible : @ferey_send_bot\n▪️recherche : @ferey_find_bot\n▪️messages : @ferey_post_bot\n▪️réponses automatiques : @ferey_user_bot\n▪️canal : @ferey_chat_bot\n▪️ chaîne : @ferey_channel_bot\n▪️annonces : @ferey_advert_bot\n\n❗️tous les bots sont publics et publics",
-    'zh': "<b>🦋 社交媒体自动漏斗和聊天机器人</b>：\n\n▪️目标： @ferey_send_bot\n▪️搜索： @ferey_find_bot\n▪️帖子： @ferey_post_bot\n▪️自动回复： @ferey_user_bot\n▪️频道： @ferey_chat_bot\n▪️频道： @ferey_channel_bot\n▪️广告： @ferey_advert_bot\n\n❗️所有机器人都是公开的和公开的",
-    'ar': "<b>🦋 مسارات تحويل SocialMedia التلقائية وروبوتات الدردشة</b> من أجل:\n\n▪️ الهدف: @ferey_send_bot\n▪️search: @ferey_find_bot\n▪️ المشاركات: @ferey_post_bot\n▪️auto-response: @ferey_user_bot\n▪️ القناة: @ferey_chat_bot القناة: @ferey_channel_bot\n▪️ads: @ferey_advert_bot\n\n❗️ جميع البوتات عامة وعامة",
+    'ru': "<b>🦋 Автоворонки & чат-боты в SocialMedia</b> для:\n\n▪️таргета: @ferey_send_bot\n▪️поиска: @ferey_find_bot\n▪️постов: @ferey_post_bot\n▪️автоответов: @ferey_user_bot\n▪️канала: @ferey_chat_bot\n▪️канала: @ferey_chn_bot\n▪️рекламы: @ferey_advert_bot\n\n❗️все боты общедоступны & для общего пользования",
+    'en': "<b>🦋 SocialMedia auto funnels &amp; chatbots</b> for:\n\n▪️target: @ferey_send_bot\n▪️search: @ferey_find_bot\n▪️posts: @ferey_post_bot\n▪️auto-replies: @ferey_user_bot\n▪️channel: @ferey_chat_bot\n▪️ channel: @ferey_chn_bot\n▪️ads: @ferey_advert_bot\n\n❗️all bots are public & public",
+    'es': "<b>🦋 Embudos automáticos de redes sociales y chatbots</b> para:\n\n▪️objetivo: @ferey_send_bot\n▪️búsqueda: @ferey_find_bot\n▪️publicaciones: @ferey_post_bot\n▪️respuestas automáticas: @ferey_user_bot\n▪️canal: @ferey_chat_bot\n▪️ canal: @ferey_chn_bot\n▪️anuncios: @ferey_advert_bot\n\n❗️todos los bots son públicos y públicos",
+    'fr': "<b>🦋 Entonnoirs automatiques et chatbots des médias sociaux</b> pour :\n\n▪️cible : @ferey_send_bot\n▪️recherche : @ferey_find_bot\n▪️messages : @ferey_post_bot\n▪️réponses automatiques : @ferey_user_bot\n▪️canal : @ferey_chat_bot\n▪️ chaîne : @ferey_chn_bot\n▪️annonces : @ferey_advert_bot\n\n❗️tous les bots sont publics et publics",
+    'zh': "<b>🦋 社交媒体自动漏斗和聊天机器人</b>：\n\n▪️目标： @ferey_send_bot\n▪️搜索： @ferey_find_bot\n▪️帖子： @ferey_post_bot\n▪️自动回复： @ferey_user_bot\n▪️频道： @ferey_chat_bot\n▪️频道： @ferey_chn_bot\n▪️广告： @ferey_advert_bot\n\n❗️所有机器人都是公开的和公开的",
+    'ar': "<b>🦋 مسارات تحويل SocialMedia التلقائية وروبوتات الدردشة</b> من أجل:\n\n▪️ الهدف: @ferey_send_bot\n▪️search: @ferey_find_bot\n▪️ المشاركات: @ferey_post_bot\n▪️auto-response: @ferey_user_bot\n▪️ القناة: @ferey_chat_bot القناة: @ferey_chn_bot\n▪️ads: @ferey_advert_bot\n\n❗️ جميع البوتات عامة وعامة",
 }
 l_subscribe = {
     'ru': "👩🏽‍💻 <b>Оформи</b> ежемесячную <i>подписку</i>\n\n¹ на @{0}-бота [{1} ₽]\n▪️ отсутствие рекламы\n▪️ творческие задания\n² Подписка на <u>всех</u> ботов [{2} ₽]",
     'en': "👩🏽‍💻 <b>Sign up for</b> a monthly\n\n¹ <i>subscription</i> to @{0}-bot [{1} ₽]\n▪️ no ads\n▪️ creative tasks\n² Subscribe to <u>all</u> bots [{2} ₽]",
     'es': "👩🏽‍💻 <b>Regístrese para obtener</b> una\n\n¹ <i>suscripción</i> mensual a @{0}-bot [{1} ₽]\n▪️ sin anuncios\n▪️ tareas creativas\n² Suscríbase a <u>todos</u> los bots [{2} ₽]",
     'fr': "👩🏽‍💻 <b>Inscrivez-vous pour</b> un <i>abonnement</i>\n\n¹ mensuel à @{0}-bot [{1} ₽]\n▪️ pas de publicité\n▪️ tâches créatives\n² Abonnez-vous à <u>tous</u> les bots [{2} ₽]",
     'zh': "👩🏽‍💻<b>注册</b>每月\n\n¹<i>订阅</i>@{0}-bot [{1} ₽]\n▪️ 无广告\n▪️ 创意任务\n² 订阅<u>所有</u>机器人 [{2} ₽]",
@@ -484,14 +484,30 @@
     'ru': "👥 Всем",
     'en': "👥 Everyone",
     'es': "👥 Todos",
     'fr': "👥 Tout le monde",
     'zh': "👥 大家",
     'ar': "👥 الجميع",
 }
+l_channel = {
+    'ru': "⛰️ Канал",
+    'en': "👥 Everyone",
+    'es': "👥 Todos",
+    'fr': "👥 Tout le monde",
+    'zh': "👥 大家",
+    'ar': "👥 الجميع",
+}
+l_group = {
+    'ru': "⛰️ Group",
+    'en': "👥 Everyone",
+    'es': "👥 Todos",
+    'fr': "👥 Tout le monde",
+    'zh': "👥 大家",
+    'ar': "👥 الجميع",
+}
 l_ids = {
     'ru': "🙌🏽 По id",
     'en': "🙌🏽 By id",
     'es': "🙌🏽 Por identificación",
     'fr': "🙌🏽 Par identifiant",
     'zh': "🙌🏽 通过 id",
     'ar': "🙌🏽 بالمعرف",
@@ -508,38 +524,22 @@
     'ru': "👩🏽‍💻 <b>Введи</b> Ids получателей через пробельные или разделительные символы",
     'en': "👩🏽‍💻 <b>Enter</b> recipient Ids separated by spaces or separator characters",
     'es': "👩🏽‍💻 <b>Ingrese</b> las identificaciones de los destinatarios separadas por espacios o caracteres separadores",
     'fr': "👩🏽‍💻 <b>Entrez</b> les identifiants des destinataires séparés par des espaces ou des caractères de séparation",
     'zh': "👩🏽‍💻<b>输入</b>以空格或分隔符分隔的收件人 ID",
     'ar': "<b>أدخل</b> معرفات المستلمين مفصولة بمسافات أو أحرف فاصلة",
 }
-offer_has_restricted = {
-    'ru': "👩🏽‍💻 В настройках <b>[Конфиденциальность]</b> добавь @{0} в <i>исключения</i> для <b>[Голосовые сообщения]</b>, чтобы отобразить <code>видео-заметку</code>/<code>голосовое</code>",
-    'en': "👩🏽‍💻 In the <b>[Privacy]</b> settings, add @{0} to <i>the exclusions</i> for <b>[Voice Messages]</b> to display <code>видео-заметку</code> / <code>голосовое</code>",
-    'es': "👩🏽‍💻 En la configuración <b>de [Privacidad]</b> , agregue @{0} a <i>las exclusiones</i> de <b>[Mensajes de voz]</b> para mostrar <code>видео-заметку</code> / <code>голосовое</code>",
-    'fr': "👩🏽‍💻 Dans les paramètres <b>[Confidentialité]</b> , ajoutez @{0} aux <i>exclusions</i> pour <b>[Messages vocaux]</b> pour afficher <code>видео-заметку</code> / <code>голосовое</code>",
-    'zh': "👩🏽‍💻在<b>【隐私】</b>设置中，添加@{0}到<b>【语音消息】</b>的<i>排除项</i>中，以显示<code>видео-заметку</code> / <code>голосовое</code>",
-    'ar': "👩🏽‍💻 في إعدادات <b>[الخصوصية]</b> ، أضف @ {0} إلى <i>استثناءات</i> <b>[الرسائل الصوتية]</b> لعرض <code>видео-заметку</code> / <code>голосовое</code>",
-}
-offer_time_zone = {
+l_post_time_zone = {
     'ru': "📍 <b>Часовой пояс</b> геопозиции установлен\n\n🕐 Текущее время: <u>{0}</u> ({1}{2} по Гринвичу)",
     'en': "📍 Location <b>time zone</b> set\n\n🕐 Current time: <u>{0}</u> ({1}{2} GMT)",
     'es': "📍 Configuración <b>de la zona horaria</b> de la ubicación\n\n🕐 Hora actual: <u>{0}</u> ({1}{2} GMT)",
     'fr': "📍 <b>Fuseau horaire</b> de l&#x27;emplacement défini\n\n🕐 Heure actuelle : <u>{0}</u> ({1}{2} GMT)",
     'zh': "📍 位置<b>时区</b>设置\n\n🕐 当前时间： <u>{0}</u> （{1}{2} GMT）",
     'ar': "📍 تعيين <b>المنطقة الزمنية</b> للموقع\n\n🕐 الوقت الحالي: <u>{0}</u> ({1} {2} GMT)",
 }
-offer_time_future = {
-    'ru': "🕒 <b>Укажи</b> время в будущем",
-    'en': "🕒 <b>Set</b> time in the future",
-    'es': "🕒 <b>Establecer</b> tiempo en el futuro",
-    'fr': "🕒 <b>Réglez</b> l'heure dans le futur",
-    'zh': "🕒<b>设定</b>未来的时间",
-    'ar': "🕒 <b>حدد</b> الوقت في المستقبل",
-}
 l_broadcast_plan = {
     'ru': "🗝️ <b>Готово!</b> Рассылка запланирована",
     'en': "🗝️ <b>Done!</b> Newsletter scheduled",
     'es': "🗝️ <b>Listo!</b> Boletín programado",
     'fr': "🗝️ <b>C&#x27;est fait !</b> Newsletter prévue",
     'zh': "🗝️<b>完成！</b>已安排时事通讯",
     'ar': "🗝️ <b>انتهى!</b> النشرة الإخبارية المجدولة",
@@ -1908,23 +1908,23 @@
     'en': "+",
     'es': "+",
     'fr': "+",
     'zh': "+",
     'ar': "+",
 }
 l_geo_text1 = {
-    'ru': "📍 <b>Geo-поиск</b> пользователей по координатам\n\n👩🏽‍💻 Жми на -/+, чтобы настроить 📍Radius",
+    'ru': "📍 <b>Geo-поиск</b> пользователей по координатам\n\n👩🏽‍💻 <b>Жми</b> на -/+, чтобы настроить 📍Radius",
     'en': "📍 <b>Geo-search</b> users by coordinates\n\n👩🏽‍💻 Click on -/+ to adjust 📍Radius",
     'es': "📍 Usuarios <b>de búsqueda geográfica</b> por coordenadas\n\n👩🏽‍💻 Haz clic en -/+ para ajustar el 📍Radio",
     'fr': "📍 <b>Géo-recherche</b> des utilisateurs par coordonnées\n\n👩🏽‍💻 Cliquez sur -/+ pour ajuster 📍Rayon",
     'zh': "📍 按坐标<b>地理搜索</b>用户\n\n👩🏽‍💻 点击 -/+ 调整📍半径",
     'ar': "📍 <b>البحث الجغرافي</b> للمستخدمين عن طريق الإحداثيات\n\n👩🏽‍💻 انقر فوق - / + لضبط 📍Radius",
 }
 l_geo_text2 = {
-    'ru': "👩🏽‍💻 <b>Прикрепи</b> геопозицию через 📎-меню вложений или нажми на кнопку ниже\n[📍Отправить Geo] 👇🏽",
+    'ru': "👩🏽‍💻 <b>Прикрепи</b> геопозицию через 📎-меню вложений или на<b>Жми</b> на кнопку ниже\n[📍Отправить Geo] 👇🏽",
     'en': "👩🏽‍💻 <b>Attach</b> a location via the attachments 📎 menu or click the button below\n[📍Send Geo] 👇🏽",
     'es': "👩🏽‍💻 <b>Adjunte</b> una ubicación a través del menú de archivos adjuntos 📎 o haga clic en el botón a continuación\n[📍Enviar geo] 👇🏽",
     'fr': "👩🏽‍💻 <b>Joignez</b> un emplacement via le menu des pièces jointes 📎 ou cliquez sur le bouton ci-dessous\n[📍Envoyer la géo] 👇🏽",
     'zh': "👩🏽‍💻通过附件📎菜单<b>附加</b>位置或单击下面的按钮\n[📍发送地理信息]👇🏽",
     'ar': "👩🏽‍💻 <b>أرفق</b> موقعًا عبر قائمة المرفقات أو انقر فوق الزر أدناه\n[Send Geo] 👇🏽",
 }
 l_geo_send = {
@@ -2661,7 +2661,1179 @@
     'en': "👩🏽‍💻 <b>To</b> get a link to the message and the customer, subscribe to @FereyFindBot -bot:\n\nhttps://t.me",
     'es': "👩🏽‍💻 <b>Para</b> obtener un enlace al mensaje y al cliente, suscríbete a @FereyFindBot -bot:\n\nhttps://t.me",
     'fr': "👩🏽‍💻 <b>Pour</b> obtenir un lien vers le message et le client, abonnez-vous à @FereyFindBot -bot :\n\nhttps://t.me",
     'zh': "👩🏽‍💻<b>要</b>获取消息和客户的链接，请订阅@FereyFindBot -bot：\n\nhttps://t.me",
     'ar': "👩🏽‍💻 <b>للحصول</b> على ارتباط للرسالة والعميل ، اشترك في @FereyFindBot -bot:\n\nhttps: //t.me",
 }
 # endregion
+
+
+# region FereyChannelBot
+l_chn_btn1 = {
+    'ru': '⛰️ Каналы',
+    'en': "⛰️ VPN",
+    'es': "⛰️VPN",
+    'fr': "⛰️VPN",
+    'zh': "⛰️ VPN",
+    'ar': "⛰️ VPN",
+}
+l_chn_btn2 = {
+    'ru': "🌬 Подписка",
+    'en': "🌬 Subscription",
+    'es': "🌬 Suscripción",
+    'fr': "🌬 Abonnement",
+    'zh': "🌬订阅",
+    'ar': "🌬 الاشتراك",
+}
+l_chn_welcome = {
+    'ru': "🌱 {0}, добро пожаловать в <i>лендинг-бот</i> <code>администрирования</code> <b>Telegram</b>-каналов:\n\n▪️<b>защита</b> канала от вступления шпионов\n▪️вывод <b>статистики</b> и вовлеченности (%)\n▪️ограничение прав до <b>подписки</b> на канал\n▪️<b>организация</b> бана и антифлуда\n\n❗️также можно заказать разработку чат-бота в нашей студии <a href='https://t.me/{1}'>Ferey</a>",
+    'en': "🌱 {0}, welcome to <i>the landing bot</i> of the Ferey project:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
+    'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del proyecto Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
+    'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du projet Ferey :\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
+    'zh': "🌱 {0}，欢迎来到 Ferey 项目的<i>落地机器人</i>：\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
+    'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص بمشروع Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey",
+}
+l_add_chn_text = {
+    'ru': "👮🏽‍♀️ <b>Добавь</b> @{0}-бота как  <b>Administrator</b> через настройки своего канала: ‹👤Add Admin›\n\n👮🏽‍♀️ Если не добавляется канал, то измени <b>Должность</b> (см. скрин)",
+    'en': "👇🏽 Push the ‹channel› to add into your channel (with default settings): @{0}\n\n👮🏽‍♀️ Or add bot as <b>Admin</b> via Settings of your channel: ‹👤Add Admin›\n\n👮🏽‍♀️ If you can't add channel, try to change <b>Custom Title</b> (look screenshot)",
+    'es': "👇🏽 Presione ‹➕ Agregar grupo› para agregar a su grupo (con la configuración predeterminada): @{0}\n\n👮🏽‍♀️ O agregue bot como <b>Administrador</b> a través de la Configuración de su grupo: ‹👤Agregar administrador›\n\n👮🏽‍♀️ Si no puede agregar un grupo, intente cambiar <b>Título personalizado</b> (ver captura de pantalla)",
+    'fr': "👇🏽 Appuyez sur ‹➕ Ajouter un channele› pour ajouter à votre channele (avec les paramètres par défaut): @{0}\n\n👮🏽‍♀️ Ou ajoutez le bot en tant qu'<b>administrateur</b> via les paramètres de votre channele : ‹👤Ajouter un administrateur›\n\n👮🏽‍♀️ Si vous ne pouvez pas ajouter de channele, essayez de modifier le <b>Titre personnalisé</b> (regardez la capture d'écran)",
+    'zh': "👇🏽 按下‹➕添加群組›以添加到您的群組（使用默認設置）: @{0}\n\n👮🏽‍♀️ 或通過您組的設置將機器人添加為 <b>Admin</b>：‹👤添加管理員›\n\n👮🏽‍♀️ 如果無法添加組，請嘗試更改 <b>自定義標題</b>（看截圖）",
+    'ar': "👇🏽 اضغط على ‹➕ إضافة مجموعة› لإضافتها إلى مجموعتك (بالإعدادات الافتراضية): @{0}\n\n👮🏽‍♀️ أو أضف البوت كـ <b> مسؤول </b> عبر إعدادات مجموعتك: ‹👤 إضافة مسؤول›\n\n👮🏽‍♀️ إذا لم تتمكن من إضافة مجموعة ، فحاول تغيير <b> عنوان مخصص </b> (انظر في لقطة الشاشة)",
+}
+l_add_chn_txt_call = {
+    'ru': "👮🏽‍♀️ Добавь @{0}-бота как Administrator через настройки своего канала: ‹👤Add Admin›\n\n👮🏽‍♀️ Если не добавляется канал, то измени Должность",
+    'en': "👇🏽 Push the ‹channel› to add into your channel (with default settings): @{0}\n\n👮🏽‍♀️ Or add bot as <b>Admin</b> via Settings of your channel: ‹👤Add Admin›\n\n👮🏽‍♀️ If you can't add channel, try to change <b>Custom Title</b> (look screenshot)",
+    'es': "👇🏽 Presione ‹➕ Agregar grupo› para agregar a su grupo (con la configuración predeterminada): @{0}\n\n👮🏽‍♀️ O agregue bot como <b>Administrador</b> a través de la Configuración de su grupo: ‹👤Agregar administrador›\n\n👮🏽‍♀️ Si no puede agregar un grupo, intente cambiar <b>Título personalizado</b> (ver captura de pantalla)",
+    'fr': "👇🏽 Appuyez sur ‹➕ Ajouter un channele› pour ajouter à votre channele (avec les paramètres par défaut): @{0}\n\n👮🏽‍♀️ Ou ajoutez le bot en tant qu'<b>administrateur</b> via les paramètres de votre channele : ‹👤Ajouter un administrateur›\n\n👮🏽‍♀️ Si vous ne pouvez pas ajouter de channele, essayez de modifier le <b>Titre personnalisé</b> (regardez la capture d'écran)",
+    'zh': "👇🏽 按下‹➕添加群組›以添加到您的群組（使用默認設置）: @{0}\n\n👮🏽‍♀️ 或通過您組的設置將機器人添加為 <b>Admin</b>：‹👤添加管理員›\n\n👮🏽‍♀️ 如果無法添加組，請嘗試更改 <b>自定義標題</b>（看截圖）",
+    'ar': "👇🏽 اضغط على ‹➕ إضافة مجموعة› لإضافتها إلى مجموعتك (بالإعدادات الافتراضية): @{0}\n\n👮🏽‍♀️ أو أضف البوت كـ <b> مسؤول </b> عبر إعدادات مجموعتك: ‹👤 إضافة مسؤول›\n\n👮🏽‍♀️ إذا لم تتمكن من إضافة مجموعة ، فحاول تغيير <b> عنوان مخصص </b> (انظر في لقطة الشاشة)",
+}
+l_add_chn_button = {
+    'ru': "➕ Добавить канал",
+    'en': "➕ Add channel",
+    'es': "➕ Agregar grupo",
+    'fr': "➕ Ajouter un channele",
+    'zh': "➕ 添加組",
+    'ar': "➕ إضافة مجموعة",
+}
+l_bot_removed = {
+    'ru': "🚫 @{0}-бот удален из канала <b>{1}</b> (<code>{2}</code>)",
+    'en': "🚫 @{0}-бот удален из канала {1} (<code>{2}</code>)",
+    'es': "➕ Agregar grupo",
+    'fr': "➕ Ajouter un channele",
+    'zh': "➕ 添加組",
+    'ar': "➕ إضافة مجموعة",
+}
+
+l_msgConfig = {
+    ("cban", "🕵🏽", "☑"): {
+        'ru': "Авто-бан",
+        'en': "Auto-ban",
+        'es': "Prohibición automática",
+        'fr': "Interdiction automatique",
+        'zh': "自動禁止",
+        'ar': "حظر تلقائي",
+    },
+    ("cpost", "🔔", "☐"): {
+        'ru': "Авто-постинг",
+        'en': "Auto-posting",
+        'es': "Publicación automática",
+        'fr': "Publication automatique",
+        'zh': "自動發布",
+        'ar': "النشر التلقائي",
+    },
+    ("creact", "👍🏽", "☐"): {
+        'ru': "Авто-реакции",
+        'en': "System messages",
+        'es': "Mensajes del sistema",
+        'fr': "Messages système",
+        'zh': "系統消息",
+        'ar': "رسائل النظام",
+    },
+    ("cview", "👁️‍🗨️", "☐"): {
+        'ru': "Авто-просмотры",
+        'en': "System messages",
+        'es': "Mensajes del sistema",
+        'fr': "Messages système",
+        'zh': "系統消息",
+        'ar': "رسائل النظام",
+    },
+    ("cdecor", "🪄", "☐"): {
+        'ru': "Авто-декор",
+        'en': "System messages",
+        'es': "Mensajes del sistema",
+        'fr': "Messages système",
+        'zh': "系統消息",
+        'ar': "رسائل النظام",
+    },
+    ("cmember", "👥", "☐"): {
+        'ru': "Сбор подписчиков",
+        'en': "System messages",
+        'es': "Mensajes del sistema",
+        'fr': "Messages système",
+        'zh': "系統消息",
+        'ar': "رسائل النظام",
+    },
+    ("ccheck", "👮🏽", "☐"): {
+        'ru': "Запрос на вступление",
+        'en': "Join request",
+        'es': "Entrar en control",
+        'fr': "Prenez le contrôle",
+        'zh': "進入控制",
+        'ar': "أدخل السيطرة",
+    },
+}
+l_to_default = {
+    'ru': "✖️Сброс настроек",
+    'en': "✖️Restore settings",
+    'es': "✖️Restaurar configuración",
+    'fr': "✖️Restaurer les paramètres",
+    'zh': "✖️恢復設置",
+    'ar': "✖️ استعادة الإعدادات",
+}
+l_to_delete = {
+    'ru': "🚫Убрать канал",
+    'en': "🚫Put away channel",
+    'es': "🚫Guardar grupo",
+    'fr': "🚫channele de rangement",
+    'zh': "🚫收起組",
+    'ar': "🚫 أبعد المجموعة",
+}
+l_show_channels = {
+    'ru': "👩🏽‍💻 <b>Добавленные каналы</b>\n\n[команды /cmd]",
+    'en': "👩🏽‍💻 <b>Added channels</b>\n\n[commands /cmd]",
+    'es': "👩🏽‍💻 <b>Grupos añadidos</b>\n\n[comandos /cmd]",
+    'fr': "👩🏽‍💻 <b>channeles ajoutés</b>\n\n[commands /cmd]",
+    'zh': "👩🏽‍💻 <b>添加組</b>\n\n[命令 /cmd]",
+    'ar': "👩🏽‍💻 <b> المجموعات المضافة </b> \n\n [أوامر /cmd]",
+}
+l_show_settings = {
+    'ru': "⚙️ <b>Выбери</b> опцию для /cmd <i>настройки</i> [<b>{0}</b>] {1}",
+    'en': "⚙️ <b>Choose</b> option for <i>settings</i> /cmd <b>{0}</b> {1}",
+    'es': "⚙️ <b>Elegir</b> opción para <i>configuración</i> /cmd <b>{0}</b> {1}",
+    'fr': "⚙️ <b>Choisir</b> l'option pour les <i>paramètres</i> /cmd <b>{0}</b> {1}",
+    'zh': "⚙️ <i>設置</i> /cmd <b>{0}</b>{1}的<b>選擇</b>選項",
+    'ar': "⚙️ <b> اختر </b> خيار <i> الإعدادات </i> /cmd <b>{0}</b>{1}",
+}
+l_chat_join_request_handler = {
+    'ru': "👮🏽 {0}, ты отправил(а) заявку на вступление в канал <b>{1}</b>\n\n👉🏼 Выбери <i>правильный вариант</i> в соответствии с <code>заданием</code> на картинке, чтобы твоя <i>заявка</i> на вступление была <b>одобрена</b>",
+    'en': "👮🏽 {0}, you send join-request to channel <b>{1}</b>\n\n👉🏼 Choose <i>correct option</i> according to the <code>task</code> on picture to Approve your join-<i>request</i>",
+    'es': "👮🏽 {0}, envías una solicitud de unión al grupo <b>{1}</b>\n\n👉🏼 Elige la <i>opción correcta</i> según la <code>tarea</code> en la imagen para aprobar su <i>solicitud de unión</i>",
+    'fr': "👮🏽 {0}, vous envoyez une demande de participation au channele <b>{1}</b>\n\n👉🏼 Choisissez <i>l'option correcte</i> en fonction de la <code>tâche</code> sur l'image pour approuver votre inscription-<i>demande</i>",
+    'zh': "👮🏽 {0}，你發送加入請求到組 <b>{1}</b>\n\n👉🏼 根據<code>task</code>選擇<i>正確的選項</i> 在圖片上批准您的加入-<i>請求</i>",
+    'ar': "👮🏽 {0} ، ترسل طلب انضمام إلى المجموعة <b>{1}</b> \n\n👉🏼 اختر <i> الخيار الصحيح </i> وفقًا لـ <code> المهمة </code> على الصورة للموافقة على انضمامك- <i> طلب </i>",
+}
+l_content_types_sub_button = {
+    'ru': "👮🏽 Я подписался",
+    'en': "👮🏽 I subscribed",
+    'es': "👮🏽 Me suscribí",
+    'fr': "👮🏽 Je me suis abonné",
+    'zh': "👮🏽 我訂閱了",
+    'ar': "👮🏽 لقد اشتركت",
+}
+l_content_types_subscribe = {
+    'ru': "👮🏽 {0}, подпишись на {1}, чтобы вступить в канал",
+    'en': "👮🏽 {0}, subscribe on the {1} to join the channel",
+    'es': "👮🏽 {0}, suscríbete en {1} para unirte al grupo",
+    'fr': "👮🏽 {0}, abonnez-vous sur le {1} pour rejoindre le channele",
+    'zh': "👮🏽 {0}，在 {1} 上訂閱以加入群組",
+    'ar': "👮🏽 {0} ، اشترك في {1} للانضمام إلى المجموعة",
+}
+l_wait_1_min = {
+    'ru': "🕐 Подожди 1мин",
+    'en': "✖️ channel settings of [<b>{0}</b>] successfully reset!",
+    'es': "✖️ ¡La configuración de grupo de [<b>{0}</b>] se restableció correctamente!",
+    'fr': "✖️ Les paramètres de channele de [<b>{0}</b>] ont été réinitialisés !",
+    'zh': "✖️ [<b>{0}</b>] 的群組設置已成功重置！",
+    'ar': "✖️ تمت إعادة تعيين إعدادات المجموعة لـ [<b>{0}</b>] بنجاح!",
+}
+
+l_creturn_answer = {
+    'ru': "✖️ Настройки канала [<b>{0}</b>] успешно сброшены!",
+    'en': "✖️ channel settings of [<b>{0}</b>] successfully reset!",
+    'es': "✖️ ¡La configuración de grupo de [<b>{0}</b>] se restableció correctamente!",
+    'fr': "✖️ Les paramètres de channele de [<b>{0}</b>] ont été réinitialisés !",
+    'zh': "✖️ [<b>{0}</b>] 的群組設置已成功重置！",
+    'ar': "✖️ تمت إعادة تعيين إعدادات المجموعة لـ [<b>{0}</b>] بنجاح!",
+}
+l_cdelete_text = {
+    'ru': "🚫 Убрать привязку бота к канале [<b>{0}</b>]?",
+    'en': "🚫 Put away bot-connection with channel [<b>{0}</b>]?",
+    'es': "🚫 ¿Eliminar la conexión de bot con el grupo [<b>{0}</b>]?",
+    'fr': "🚫 Mettre de côté la connexion au bot avec le channele [<b>{0}</b>] ?",
+    'zh': "🚫 放棄與組 [<b>{0}</b>] 的機器人連接？",
+    'ar': "🚫 التخلص من اتصال الروبوت بالمجموعة [<b>{0}</b>]؟",
+}
+l_cdelete_answer = {
+    'ru': "🚫 <b>Бот</b> успешно отвязан от канала [<b>{0}</b>] и не числится его в участниках!",
+    'en': "🚫 Bot successfully disconnected from channel [<b>{0}</b>] and it is not a member at all!",
+    'es': "🚫 ¡El bot se desconectó con éxito del grupo [<b>{0}</b>] y no es miembro en absoluto!",
+    'fr': "🚫 Le bot s'est déconnecté avec succès du channele [<b>{0}</b>] et il n'est pas du tout membre !",
+    'zh': "🚫 Bot 已成功與群組 [<b>{0}</b>] 斷開連接，並且它根本不是成員！",
+    'ar': "🚫 تم قطع اتصال البوت بنجاح بالمجموعة [<b>{0}</b>] وهو ليس عضوًا على الإطلاق!",
+}
+
+l_chn_CCHECKBTNNAME = {
+    'ru': "✔ Я человек",
+    'en': "✔ I am human",
+    'es': "✔ Soy humana",
+    'fr': "✔ Je suis humain",
+    'zh': "✔ 我是人",
+    'ar': "✔ أنا إنسان",
+}
+l_chn_CHELLOTEXT = {
+    'ru': "🌱 {name}, добро пожаловать в нашу <b>канал</b> {title}!",
+    'en': "🌱 {name}, welcome to our <b>channel</b> {title}!",
+    'es': "🌱 {name}, Bienvenida a nuestro <b>grupo</b> {title}!",
+    'fr': "🌱 {name}, bienvenue dans notre <b>channele</b> {title}!",
+    'zh': "🌱 {name}, 歡迎加入我們的<b>群</b> {title}!",
+    'ar': "🌱 {name} ، مرحبًا بك في <b> مجموعتنا </ b> {title}!"
+}
+l_chn_CCHECKCHANNEL = {
+    'ru': "👮🏽 Для <i>проверки подписки</i> необходимо добавить канал командой:\n\n/channel ССЫЛКА НА КАНАЛ",
+    'en': "👮🏽 It is necessary add channel for <i>subscribe checking</i> by command:\n\n/channel LINK",
+    'es': "👮🏽 Es necesario agregar un canal para <i>comprobar suscripciones</i> mediante el comando:\n\n/channel LINK",
+    'fr': "👮🏽 Il est nécessaire d'ajouter un canal pour <i>vérifier l'abonnement</i> par la commande :\n\n/channel LINK",
+    'zh': "👮🏽 <i>訂閱檢查</i>需要通過命令添加頻道：\n\n/channel LINK",
+    'ar': "👮🏽 من الضروري إضافة قناة لـ <i> فحص الاشتراك </i> بواسطة الأمر: \n\n/channel LINK",
+}
+
+
+# region commands
+l_update_text = {
+    'ru': "👩🏽‍💻 Данные о канале успешно обновлены:\n\n<b>{0}</b> [<code>{1}</code>]\n{2}\n<i>{3}</i>\n\n⚙️ <b>Команды</b> /cmd",
+    'en': "➕ Add channel",
+    'es': "➕ Agregar grupo",
+    'fr': "➕ Ajouter un channele",
+    'zh': "➕ 添加組",
+    'ar': "➕ إضافة مجموعة",
+}
+l_commands_handler = {
+    'ru': "⚙️ <b>Настройка</b> канала <b>{0}</b> {1}\n\n<b>⛏ Admin-команды @{2}</b>\n/update <i>обновление параметров</i>\n/transfer   <i>передача admin-прав</i>\n/info   <i>информация</i>\n/stat   <i>статистика</i>\n/parse  <i>выгрузка базы подписчиков</i>\n/videochat 1 1 <i>анонс видео-трансляции</i>\n/clean  <i>долгая очистка канала от deleted/scam/fake-аккаунтов, а также по 🕵🏽 Авто-бан правилам</i>\n/channel NAME   <i>добавить канал для проверки подписки</i>",
+    'en': "⚙️ <b>channel</b> settings of <b>{0}</b> {1}\n\n<b>⛏ Admin-commands @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+    'es': "⚙️ Configuración de <b>Grupo</b> de <b>{0}</b> {1}\n\n<b>⛏ Comandos de administración @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+    'fr': "⚙️ Paramètres de <b>channele</b> de <b>{0}</b> {1}\n\n<b>⛏ Commandes d'administration @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+    'zh': "⚙️ <b>組</b>設置 <b>{0}</b> {1}\n\n<b>⛏ 管理員命令 @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/log   <i>see logs</i>\n/parse  <i>[all|old|premium|active|online]</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+    'ar': "⚙️ إعدادات <b> المجموعة </b> الخاصة بـ <b>{0}</b> {1}\n\n<b>⛏ أوامر المسؤول @{2}</b>\n/update <i>parameters</i>\n/transfer   <i>admin-settings</i>\n/info   <i>information</i>\n/stat   <i>statistics</i>\n/parse  <i>[all|old|premium|active|online]</i>\n/log   <i>see logs</i>\n<code>/parse old</code> - <i>parsing old id-accounts</i>\n\n/channel NAME   <i>add channel for subscribe checking</i>\n/button NAME    <i>add button's name for Enter Control</i>\n/delay MIN      <i>set delay number [min] for 1st message</i>\n/flood NUM      <i>set msg-number for flood</i>\n\n<b>⛏ Commands for other administrations</b>\n/ban 5m|1h|10d <i>delete from channel for time</i>\n/unban\n/mute 5m|1h|10d <i>restriction in channel for time</i>\n/unmute\n/warn+msg <i>warning</i>\n/status\n/karma  [+|-]\n/tag+msg   <i>@tager random-accounts</i>\n\n<b>⛏ Commands for users</b>\n/help   <i>show commands</i>\n/rules  <i>for channel</i>\n/report <i>about violation</i>\n/happy  <i>get happyness</i>\n/thanks <i>say to user thank you</i>",
+}
+l_info_restrict = {
+    'ru': "<code>запрещено</code>\n",
+    'en': "<code>prohibited</code>\n",
+    'es': "<code>prohibida</code>\n",
+    'fr': "<code>interdite</code>\n",
+    'zh': "<code>禁止</code>\n",
+    'ar': "<code>محظور</code>\n",
+}
+l_info_allow = {
+    'ru': "<code>разрешено</code>\n",
+    'en': "<code>allowed</code>\n",
+    'es': "<code>permitida</code>\n",
+    'fr': "<code>permise</code>\n",
+    'zh': "<code>允許</code>\n",
+    'ar': "<code>مسموح</code>\n",
+}
+l_info_protect = {
+    'ru': "<b>Сохранение контента</b>: ",
+    'en': "<b>Saving Content</b>: ",
+    'es': "<b>Guardar contenido</b>:",
+    'fr': "<b>Enregistrement du contenu</b> :",
+    'zh': "<b>保存內容</b>：",
+    'ar': "<b> حفظ المحتوى </b>:",
+}
+l_info_request = {
+    'ru': "<b>Вступление после одобрения</b>: ",
+    'en': "<b>Approve New Members</b>: ",
+    'es': "<b>Aprobar nuevos miembros</b>:",
+    'fr': "<b>Approuver les nouveaux membres</b> :",
+    'zh': "<b>批准新成員</b>：",
+    'ar': "<b> قبول الأعضاء الجدد </b>:",
+}
+l_info_send = {
+    'ru': "<b>Возможность писать после вступления</b>: ",
+    'en': "<b>Join to send message</b>: ",
+    'es': "<b>Únete para enviar un mensaje</b>:",
+    'fr': "<b>Rejoindre pour envoyer un message</b> :",
+    'zh': "<b>加入發送消息</b>：",
+    'ar': "<b> انضم لإرسال رسالة </b>:",
+}
+l_info_subscribe = {
+    'ru': "<b>Проверка подписки при вступлении в канал</b>: ",
+    'en': "<b>Check subscription to join</b>: ",
+    'es': "<b>Verifique la suscripción para unirse</b>:",
+    'fr': "<b>Vérifier l'abonnement pour rejoindre</b> :",
+    'zh': "<b>檢查訂閱以加入</b>：",
+    'ar': "<b> تحقق من الاشتراك للانضمام </b>:",
+}
+l_info_oppforpart = {
+    'ru': "Возможности подписчиков",
+    'en': "Participants opportunities",
+    'es': "Oportunidades de los participantes",
+    'fr': "Opportunités pour les participants",
+    'zh': "參與者機會",
+    'ar': "فرص المشاركين",
+}
+l_info_cmd = {
+    'ru': "⚙️ <b>Команды</b> /cmd",
+    'en': "Participants opportunities",
+    'es': "Oportunidades de los participantes",
+    'fr': "Opportunités pour les participants",
+    'zh': "參與者機會",
+    'ar': "فرص المشاركين",
+}
+
+l_change_chn_info = {
+    'ru': "Изменение профиля канала",
+    'en': "Change channel Info",
+    'es': "Cambiar información del grupo",
+    'fr': "Modifier les informations du channele",
+    'zh': "更改組信息",
+    'ar': "تغيير معلومات المجموعة",
+}
+l_pin_message = {
+    'ru': "Закрепление сообщений",
+    'en': "Pin Messages",
+    'es': "Mensajes de pines",
+    'fr': "Épingler les messages",
+    'zh': "固定消息",
+    'ar': "تثبيت الرسائل",
+}
+l_add_members = {
+    'ru': "Добавление участников",
+    'en': "Add Members",
+    'es': "Añadir miembros",
+    'fr': "Ajouter des membres",
+    'zh': "添加成員",
+    'ar': "إضافة أعضاء",
+}
+l_embed_links = {
+    'ru': "Предпросмотр ссылок",
+    'en': "Embed links",
+    'es': "Insertar enlaces",
+    'fr': "Intégrer des liens",
+    'zh': "嵌入鏈接",
+    'ar': "روابط التضمين",
+}
+l_send_messages = {
+    'ru': "Отправка сообщений",
+    'en': "Send Messages",
+    'es': "Enviar mensajes",
+    'fr': "Envoyer des messages",
+    'zh': "發送信息",
+    'ar': "إرسل رسائل",
+}
+l_send_media = {
+    'ru': "Отправка фото и видео",
+    'en': "Send Media",
+    'es': "Enviar medios",
+    'fr': "Envoyer le média",
+    'zh': "發送媒體",
+    'ar': "إرسال الوسائط",
+}
+l_send_polls = {
+    'ru': "Отправка опросов",
+    'en': "Send Polls",
+    'es': "Enviar encuestas",
+    'fr': "Envoyer des sondages",
+    'zh': "發送投票",
+    'ar': "إرسال استطلاعات الرأي",
+}
+l_send_stickers = {
+    'ru': "Отправка sticker/giff/via_bot",
+    'en': "Send sticker/giff/via_bot",
+    'es': "apagada",
+    'fr': "à l'arrêt",
+    'zh': "離開",
+    'ar': "إيقاف",
+}
+l_info_reactions = {
+    'ru': "Допуск emoji-реакций",
+    'en': "Allowed emoji-reactions",
+    'es': "Emoji-reacciones permitidas",
+    'fr': "Emoji-réactions autorisées",
+    'zh': "允許的表情符號反應",
+    'ar': "ردود فعل الرموز التعبيرية المسموح بها",
+}
+l_admins = {
+    'ru': "Администраторы",
+    'en': "Administrators",
+    'es': "Administradoras",
+    'fr': "Administratrices",
+    'zh': "管理員",
+    'ar': "المسؤولين",
+}
+l_info_anonymous_for = {
+    'ru': "Анонимность для",
+    'en': "Anonymous for",
+    'es': "Anónimo para",
+    'fr': "Anonyme pour",
+    'zh': "匿名",
+    'ar': "مجهول لـ",
+}
+l_info_invite_admins = {
+    'ru': "Приглашение других админов для",
+    'en': "Promote admins for",
+    'es': "Promocionar administradores para",
+    'fr': "Promouvoir les administrateurs pour",
+    'zh': "提升管理員為",
+    'ar': "قم بترقية المسؤولين لـ",
+}
+l_info_start1 = {
+    'ru': "ℹ️ <b>Общая информация о канале</b>\n\n<b>Название</b>: {0} [id=<code>{1}</code>, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
+    'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
+    'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
+    'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
+    'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
+    'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
+}
+l_stat_start1 = {
+    'ru': "ℹ️ <b>Общая статистика канала</b>\n\n<b>Название</b>: {0} [id=<code>{1}</code>, <i>{2} {3}</i>, <u>{4}</u> участ.]{5}{6}{7}",
+    'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
+    'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
+    'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
+    'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
+    'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
+}
+l_stat_start2 = {
+    'ru': "\n<b>Ссылка</b>: {0}\n<b>Описание</b>: {1}\n<b>Привязанная группа</b>: <code>{2}</code>\n",
+    'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
+    'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
+    'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
+    'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
+    'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
+}
+l_stat_start3 = {
+    'ru': "\n<b>ID последнего поста</b>: {0}\n<b>Посты</b>: {1}\n<b>Реакции</b>: {2}\n<b>Просмотры</b>: {3}\n<b>Комментарии</b>: {4}\n<b>$кэштеги</b>: {5}\n<b>#хэштеги</b>: {6}\n",
+    'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
+    'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
+    'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
+    'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
+    'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
+}
+l_top_hashtags = {
+    'ru': "\n<b>Топ #хэштеги</b>:\n{0}\n",
+    'en': "ℹ️ <b>Common info about channel statistics</b>\n\n",
+    'es': "ℹ️ <b>Información común sobre las estadísticas del grupo</b>\n\n",
+    'fr': "ℹ️ <b>Informations communes sur les statistiques de channele</b>\n\n",
+    'zh': "ℹ️ <b>關於組統計的常見信息</b>\n\n",
+    'ar': "ℹ️ <b> معلومات عامة حول إحصائيات المجموعة </b> \n\n",
+}
+
+l_stat_top5users = {
+    'ru': "Топ 5 пользователей (на 1000 сообщ)",
+    'en': "Top 5 users (for 1000 msgs)",
+    'es': "Las 5 mejores usuarios (para 1000 msgs)",
+    'fr': "Top 5 des utilisateurs (pour 1000 msgs)",
+    'zh': "前 5 名用戶（1000 條消息）",
+    'ar': "أعلى 5 مستخدمين (لكل 1000 رسالة)",
+}
+l_stat_top5msgs = {
+    'ru': "Топ 5 сообщ (из 1000)",
+    'en': "Top 5 msgs (from 1000)",
+    'es': "Las 5 mejores mensajes (desde 1000)",
+    'fr': "Top 5 des messages (sur 1000)",
+    'zh': "前 5 條消息（來自 1000 條）",
+    'ar': "أهم 5 رسائل (من 1000)",
+}
+l_transfer_start = {
+    'ru': "⚠️ Пользователь {0} должен /start-запустить @{1}",
+    'en': "⚠️ User {0} have to /start @{1}",
+    'es': "⚠️ El usuario {0} debe /iniciar @{1}",
+    'fr': "⚠️ L'utilisateur {0} doit /start @{1}",
+    'zh': "⚠️ 用戶 {0} 必須 /start @{1}",
+    'ar': "⚠️ المستخدم {0} يجب أن يبدأ @{1}",
+}
+l_transfer_admin = {
+    'ru': "⚠️ Пользователь {0} должен быть <b>администратором</b> канала <b>{1}</b>",
+    'en': "⚠️ User {0} have to be <b>admin</b> of channel <b>{1}</b>",
+    'es': "⚠️ El usuario {0} debe ser <b>administrador</b> del grupo <b>{1}</b>",
+    'fr': "⚠️ L'utilisateur {0} doit être <b>admin</b> du channele <b>{1}</b>",
+    'zh': "⚠️ 用戶 {0} 必須是組 <b>{1}</b> 的 <b>admin</b>",
+    'ar': "⚠️ يجب أن يكون المستخدم {0}<b> مسؤولًا </b> للمجموعة <b>{1}</b>",
+}
+l_transfer_transfer = {
+    'ru': "⚠️ Вы уверены, что хотите передать <b>admin</b>-права на канал <b>{0}</b> пользователю {1} в @{2}-боте?",
+    'en': "⚠️ Are you sure to transfer ownership of channel <b>{0}</b> to user {1} in @{2}?",
+    'es': "⚠️ ¿Estás seguro de transferir la propiedad del grupo <b>{0}</b> al usuario {1} en @{2}?",
+    'fr': "⚠️ Êtes-vous sûr de transférer la propriété du channele <b>{0}</b> à l'utilisateur {1} dans @{2} ?",
+    'zh': "⚠️ 您確定將組 <b>{0}</b> 的所有權轉讓給 @{2} 中的用戶 {1}？",
+    'ar': "⚠️ هل أنت متأكد من نقل ملكية المجموعة <b>{0}</b> إلى المستخدم {1} في @{2}؟",
+}
+l_transfer_text = {
+    'ru': "⚠️ Для передачи admin-прав канала в @{0}-боте используй команду: <code>/transfer ID-ПОЛЬЗОВАТЕЛЯ</code> (/id), где пользователь: администратор канала и участник @{0}-бота\n\n⚙️ <b>Команды</b> /cmd",
+    'en': "⚠️ Use /transfer-command in reply user-message to transfer him ownership",
+    'es': "⚠️ Use /transfer-command en el mensaje de usuario de respuesta para transferirle la propiedad",
+    'fr': "⚠️ Utilisez /transfer-command dans le message utilisateur de réponse pour lui transférer la propriété",
+    'zh': "⚠️ 使用 /transfer-command 回复 user-message 轉移他的所有權",
+    'ar': "استخدم الأمر transfer-command/ في الرد على رسالة المستخدم لنقل ملكيته",
+}
+l_transfer_done_to = {
+    'ru': "⚠️ <b>Admin</b>-права на канал [<b>{0}</b>] успешно переданы {1}",
+    'en': "⚠️ <b>Admin</b>-privileges for channel [<b>{0}</b>] are successfully transferred to {1}",
+    'es': "⚠️ <b>Administrador</b>: los privilegios del grupo [<b>{0}</b>] se transfirieron correctamente a {1}",
+    'fr': "⚠️ Les privilèges <b>Admin</b> pour le channele [<b>{0}</b>] ont été transférés avec succès vers {1}",
+    'zh': "⚠️ <b>Admin</b>-組 [<b>{0}</b>] 的權限已成功轉移到 {1}",
+    'ar': "⚠️ تم نقل امتيازات <b> المسؤول </b> للمجموعة [<b>{0}</b>] بنجاح إلى {1}",
+}
+l_transfer_done_from = {
+    'ru': "⚠️ <b>Admin</b>-права на канал [<b>{0}</b>] успешно получены от {1}",
+    'en': "⚠️ <b>Admin</b>-privileges for channel [<b>{0}</b>] are successfully received from {1}",
+    'es': "⚠️ <b>Administrador</b>: los privilegios para el grupo [<b>{0}</b>] se recibieron correctamente de {1}",
+    'fr': "⚠️ Les privilèges <b>Admin</b> pour le channele [<b>{0}</b>] ont bien été reçus de {1}",
+    'zh': "⚠️ <b>Admin</b>-組 [<b>{0}</b>] 的權限已從 {1} 成功接收",
+    'ar': "⚠️ تم استلام امتيازات <b> المسؤول </b> للمجموعة [<b>{0}</b>] بنجاح من {1}",
+}
+l_chn_check = {
+    'ru': "⚙️ Добавь @{0}-бота в канал для проверки подписки на него. Пришли мне корректную ссылку на канал:",
+    'en': "⚙️ Add @{0} to channel for subscribe checking. Send me correct link to channel:",
+    'es': "⚙️ Agregue @{0} al canal para verificar la suscripción. Envíame el enlace correcto al canal:",
+    'fr': "⚙️ Ajoutez @{0} à la chaîne pour vérifier l'abonnement. Envoyez-moi le lien correct vers la chaîne :",
+    'zh': "⚙️ 將@{0} 添加到頻道以進行訂閱檢查。 向我發送正確的頻道鏈接：",
+    'ar': "⚙️ إضافة @{0} للقناة للتحقق من الاشتراك. أرسل لي الرابط الصحيح للقناة:",
+}
+l_chn_done = {
+    'ru': "👮🏽 Готово! Проверка подписки на {0}-канал настроена\n\nОпцию можно включить в настройках, нажав [✅☑Вкл подписку]",
+    'en': "👮🏽 Ready! Subscribe checking to {0}-channel is configured\n\nEnable this option in the Settings by pushing [✅☑Enable subscription]",
+    'es': "👮🏽 Listo! La verificación de suscripción a {0}-canal está configurada\n\nActive esta opción en Configuración presionando [✅☑Habilitar suscripción]",
+    'fr': "👮🏽 Prêt! La vérification de l'abonnement à la chaîne {0} est configurée\n\nActivez cette option dans les paramètres par push [✅☑Activer l'abonnement]",
+    'zh': "👮🏽 準備好了！ 已配置對 {0} 頻道的訂閱檢查\n\n通過推送在“設置”中打開此選項 [✅☑啟用訂閱]",
+    'ar': "👮🏽 جاهز! التحقق من الاشتراك في {0} - تم تكوين القناة \n\n قم بتشغيل هذا الخيار في الإعدادات عن طريق الدفع [✅☑ تمكين الاشتراك]",
+}
+l_parse_rights = {
+    'ru': "👩🏽‍💻 В настройках [Администраторы] вкл опцию для @{0}-бота:\n[✅ Назначение администраторов]\n\n🕚Подожди 1min",
+    'en': "In the Settings [Administrators] for @{0} enable:\n[✅ Delete Msgs]\n[✅ Ban Users]\n[✅ Invite Users]\n🕚Wait for 1min",
+    'es': "En la Configuración [Administradores] para @{0} active:\n[✅ Eliminar mensajes]\n[✅ Prohibir usuarios]\n[✅ Invitar usuarios]\n🕚Espere 1 minuto",
+    'fr': "Dans les paramètres [Administrateurs] pour @{0}, activez :\n[✅ Supprimer les messages]\n[✅ Bannir les utilisateurs]\n[✅ Inviter des utilisateurs]\n🕚Attendez 1 minute",
+    'zh': "在@{0}的設置[管理員]中打開：\n[✅刪除消息]\n[✅禁止用戶]\n[✅邀請用戶]\n🕚等待1分鐘",
+    'ar': " في الإعدادات [Administrators] لـ @{0} شغّل:\n [✅ حذف الرسائل] \n على [✅ حظر المستخدمين] \n [✅ دعوة المستخدمين] \n وانتظر لمدة دقيقة واحدة",
+}
+l_videochat_rights = {
+    'ru': "🎥 В настройках [Администраторы] вкл опцию для @{0}-бота:\n[✅ Назначение администраторов]\n[✅ Управление трансляциями]\n\n🕚Подожди 1min",
+    'en': "In the Settings [Administrators] for @{0} enable:\n[✅ Delete Msgs]\n[✅ Ban Users]\n[✅ Invite Users]\n🕚Wait for 1min",
+    'es': "En la Configuración [Administradores] para @{0} active:\n[✅ Eliminar mensajes]\n[✅ Prohibir usuarios]\n[✅ Invitar usuarios]\n🕚Espere 1 minuto",
+    'fr': "Dans les paramètres [Administrateurs] pour @{0}, activez :\n[✅ Supprimer les messages]\n[✅ Bannir les utilisateurs]\n[✅ Inviter des utilisateurs]\n🕚Attendez 1 minute",
+    'zh': "在@{0}的設置[管理員]中打開：\n[✅刪除消息]\n[✅禁止用戶]\n[✅邀請用戶]\n🕚等待1分鐘",
+    'ar': " في الإعدادات [Administrators] لـ @{0} شغّل:\n [✅ حذف الرسائل] \n على [✅ حظر المستخدمين] \n [✅ دعوة المستخدمين] \n وانتظر لمدة دقيقة واحدة",
+}
+l_videochat_handler = {
+    'ru': "🎥 Автоматическое анонсирование <b>видео-трансляции</b> <code>[/videochat d h]</code> каждый <u>d</u>-день (1-31) на <u>h</u>-часов (1-168). Текущее значение: /videochat {0}\n\n👩🏽‍💻 Например,\n<code>/videochat 1 1</code> (ежедневный видео-анонс длительностью 1 час)\n<code>/videochat 0</code> (отключение опции)\n\n⚙️ <b>Команды</b> /cmd",
+    'en': "🎥 Send this command as reply to message",
+    'es': "🎥 Enviar este comando como respuesta al mensaje",
+    'fr': "🎥 Envoyez cette commande en réponse au message",
+    'zh': "🎥 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_videochat_on = {
+    'ru': "🎥 Анонсирована <b>видео-трансляция</b>: каждый <u>{0}</u> день на <u>{1}</u> часов\n\n⚙️ <b>Команды</b> /cmd",
+    'en': "🎥 Send this command as reply to message",
+    'es': "🎥 Enviar este comando como respuesta al mensaje",
+    'fr': "🎥 Envoyez cette commande en réponse au message",
+    'zh': "🎥 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_videochat_off = {
+    'ru': "🎥 Анонсирование <b>видео-трансляции</b> отключено\n\n⚙️ <b>Команды</b> /cmd",
+    'en': "🎥 Send this command as reply to message",
+    'es': "🎥 Enviar este comando como respuesta al mensaje",
+    'fr': "🎥 Envoyez cette commande en réponse au message",
+    'zh': "🎥 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_ban_users_start = {
+    'ru': "👩🏽‍💻 Начинаем очистку канала\nТекущее количество пользователей: {0}",
+    'en': "🎥 Send this command as reply to message",
+    'es': "🎥 Enviar este comando como respuesta al mensaje",
+    'fr': "🎥 Envoyez cette commande en réponse au message",
+    'zh': "🎥 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_ban_users_stop = {
+    'ru': "👩🏽‍💻 Очистка завершена\nТекущее количество пользователей {0} (-{1})",
+    'en': "🎥 Send this command as reply to message",
+    'es': "🎥 Enviar este comando como respuesta al mensaje",
+    'fr': "🎥 Envoyez cette commande en réponse au message",
+    'zh': "🎥 將此命令作為對消息的回復發送",
+    'ar': "🎉 أرسل هذا الأمر كرد على الرسالة",
+}
+l_ccheck_handler = {
+    'ru': "👮🏽 <b>Жми</b> на ✅/🔘, чтобы <b>переключить</b> тип <i>проверки</i> пользователя при <u>вступлении</u> по сгенерированной ссылке: {0} (только для <code>ЧАСТНЫХ</code> каналов)\n\n👉🏼 Для <b>проверки подписки</b> на другой канал <i>добавь</i> @{1}-бота в канал и выполни команду: <code>/channel {2}</code>\n\n👉🏼 Для <i>защиты от атаки</i> на канал включи режим <b>антирейд</b> (блокировка <u>всех</u> вступающих)",
+    'en': "👮🏽 Push the ✅/🔘 to <b>switch</b> <i>Enter control</i> of user <u>joining</u> into channel\n\n👉🏼 To set name of <b>pushing button</b> execute command: <code>/button {0}</code>\n\n👉🏼 To check <b>channel-subscription</b> <i>add</i> @{1} to channel and execute command: <code>/channel {2}</code>\n\n👉🏼 To <i>defend</i> from channel-attack switch <b>anti-raid</b>-mode (ban <u>everyone</u> who joining)",
+    'es': "👮🏽 Presiona ✅/🔘 para <b>cambiar</b> <i>Enter control</i> del usuario <u>uniéndose</u> al grupo\n\n👉🏼 Para establecer el nombre de <b> presionando el botón</b> ejecute el comando: <code>/button {0}</code>\n\n👉🏼 Para verificar <b>channel-subscription</b> <i>add</i> @{1} para canalizar y ejecutar el comando: <code>/channel {2}</code>\n\n👉🏼 Para <i>defender</i> del ataque grupal, active el modo <b>anti-raid</b> (prohibir a <u>todos</u> que se unan)",
+    'fr': "👮🏽 Appuyez sur ✅/🔘 pour <b>commuter</b> <i>Entrez le contrôle</i> de l'utilisateur <u>rejoignant</u> le channele\n\n👉🏼 Pour définir le nom de <b> en appuyant sur le bouton</b> exécutez la commande : <code>/button {0}</code>\n\n👉🏼 Pour vérifier <b>channel-subscription</b> <i>add</i> @{1} pour canaliser et exécuter la commande : <code>/channel {2}</code>\n\n👉🏼 Pour <i>se défendre</i> contre une attaque de channele, activez le mode <b>anti-raid</b> (bannir <u>tous ceux</u> qui se joignent)",
+    'zh': "👮🏽 按下 ✅/🔘 來<b>切換</b> <i>進入控制</i> 用戶<u>加入</u> 入組\n\n👉🏼 設置<b>的名字 按下按鈕</b> 執行命令：<code>/button {0}</code>\n\n👉🏼 檢查<b>頻道訂閱</b> <i>add</i> @{1} 引導並執行命令：<code>/channel {2}</code>\n\n👉🏼 以 <i>defend</i> 免受群攻開啟 <b>anti-raid</b>-mode （禁止加入的<u>每個人</u>）",
+    'ar': "👮🏽 ادفع ✅ / 🔘 إلى <b> التبديل </b> <i> أدخل التحكم </i> للمستخدم <u> المنضم </u> إلى مجموعة \n\n👉🏼 لتعيين اسم <b> ضغط الزر </b> نفذ الأمر: <code> / button {0}</code>\n\n👉🏼 للتحقق من <b> اشتراك القناة </b> <i> إضافة </i> @{1} لتوجيه وتنفيذ الأمر: <code> / channel {2}</code>\n\n👉🏼 <i> للدفاع </i> من هجوم المجموعة ، شغّل وضع <b> anti-raid </b> (حظر <u> كل شخص </u> من ينضم)",
+}
+l_ccheck_call = {
+    'ru': "👮🏽 Для проверки подписки необходимо добавить дополнительный канал командой:\n\n/channel ССЫЛКА НА КАНАЛ",
+    'en': "👮🏽 To check <i>subscription</i> you have to add channel by command:\n\n/channel LINK",
+    'es': "👮🏽 Para verificar la <i>suscripción</i>, debe agregar el canal mediante el comando:\n\n/channel LINK",
+    'fr': "👮🏽 Pour vérifier l'<i>abonnement</i>, vous devez ajouter une chaîne par commande :\n\n/channel LINK",
+    'zh': "👮🏽 要檢查<i>訂閱</i>，您必須通過命令添加頻道：\n\n/channel LINK",
+    'ar': "👮🏽 للتحقق من <i> اشتراك </i> ، عليك إضافة قناة بأمر: \n\n/ channel LINK",
+}
+l_ccheck_call2 = {
+    'ru': "👮🏽 В настройках [Администраторы] вкл опцию для @{0}-бота:\n[✅ Удаление сообщ]\n[✅ Блокировка польз]\n[✅ Добавление участ]\n\n🕚Подожди 1min",
+    'en': "👮🏽 In the Settings [Administrators] for @{0} enable:\n[✅ Delete Msgs]\n[✅ Ban Users]\n[✅ Invite Users]\n🕚Wait for 1min",
+    'es': "👮🏽 En la Configuración [Administradores] para @{0} active:\n[✅ Eliminar mensajes]\n[✅ Prohibir usuarios]\n[✅ Invitar usuarios]\n🕚Espere 1 minuto",
+    'fr': "👮🏽 Dans les paramètres [Administrateurs] pour @{0}, activez :\n[✅ Supprimer les messages]\n[✅ Bannir les utilisateurs]\n[✅ Inviter des utilisateurs]\n🕚Attendez 1 minute",
+    'zh': "👮🏽 在@{0}的設置[管理員]中打開：\n[✅刪除消息]\n[✅禁止用戶]\n[✅邀請用戶]\n🕚等待1分鐘",
+    'ar': " في الإعدادات [Administrators] لـ @{0} شغّل:\n [✅ حذف الرسائل] \n على [✅ حظر المستخدمين] \n [✅ دعوة المستخدمين] \n وانتظر لمدة دقيقة واحدة",
+}
+l_ccheck_free_on = {
+    'ru': "✅☑Вкл свободный вход",
+    'en': "✅☑On free entrance",
+    'es': "✅☑En entrada libre",
+    'fr': "✅☑En entrée libre",
+    'zh': "✅☑免費入場",
+    'ar': "✅☑ الدخول مجاني",
+}
+l_ccheck_free_off = {
+    'ru': "🔘️☐Выкл свободный вход",
+    'en': "🔘️☐Off free entrance",
+    'es': "🔘️☐De Entrada libre",
+    'fr': "🔘️☐De entrée gratuite",
+    'zh': "🔘️☐免費入場",
+    'ar': "🔘️☐ من الدخول المجاني",
+}
+l_ccheck_button_on = {
+    'ru': "✅☑Вкл нажатие на кнопку",
+    'en': "✅☑On button push",
+    'es': "✅☑En el pulsador",
+    'fr': "✅☑En bouton poussoir",
+    'zh': "✅☑按按鈕",
+    'ar': "✅☑عند الضغط على زر",
+}
+l_ccheck_button_off = {
+    'ru': "🔘️☐Выкл нажатие на кнопку",
+    'en': "🔘️☐Off button push",
+    'es': "🔘️☐De pulsar botón",
+    'fr': "🔘️☐De bouton poussoir",
+    'zh': "🔘️☐關閉按鈕按下",
+    'ar': "🔘️☐زر الضغط",
+}
+l_ccheck_subscribe_on = {
+    'ru': "✅☑Вкл подписку",
+    'en': "✅☑On subscription",
+    'es': "✅☑En suscripción",
+    'fr': "✅☑En abonnement",
+    'zh': "✅☑啟用訂閱",
+    'ar': "✅☑ تمكين الاشتراك",
+}
+l_ccheck_subscribe_off = {
+    'ru': "🔘☐Выкл подписку",
+    'en': "🔘☐Off subscription",
+    'es': "🔘️☐De suscripción",
+    'fr': "🔘️☐De abonnement",
+    'zh': "🔘☐禁用訂閱",
+    'ar': "🔘☐ تعطيل الاشتراك",
+}
+l_ccheck_captcha_on = {
+    'ru': "✅☑Вкл решение капчи",
+    'en': "✅☑On captcha",
+    'es': "✅☑En captcha",
+    'fr': "✅☑En captcha",
+    'zh': "✅☑啟用驗證碼",
+    'ar': "✅☑ تمكين كلمة التحقق",
+}
+l_ccheck_captcha_off = {
+    'ru': "🔘️☐Выкл решение капчи",
+    'en': "🔘️☐Off captcha",
+    'es': "🔘️☐De captcha",
+    'fr': "🔘️☐De captcha",
+    'zh': "🔘️☐禁用驗證碼",
+    'ar': "🔘️☐ تعطيل كلمة التحقق",
+}
+l_ccheck_request_on = {
+    'ru': "✅☑Вкл подачу заявки",
+    'en': "✅☑On send request",
+    'es': "✅☑En enviar petición",
+    'fr': "✅☑En envoyer une demande",
+    'zh': "✅☑啟用發送請求",
+    'ar': "✅☑ تمكين إرسال الطلب",
+}
+l_ccheck_request_off = {
+    'ru': "🔘️☐Выкл подачу заявки",
+    'en': "🔘️☐Off send request",
+    'es': "🔘️☐De enviar petición",
+    'fr': "🔘️☐De envoyer une demande",
+    'zh': "🔘️☐禁用發送請求",
+    'ar': "🔘️☐ تعطيل إرسال الطلب",
+}
+l_ccheck_antiraid_on = {
+    'ru': "✅☑Вкл анти-рейд",
+    'en': "✅☑On anti-raid",
+    'es': "✅☑En anti-raid",
+    'fr': "✅☑En anti-raid",
+    'zh': "✅☑啟用反襲擊",
+    'ar': "✅☑ تمكين مكافحة الغارة",
+}
+l_ccheck_antiraid_off = {
+    'ru': "🔘️☐Выкл антирейд",
+    'en': "🔘️☐Off anti-raid",
+    'es': "🔘️☐De anti-raid",
+    'fr': "🔘️☐De anti-raid",
+    'zh': "🔘️☐禁用反襲擊",
+    'ar': "🔘️☐ تعطيل مكافحة الغارة",
+}
+
+l_ccheckconfig_handler = {
+    'ru': "Текущий добавленный канал",
+    'en': "Current added channel",
+    'es': "Canal agregado actual",
+    'fr': "Chaîne actuellement ajoutée",
+    'zh': "當前添加的頻道",
+    'ar': "القناة المضافة الحالية",
+}
+l_ccheckchannel_link = {
+    'ru': "👮🏽 Ссылка на {0} не доступна",
+    'en': "👮🏽 Link for {0} is invalid",
+    'es': "👮🏽 El enlace para {0} no es válido",
+    'fr': "👮🏽 Le lien pour {0} n'est pas valide",
+    'zh': "👮🏽 {0} 的鏈接無效",
+    'ar': "👮🏽 ارتباط {0} غير صالح",
+}
+l_ccheckchannel_chn = {
+    'ru': "👮🏽 Ты не вступил в {0}\n\nПопробуй ещё раз позже",
+    'en': "👮🏽 You are not join to {0}\n\nTry again later",
+    'es': "👮🏽 No te has unido a {0}\n\nInténtalo de nuevo más tarde",
+    'fr': "👮🏽 您沒有加入 {0}\n\n 請稍後再試",
+    'zh': "👮🏽 您沒有加入 {0}\n\n 請稍後再試",
+    'ar': "👮🏽 أنت لست مشتركًا في {0} \n\n حاول مرة أخرى لاحقًا",
+}
+l_ccheck_ban = {
+    'ru': "👮🏽‍ Пользователь <b>{0}</b> не прошел входной контроль",
+    'en': "👮🏽 User {0} did not pass Enter Control and have been deleted from this channel",
+    'es': "👮🏽 El usuario {0} no pasa el control de entrada y ha sido eliminado de este grupo",
+    'fr': "👮🏽 L'utilisateur {0} ne passe pas Enter Control et a été supprimé de ce channele",
+    'zh': "👮🏽 用戶 {0} 未通過 Enter Control 並已從該組中刪除",
+    'ar': "👮🏽 المستخدم {0} لا يجتاز إدخال التحكم وقد تم حذفه من هذه المجموعة",
+}
+
+l_ccheckchannel_error = {
+    'ru': "👮🏽 Ошибка проверки",
+    'en': "👮🏽 Error of checking",
+    'es': "👮🏽 Error de verificación",
+    'fr': "👮🏽 Erreur de vérification",
+    'zh': "👮🏽檢查錯誤",
+    'ar': "👮🏽 خطأ في الفحص",
+}
+l_ccheck_wrong = {
+    'ru': "👮🏽 К сожалению, ответ неверный\n\nПопробуйте ещё раз позже",
+    'en': "👮🏽 Unfortunately the answer is not correct\n\nTry again later",
+    'es': "👮🏽 Lamentablemente la respuesta no es correcta\n\nVuelve a intentarlo más tarde",
+    'fr': "👮🏽 Malheureusement, la réponse n'est pas correcte\n\nRéessayez plus tard",
+    'zh': "👮🏽 很遺憾答案不正確\n\n稍後再試",
+    'ar': "👮🏽 للأسف الإجابة غير صحيحة \n\n حاول مرة أخرى لاحقًا",
+}
+l_ccheck_time = {
+    'ru': "👮🏽 Входной контроль пройден за {0} sec",
+    'en': "👮🏽 Enter Control passed for {0} sec",
+    'es': "👮🏽 Control de entrada superado durante {1} seg.",
+    'fr': "👮🏽 Entrez le contrôle passé pendant {1} sec",
+    'zh': "👮🏽 輸入控制已通過 {1} 秒",
+    'ar': "👮🏽 أدخل التحكم الذي تم تمريره لمدة {1} ثانية",
+}
+
+# endregion
+
+
+# region chello_
+l_chello_your_hello = {
+    'ru': "Ваше приветствие",
+    'en': "Your greeting",
+    'es': "Tu saludo",
+    'fr': "Votre message d'accueil",
+    'zh': "你的問候",
+    'ar': "تحياتك",
+}
+l_chello_text = {
+    'ru': "👋🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> приветствие, а также его ⚙️Настроить\n\n👉🏼 Например, <code>{0}</code>{1}",
+    'en': "👋🏽 Push the ✅/☑️, to <b>On/Off</b> greeting, and to ⚙️Configure\n\n👉🏼 For example, <code>{0}</code>{1}",
+    'es': "👋🏽 Presione ✅/☑️, para <b>Activar/Desactivar</b> el saludo y para ⚙️Configurar\n\n👉🏼 Por ejemplo, <code>{0}</code>{1}",
+    'fr': "👋🏽 Appuyez sur ✅/☑️, sur <b>Activer/Désactiver</b> le message d'accueil et sur ⚙️Configurer\n\n👉🏼 Par exemple, <code>{0}</code>{1}",
+    'zh': "👋🏽 按下 ✅/☑️、<b>On/Off</b> 問候語和 ⚙️Configure\n\n👉🏼 例如，<code>{0}</code>{1}",
+    'ar': "👋🏽 اضغط على ✅ / ☑️ ، من أجل <b> تشغيل / إيقاف </b> الترحيب ، و تكوين \n\n👉🏼 على سبيل المثال ، <code>{0}</code>{1}",
+}
+l_btn_on = {
+    'ru': "✅☑Вкл",
+    'en': "✅☑On",
+    'es': "✅☑En",
+    'fr': "✅☑En",
+    'zh': "✅☑使能夠",
+    'ar': "✅☑ تمكين",
+}
+l_btn_off = {
+    'ru': "☑️☐Выкл",
+    'en': "☑️☐Off",
+    'es': "☑️☐De",
+    'fr': "☑️☐De",
+    'zh': "☑️☐禁用",
+    'ar': "☑️☐ تعطيل",
+}
+l_btn_settings = {
+    'ru': "⚙️Настроить",
+    'en': "⚙️Configure",
+    'es': "⚙️Configurar",
+    'fr': "⚙️Configurer",
+    'zh': "⚙️配置",
+    'ar': "⚙️ تكوين",
+}
+l_chellochange_handler = {
+    'ru': "👋🏽 Отправь мне <b>текст</b>/<b>медиа</b> контент с текстом: фото/гиф/видео/аудио/документ или запиши голосовое/видео-заметку в кружке\n\n👉🏼 Например, <code>{0}</code>",
+    'en': "👋🏽 Send me <b>text</b>/<b>media</b> content with text: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 For example, <code>{0}</code>",
+    'es': "👋🏽 Envíame contenido de <b>texto</b>/<b>medios</b> con texto: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 Par exemple, <code>{0}</code>",
+    'fr': "👋🏽 Envoyez-moi du contenu <b>texte</b>/<b>média</b> avec du texte: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 Par exemple, <code>{0}</code>",
+    'zh': "👋🏽 向我發送帶有文本的 <b>text</b>/<b>media</b> 內容: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 例如, <code>{0}</code>",
+    'ar': "👋🏽 أرسل لي محتوى <b> نصًا </b> / <b> وسائط </b> مع نص: photo/giff/video/audio/document or voice/video-note\n\n👉🏼 فمثلا, <code>{0}</code>",
+}
+l_fsm_hello_finish = {
+    'ru': "👋🏽 Приветствие записано!\n\nОпцию можно включить в настройках [👋🏽Авто-приветствие], нажав [✅☑Вкл]",
+    'en': "👋🏽 Greeting is recorded!\n\nYou can enable this option in the Settings [👋🏽Auto-greeting], by pushing [✅☑On]",
+    'es': "👋🏽 ¡Se graba el saludo!\n\nPuede habilitar esta opción en la Configuración [👋🏽Auto-saludo], presionando [✅☑On]",
+    'fr': "👋🏽 Le message d'accueil est enregistré !\n\nVous pouvez activer cette option dans les paramètres [👋🏽Auto-salutation], en appuyant sur [✅☑On]",
+    'zh': "👋🏽問候語已錄製！\n\n您可以在設置[👋🏽自動問候語]中啟用此選項，方法是按[✅☑On]",
+    'ar': "👋🏽 تم تسجيل الترحيب!\n\n يمكنك تمكين هذا الخيار في الإعدادات [الترحيب التلقائي] ، بالضغط على [تشغيل]",
+}
+
+# endregion
+
+
+# region cban_
+l_cban_handler = {
+    'ru': "🕵🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <u>авто</u>-бан <i>аккаунтов с недавно зарегистрированными new-id/без @username/аккаунтов из <a href='https://cas.chat'>Anti-Spam Системы</a>/аккаунтов с 文-глиф, ب-араб, <a href='https://www.zalgo.org'>zalgo-символами</a></i>\n\n👉🏼 Например, опция <b>new-id</b> блокирует аккаунты со <i>свежим</i> <u>id</u>",
+    'en': "🕵🏽 Push the ✅/☑️, to <b>On/Off</b> <u>auto</u>-ban <i>accounts with recently registered new-id/deleted-accounts/accounts from <a href='https://cas.chat'>Anti-Spam System</a>/accounts with 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 For example, the option <b>deleted-ban</b> delete such accounts: <i>👻 Deleted account [scam,fake]</i>",
+    'es': "🕵🏽 Presiona ✅/☑️, para <b>Encender/Apagar</b> <u>Auto</u>-banear <i>cuentas con nueva identificación registrada recientemente/cuentas eliminadas/cuentas de <a href='https://cas.chat'>Anti-Spam System</a>/cuentas con 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 Por ejemplo, la opción <b>deleted-ban</b> elimina dichas cuentas: <i>👻 Cuenta eliminada [estafa, falsa]</i>",
+    'fr': "🕵🏽 Appuyez sur ✅/☑️, pour <b>On/Off</b> <u>auto</u>-bannir <i>les comptes avec un nouvel identifiant/des comptes supprimés/des comptes récemment enregistrés depuis <a href='https://cas.chat'>Anti-Spam System</a>/comptes avec 文-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 Par exemple, l'option <b>deleted-ban</b> supprime ces comptes : <i>👻 Compte supprimé [arnaque, faux]</i>",
+    'zh': "🕵🏽 按下 ✅/☑️，以 <b>On/Off</b> <u>auto</u>-禁止 <i>具有最近從 註冊的 new-id/deleted-accounts/accounts <a href='https://cas.chat'>Anti-Spam System</a>/accounts with text-glif, ب-arab, <a href='https://www.zalgo.org'>zalgo-symbols</a></i>\n\n👉🏼 例如，選項 <b>deleted-ban</b> 刪除此類帳戶：<i>👻 Deleted account [scam,fake]</i>",
+    'ar': "🕵🏽 اضغط على ✅ / ☑️ ، إلى <b> تشغيل / إيقاف </b> <u> تلقائي </u> -حظر <i> الحسابات ذات المعرف الجديد / الحسابات / الحسابات المحذوفة حديثًا من <a href='https://cas.chat'> نظام مكافحة البريد العشوائي </a> / حسابات مع 文 -glif، ب- arab، <a href='https://www.zalgo.org'> zalgo-icons </a> </i> \n\n👉🏼 على سبيل المثال ، الخيار <b> حذف-حظر </b> يحذف مثل هذه الحسابات: <i> 👻 الحساب المحذوف [احتيال ، وهمي] </i>",
+}
+l_cban_new_on = {
+    'ru': "✅☑Вкл new-id-бан",
+    'en': "✅☑On new-id-ban",
+    'es': "✅☑En nueva-id-ban",
+    'fr': "✅☑En nouveau-id-ban",
+    'zh': "✅☑啟用新身份證",
+    'ar': "✅☑ تمكين حظر معرف جديد",
+}
+l_cban_new_off = {
+    'ru': "☑️☐Выкл new-id-бан",
+    'en': "☑️☐Off new-id-ban",
+    'es': "☑️☐De nueva-id-ban",
+    'fr': "☑️☐De nouveau-id-ban",
+    'zh': "☑️☐關閉新身份證",
+    'ar': "☑️☐ تعطيل حظر معرف جديد",
+}
+l_cban_nousername_on = {
+    'ru': "✅☑Вкл без @username-бан",
+    'en': "✅☑On deleted-ban",
+    'es': "✅☑En eliminadad-ban",
+    'fr': "✅☑En supprimé-ban",
+    'zh': "✅☑啟用已刪除的禁令",
+    'ar': "✅☑ تمكين الحظر المحذوف",
+}
+l_cban_nousername_off = {
+    'ru': "☑️☐Выкл без @username-бан",
+    'en': "☑️☐Off deleted-ban",
+    'es': "☑️☐De eliminadad-ban",
+    'fr': "☑️☐De supprimé-ban",
+    'zh': "☑️☐禁用已刪除的禁令",
+    'ar': "☑️☐ تعطيل الحظر المحذوف",
+}
+l_cban_cas_on = {
+    'ru': "✅☑Вкл CAS-бан",
+    'en': "✅☑On CAS-ban",
+    'es': "✅☑En CAS-ban",
+    'fr': "✅☑En CAS-ban",
+    'zh': "✅☑使能夠 CAS-ban",
+    'ar': "✅☑ يُمكَِن CAS-ban",
+}
+l_cban_cas_off = {
+    'ru': "☑️☐Выкл CAS-бан",
+    'en': "☑️☐Off CAS-ban",
+    'es': "☑️☐De CAS-ban",
+    'fr': "☑️☐De CAS-ban",
+    'zh': "☑️☐禁用 CAS-ban",
+    'ar': "☑️☐ تعطيل CAS-ban",
+}
+l_cban_symbols_on = {
+    'ru': "✅☑Вкл 文ب-бан",
+    'en': "✅☑On 文ب-ban",
+    'es': "✅☑En 文ب-ban",
+    'fr': "✅☑En 文ب-ban",
+    'zh': "✅☑使能夠 文ب-ban",
+    'ar': "✅☑ يُمكَِن 文ب-ban",
+}
+l_cban_symbols_off = {
+    'ru': "☑️☐Выкл 文ب-бан",
+    'en': "☑️☐Off 文ب-ban",
+    'es': "☑️☐De 文ب-ban",
+    'fr': "☑️☐De 文ب-ban",
+    'zh': "☑️☐禁用 文ب-ban",
+    'ar': "☑️☐ تعطيل 文ب-ban",
+}
+l_cban_zalgo_on = {
+    'ru': "✅☑Вкл zalgo-бан",
+    'en': "✅☑On zalgo-ban",
+    'es': "✅☑En zalgo-ban",
+    'fr': "✅☑En zalgo-ban",
+    'zh': "✅☑使能夠 zalgo-ban",
+    'ar': "✅☑ يُمكَِن zalgo-ban",
+}
+l_cban_zalgo_off = {
+    'ru': "☑️☐Выкл zalgo-бан",
+    'en': "☑️☐Off zalgo-ban",
+    'es': "☑️☐De zalgo-ban",
+    'fr': "☑️☐De zalgo-ban",
+    'zh': "☑️☐禁用 zalgo-ban",
+    'ar': "☑️☐ تعطيل zalgo-ban",
+}
+l_cpost_call = {
+    'ru': "🔔 Нужно ⚙️Настроить хотя бы один пост",
+    'en': "🔔 You have to  ⚙️Configure at least one post",
+    'es': "🔔 Tienes que ⚙️Configurar al menos una publicación",
+    'fr': "🔔 Vous devez ⚙️Configurer au moins une publication",
+    'zh': "🔔 你必須⚙️至少配置一篇帖子",
+    'ar': "🔔 يجب عليك ⚙️ تكوين منشور واحد على الأقل",
+}
+l_cpost_text = {
+    'ru': "🔔 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> <b>авто</b>-постинг сообщений в канал по дате\n\n👉🏼 Текущее количество постов <u>{0}</u>",
+    'en': "🔔 Push the ✅/☑️, to <b>On/Off</b> <b>auto</b>-posting of messages to channel by datetime\n\n👉🏼 Current post number is <u>{0}</u>",
+    'es': "🔔 Presiona ✅/☑️ para <b>activar/desactivar</b> <b>automático</b>: publicación de mensajes para agrupar por fecha y hora\n\n👉🏼 El número de publicación actual es <u>{0}</u>",
+    'fr': "🔔 Appuyez sur ✅/☑️, sur <b>On/Off</b> <b>auto</b>-publication des messages pour channeler par datetime\n\n👉🏼 Le numéro de publication actuel est <u>{0}</u>",
+    'zh': "🔔 將 ✅/☑️ 推到 <b>On/Off</b> <b>auto</b>- 將消息發佈到按日期時間分組\n\n👉🏼 當前帖子編號是 <u>{0}</u>",
+    'ar': "🔔 اضغط على ✅ / ☑️ ، من أجل <b> تشغيل / إيقاف </b> <b> تلقائي </b> - النشر التلقائي للرسائل إلى التجميع حسب التاريخ والوقت \n\n👉🏼 رقم المنشور الحالي هو <u>{0}</u>"
+}
+l_fsm_post_call = {
+    'ru': "🔔 В настройках [Администраторы] вкл опцию для @{0}-бота:\n[✅ Отправка сообщений]\n[✅ Редактирование постов]\n\n🕚Подожди 1min",
+    'en': "🔔 In the Settings [Administrators] enable:\n[✅ Pin Messages] for @{0}",
+    'es': "🔔 En la Configuración [Administradores] habilite:\n[✅ Pinear mensajes] para @{0}",
+    'fr': "🔔 Dans les paramètres [Administrateurs], activez :\n[✅ Épingler les messages] pour @{0}",
+    'zh': "🔔 在設置 [Administrators] 中啟用：\n[✅ Pin Messages] for @{0}",
+    'ar': "🔔 في الإعدادات ، فعّل [المسؤولون]: \n [✅ تثبيت الرسائل] لـ @{0}",
+}
+l_fsm_post_pin_call = {
+    'ru': "🔔 В настройках [Администраторы] вкл опцию для @{0}-бота:\n[✅ Закрепление сообщений]\n\n🕚Подожди 1min",
+    'en': "🔔 In the Settings [Administrators] enable:\n[✅ Pin Messages] for @{0}",
+    'es': "🔔 En la Configuración [Administradores] habilite:\n[✅ Pinear mensajes] para @{0}",
+    'fr': "🔔 Dans les paramètres [Administrateurs], activez :\n[✅ Épingler les messages] pour @{0}",
+    'zh': "🔔 在設置 [Administrators] 中啟用：\n[✅ Pin Messages] for @{0}",
+    'ar': "🔔 في الإعدادات ، فعّل [المسؤولون]: \n [✅ تثبيت الرسائل] لـ @{0}",
+}
+# endregion
+
+
+# region creact_
+l_creact_text = {
+    'ru': "👍🏽 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> креативные авто-реакции на последний пост канала\n\n👩🏽‍💻 Используй команду /react {0}, чтобы задать количество авто-реакций на пост(<b>текущее</b> количество: <u>{0}</u>)",
+    'en': "👍🏽 Push the ✅/☑️, to <b>On/Off</b> auto-inviting users to your channel\n\n👉🏼 Inviting <u>{0}</u> users per day from channel {1}",
+    'es': "👍🏽 Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👉🏼 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "👍🏽 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre channele\n\n👉🏼 Inviter <u>{0}</u> utilisateurs par jour à partir du channele {1}",
+    'zh': "👍🏽 按下 ✅/☑️, 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👉🏼 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶 ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👉🏼 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
+}
+l_creact_call = {
+    'ru': "👍🏽 В настройках [Администраторы] для @{0} вкл:\n[✅ Добавление участ]\n\n🕚Подожди 1min",
+    'en': "\n\nIn the Settings [Administrators] for @{0} enable:\n[✅ Delete Msgs]\n[✅ Ban Users]\n[✅ Invite Users]\n🕚Wait for 1min",
+    'es': "\n\nEn la Configuración [Administradores] para @{0} active:\n[✅ Eliminar mensajes]\n[✅ Prohibir usuarios]\n[✅ Invitar usuarios]\n🕚Espere 1 minuto",
+    'fr': "\n\nDans les paramètres [Administrateurs] pour @{0}, activez :\n[✅ Supprimer les messages]\n[✅ Bannir les utilisateurs]\n[✅ Inviter des utilisateurs]\n🕚Attendez 1 minute",
+    'zh': "\n\n在@{0}的設置[管理員]中打開：\n[✅刪除消息]\n[✅禁止用戶]\n[✅邀請用戶]\n🕚等待1分鐘",
+    'ar': "\n\n في الإعدادات [Administrators] لـ @{0} شغّل:\n [✅ حذف الرسائل] \n على [✅ حظر المستخدمين] \n [✅ دعوة المستخدمين] \n وانتظر لمدة دقيقة واحدة",
+}
+l_creact_correct = {
+    'ru': "👍🏽 Введи корректное <b>число</b> креативных авто-реакций на последний пост канала\n\n👩🏽‍💻 Используй команду <code>/react {0}</code>, чтобы задать количество авто-реакций (<b>текущее</b> количество: <u>{0}</u>)",
+    'en': "👍🏽 Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
+    'es': "👍🏽 Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
+    'fr': "👍🏽 Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
+    'zh': "👍🏽 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
+    'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
+}
+l_creact_on = {
+    'ru': "👍🏽 Готово! Текущее количество <b>авто-реакций</b> на пост канала установлено в значение <u>{0}</u>",
+    'en': "👍🏽 Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
+    'es': "👍🏽 Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
+    'fr': "👍🏽 Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
+    'zh': "👍🏽 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
+    'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
+}
+l_creact_off = {
+    'ru': "👍🏽 Режим /react-авто-реакций отключен",
+    'en': "👍🏽 Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
+    'es': "👍🏽 Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
+    'fr': "👍🏽 Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
+    'zh': "👍🏽 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
+    'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
+}
+# endregion
+
+
+# region cview_
+l_cview_text = {
+    'ru': "👁️‍🗨️ <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-просмотры поста канала\n\n👩🏽‍💻 Используй команду /view {0}, чтобы задать количество авто-просмотров (<b>текущее</b> количество: <u>{0}</u>)",
+    'en': "👁️‍🗨️ Push the ✅/☑️, to <b>On/Off</b> auto-inviting users to your channel\n\n👉🏼 Inviting <u>{0}</u> users per day from channel {1}",
+    'es': "👁️‍🗨️ Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👉🏼 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "👁️‍🗨️ Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre channele\n\n👉🏼 Inviter <u>{0}</u> utilisateurs par jour à partir du channele {1}",
+    'zh': "👁️‍🗨️ 按下 ✅/☑️, 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👉🏼 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶 ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👉🏼 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
+}
+l_cview_call = {
+    'ru': "👁️‍🗨️ В настройках [Администраторы] для @{0} вкл:\n[✅ Добавление участ]\n\n🕚Подожди 1min",
+    'en': "\n\nIn the Settings [Administrators] for @{0} enable:\n[✅ Delete Msgs]\n[✅ Ban Users]\n[✅ Invite Users]\n🕚Wait for 1min",
+    'es': "\n\nEn la Configuración [Administradores] para @{0} active:\n[✅ Eliminar mensajes]\n[✅ Prohibir usuarios]\n[✅ Invitar usuarios]\n🕚Espere 1 minuto",
+    'fr': "\n\nDans les paramètres [Administrateurs] pour @{0}, activez :\n[✅ Supprimer les messages]\n[✅ Bannir les utilisateurs]\n[✅ Inviter des utilisateurs]\n🕚Attendez 1 minute",
+    'zh': "\n\n在@{0}的設置[管理員]中打開：\n[✅刪除消息]\n[✅禁止用戶]\n[✅邀請用戶]\n🕚等待1分鐘",
+    'ar': "\n\n في الإعدادات [Administrators] لـ @{0} شغّل:\n [✅ حذف الرسائل] \n على [✅ حظر المستخدمين] \n [✅ دعوة المستخدمين] \n وانتظر لمدة دقيقة واحدة",
+}
+l_cview_correct = {
+    'ru': "👁️‍🗨️ Введи корректное <b>число</b> авто-просмотров последнего поста канала\n\n👩🏽‍💻 Используй команду <code>/view {0}</code>, чтобы задать количество авто-просмотров (<b>текущее</b> количество: <u>{0}</u>)",
+    'en': "👁️‍🗨️ Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
+    'es': "👁️‍🗨️ Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
+    'fr': "👁️‍🗨️ Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
+    'zh': "👁️‍🗨️ 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
+    'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
+}
+l_cview_on = {
+    'ru': "👁️‍🗨️ Готово! Текущее количество <b>авто-просмотров</b> на последний пост канала установлено в значение <u>{0}</u>",
+    'en': "👁️‍🗨️ Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
+    'es': "👁️‍🗨️ Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
+    'fr': "👁️‍🗨️ Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
+    'zh': "👁️‍🗨️ 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
+    'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
+}
+l_cview_off = {
+    'ru': "👁️‍🗨️ Режим /view-авто-просмотров отключен",
+    'en': "👁️‍🗨️ Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
+    'es': "👁️‍🗨️ Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
+    'fr': "👁️‍🗨️ Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
+    'zh': "👁️‍🗨️ 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
+    'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
+}
+# endregion
+
+
+# region cdecor_
+l_cdecor_text = {
+    'ru': "🪄 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> авто-декор публикуемого поста: <i><b>пагинация</b> (порядковый номер поста)/креативный <b>формат текста</b> (<b>жирный</b>/<i>курсив</i>/<u>подчеркнутый</u>/<code>моно</code>/<tg-spoiler>спойлер</tg-spoiler>/#хэштег/<a href='{0}'>ссылка</a>)/<b>футер</b> (текстовое окончание поста)</i>\n\n👉🏼 Например, опция <b>[✅☑Вкл формат текста]</b> означает креативное изменение поста с использованием 7 стилей",
+    'en': "🪄 Push the ✅/☑️, to <b>On/Off</b> <i>externak <b>links</b>/telegram-<b>links</b>/forward</i>-<b>links</b>\n\n👉🏼 For example, [✅☑On forward-links] means permission on <b>forward</b> messages from <u>other</u> Telegram-<i>channels/channels/accounts</i> into <u>our</u> channel",
+    'es': "🪄 Presiona ✅/☑️ para <b>Activar/Desactivar</b> <i>externak <b>enlaces</b>/telegram-<b>enlaces</b>/reenviar</i>-<b>enlaces</b>\n\n👉🏼 Por ejemplo, [✅☑On forward-links] significa permiso en <b>reenviar</b> mensajes de <u>otros</u> Telegram-<i>canales /grupos/cuentas</i> en <u>nuestro</u> grupo",
+    'fr': "🪄 Appuyez sur le ✅/☑️, sur <b>On/Off</b> <i>externak <b>links</b>/telegram-<b>links</b>/forward</i>-<b>liens</b>\n\n👉🏼 Par exemple, [✅☑On forward-links] signifie l'autorisation de <b>transférer</b> les messages provenant d'<u>autres</u> chaînes Telegram-<i> /channeles/comptes</i> dans <u>notre</u> channele",
+    'zh': "🪄 將 ✅/☑️ 推到 <b>On/Off</b> <i>externak <b>links</b>/telegram-<b>links</b>/forward</i>-<b>links</b>\n\n👉🏼 例如，[✅☑On forward-links] 表示允許 <b>forward</b> 來自 <u>other</u> Telegram-<i> 頻道的消息 /channels/accounts</i> 進入 <u>我們的</u> 組",
+    'ar': "🔗 ادفع ✅ / ☑️ إلى تشغيل / إيقاف روابط خارجية telegram- روابط/ إعادة توجيه الروابط \n\n👉🏼 على سبيل المثال ، [على روابط إعادة التوجيه] تعني إذنًا بشأن <b> إعادة توجيه </b> الرسائل من أخرى Telegram قنوات/channels/accounts في مجموعتنا",
+}
+l_cdecor_footer_call = {
+    'ru': "🪄 Футер пустой, необходимо его ⚙️Настроить",
+    'en': "🪄 There are no greetings you need to ⚙️Configure",
+    'es': "🪄 No hay saludos que necesites ⚙️Configurar",
+    'fr': "🪄 Vous n'avez pas besoin de salutations ⚙️Configurer",
+    'zh': "🪄 無需問候⚙️配置",
+    'ar': "🔔لا توجد تحيات تحتاج إلى تكوين",
+}
+l_cdecor_footer_call2 = {
+    'ru': "🪄 В настройках [Администраторы] вкл опцию для @{0}-бота:\n[✅ Редактирование постов]\n\n🕚Подожди 1min",
+    'en': "🪄 In the Settings [Administrators] enable:\n[✅ Pin Messages] for @{0}",
+    'es': "🪄 En la Configuración [Administradores] habilite:\n[✅ Pinear mensajes] para @{0}",
+    'fr': "🪄 Dans les paramètres [Administrateurs], activez :\n[✅ Épingler les messages] pour @{0}",
+    'zh': "🪄 在設置 [Administrators] 中啟用：\n[✅ Pin Messages] for @{0}",
+    'ar': "🔔 في الإعدادات ، فعّل [المسؤولون]: \n [✅ تثبيت الرسائل] لـ @{0}",
+}
+l_cdecor_footer_config = {
+    'ru': "🪄 Введи краткий <b>текст</b>, который будет добавляться в окончание к постам канала (например, часто используемые #хэштеги)",
+    'en': "🪄 There are no greetings you need to ⚙️Configure",
+    'es': "🪄 No hay saludos que necesites ⚙️Configurar",
+    'fr': "🪄 Vous n'avez pas besoin de salutations ⚙️Configurer",
+    'zh': "🪄 無需問候⚙️配置",
+    'ar': "🔔لا توجد تحيات تحتاج إلى تكوين",
+}
+l_cdecor_footer_done = {
+    'ru': "🪄 Готово! <b>Футер</b> из <u>{0}</u>-символов будет использоваться как окончание поста в канале\n\nОпцию можно включить, нажав <b>[✅☑Вкл футер]</b>",
+    'en': "🪄 There are no greetings you need to ⚙️Configure",
+    'es': "🪄 No hay saludos que necesites ⚙️Configurar",
+    'fr': "🪄 Vous n'avez pas besoin de salutations ⚙️Configurer",
+    'zh': "🪄 無需問候⚙️配置",
+    'ar': "🔔لا توجد تحيات تحتاج إلى تكوين",
+}
+l_cdecor_page_on = {
+    'ru': "✅☑Вкл пагинация",
+    'en': "✅☑On external links",
+    'es': "✅☑En enlaces externos",
+    'fr': "✅☑En Liens externes",
+    'zh': "✅☑使能夠 外部鏈接",
+    'ar': "✅☑ يُمكَِن روابط خارجية",
+}
+l_cdecor_page_off = {
+    'ru': "☑️☐Выкл пагинация",
+    'en': "☑️☐Off external links",
+    'es': "☑️☐De enlaces externos",
+    'fr': "☑️☐De Liens externes",
+    'zh': "☑️☐禁用 外部鏈接",
+    'ar': "☑️☐ تعطيل روابط خارجية",
+}
+l_cdecor_footer_on = {
+    'ru': "✅☑Вкл футер",
+    'en': "✅☑On @telegram links",
+    'es': "✅☑En enlaces @telegram",
+    'fr': "✅☑En Liens @telegram",
+    'zh': "✅☑使能夠 @telegram-鏈接",
+    'ar': "✅☑ يُمكَِن @telegram-الروابط",
+}
+l_cdecor_footer_off = {
+    'ru': "☑️☐Выкл футер",
+    'en': "☑️☐Off @telegram-links",
+    'es': "☑️☐De @telegram-enlaces",
+    'fr': "☑️☐De @telegram-Liens",
+    'zh': "☑️☐禁用 @telegram-鏈接",
+    'ar': "☑️☐ تعطيل @telegram-الروابط",
+}
+l_cdecor_format_on = {
+    'ru': "✅☑Вкл формат текста",
+    'en': "✅☑On forward-links",
+    'es': "✅☑En forward-enlaces",
+    'fr': "✅☑En forward-Liens",
+    'zh': "✅☑使能夠 forward-鏈接",
+    'ar': "✅☑ يُمكَِن forward-الروابط",
+}
+l_cdecor_format_off = {
+    'ru': "☑️☐Выкл формат текста",
+    'en': "☑️☐Off forward-links",
+    'es': "☑️☐De forward-enlaces",
+    'fr': "☑️☐De forward-Liens",
+    'zh': "☑️☐禁用 forward-鏈接",
+    'ar': "☑️☐ تعطيل forward-الروابط",
+}
+# endregion
+
+
+# region cmember_
+l_cmember_text = {
+    'ru': "👥 <b>Жми</b> на ✅/☑️, чтобы <b>Вкл/Выкл</b> сбор подписчиков канала (с момента подключения бота в канал)\n\n👩🏽‍💻 Для выгрузки подписчиков канала выполните команду /parse",
+    'en': "👥 Push the ✅/☑️, to <b>On/Off</b> auto-inviting users to your channel\n\n👉🏼 Inviting <u>{0}</u> users per day from channel {1}",
+    'es': "👥 Presiona ✅/☑️ para <b>activar/desactivar</b> la invitación automática de usuarios a tu grupo\n\n👉🏼 Invitar a <u>{0}</u> usuarios por día del grupo {1}",
+    'fr': "👥 Appuyez sur ✅/☑️, pour <b>Activer/Désactiver</b> l'invitation automatique d'utilisateurs dans votre channele\n\n👉🏼 Inviter <u>{0}</u> utilisateurs par jour à partir du channele {1}",
+    'zh': "👥 按下 ✅/☑️, 以<b>開/關</b>自動邀請用戶加入您的群組\n\n👉🏼 每天從群組 {1} 中邀請 <u>{0}</u> 個用戶",
+    'ar': "🚶 ادفع ✅ / ☑️ إلى <b> تشغيل / إيقاف </b> لدعوة المستخدمين تلقائيًا إلى مجموعتك \n\n👉🏼 دعوة <u>{0}</u> مستخدمين يوميًا من المجموعة {1}",
+}
+l_cmember_on = {
+    'ru': "👁️‍🗨️ Готово! Текущее количество <b>авто-просмотров</b> на последний пост канала установлено в значение <u>{0}</u>",
+    'en': "👁️‍🗨️ Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
+    'es': "👁️‍🗨️ Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
+    'fr': "👁️‍🗨️ Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
+    'zh': "👁️‍🗨️ 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
+    'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
+}
+l_cmember_off = {
+    'ru': "👁️‍🗨️ Режим /view-авто-просмотров отключен",
+    'en': "👁️‍🗨️ Ready! Current primary delay for <u>new</u> users (before writing their <u>1</u>st message) is <u>{0}</u> min",
+    'es': "👁️‍🗨️ Listo! El retraso principal actual para los <u>nuevos</u> usuarios (antes de escribir su <u>1</u>er mensaje) es <u>{0}</u> min",
+    'fr': "👁️‍🗨️ Prêt! Le délai principal actuel pour les <u>nouveaux</u> utilisateurs (avant d'écrire leur <u>1</u>er message) est de <u>{0}</u> min",
+    'zh': "👁️‍🗨️ 準備好了！<u>新</u>用戶的當前主要延遲（在寫他們的<u>1</u>st消息之前）是<u>{0}</u>分鐘",
+    'ar': "👥 جاهز! التأخير الأساسي الحالي لمستخدمي <u> الجدد </u> (قبل كتابة رسالتهم <u> 1 </u> st) هو <u>{0}</u> min",
+}
+l_cmember_parse = {
+    'ru': "👥 Готово! Собрано реальных участников: <u>{0}</u>\n\n👩🏽‍💻 Остальные подписчики будут постепенно пополнять базу, пока у @{1}-бота есть права [✅ Назначение администраторов]\n\n{2}",
+    'en': "👥 Ready! Gathered members: <u>{0}</u>. You can immediately make an <b>sending</b> or <b>inviting</b> to channel by received members{1}",
+    'es': "👥 Listo! Miembros reunidos: <u>{0}</u>. Inmediatamente puede hacer un <b>envío</b> o <b>invitación</b> al grupo por miembros recibidos{1}",
+    'fr': "👥 Prêt ! Membres réunis : <u>{0}</u>. Vous pouvez immédiatement faire un <b>envoi</b> ou <b>inviter</b> pour channeler par membres reçus{1}",
+    'zh': "👥 準備好了！ 聚集成員：<u>{0}</u>。 您可以立即<b>發送</b>或<b>邀請</b>按收到的成員分組{1}",
+    'ar': "🔥 جاهز! الأعضاء الذين تم تجميعهم: <u>{0}</u>. يمكنك على الفور إجراء <b> إرسال </b> أو <b> دعوة </b> للانضمام إلى المجموعة بواسطة الأعضاء المستلمين {1}",
+}
+# endregion
+# endregion
+
```

### Comparing `yeref-0.1.46/yeref/yeref.py` & `yeref-0.1.47/yeref/yeref.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,27 +51,25 @@
     '6090677494',
 
     '5754810063',
     '5491025132',
     '5360564451',
     '6281795468',
 ]
-old_tid = 4_000_000_000
+old_tid = 5_000_000_000
 lat_company = 59.395881
 long_company = 24.658980
 lkjhgfdsa_channel_id = -1001657854832
 lkjhgfdsa_channel_un = "lkjhgfdsa_channel"
 tg_ch_ads_un = 'kiejakn3_djdjn4m_ads'
 tg_ch_ads_id = -1001921910898
 price_one = 200
 price_all = 500
 
 TGPH_TOKEN_MAIN = 'a9335172886eae62ec0743bf8a4e195286ec30cff067da5fd1db2899d008'
-TGPH_TOKEN_BROADCAST = 'b348a7a3964bbb4df2b66f8dbcd142e9dbf22ce58478a96bab3761dba51c'
-pp = 'https://telegra.ph/broadcasting-04-22'
 SECTION = 'CONFIG'
 LINES_ON_PAGE = 5
 short_name = 'me'
 const_url = 'https://t.me/'
 phone_number = '79999999999'
 vk_group = 'https://vk.com'
 vk_account = 'https://vk.com'
@@ -546,52 +544,56 @@
         show_offers_off = yeref.l_off[lz]
 
         extra = f"\n\n{show_offers_datetime}: {OFFER_DT if OFFER_DT else show_offers_off}\n" \
                 f"{show_offers_button}: {OFFER_BUTTON if OFFER_BUTTON else show_offers_off}\n"
         OFFER_TEXT = OFFER_TEXT or ''
         OFFER_TEXT = '' if OFFER_MEDIATYPE == 'video_note' or OFFER_MEDIATYPE == 'sticker' else OFFER_TEXT
         moment = 1020 - len(OFFER_TEXT) - len(extra)
-        OFFER_TEXT = await correct_tag(f"{yeref.l_post_text[0:(len(OFFER_TEXT) + moment)]}") if moment <= 0 else OFFER_TEXT
+        OFFER_TEXT = await correct_tag(
+            f"{yeref.l_post_text[0:(len(OFFER_TEXT) + moment)]}") if moment <= 0 else OFFER_TEXT
 
         # endregion
         # region reply_markup
         reply_markup = get_keyboard_admin(data_offers, 'offers', post_id)
 
         buttons = [
             types.InlineKeyboardButton(text=f"✅ {yeref.l_btn[lz]}" if OFFER_ISBUTTON else f"☑️ {yeref.l_btn[lz]}",
                                        callback_data=f'ofr_isbtn_{OFFER_ID}_{post_id}'),
             types.InlineKeyboardButton(text=f"✅ {yeref.l_pin[lz]}" if OFFER_ISPIN else f"☑️ {yeref.l_pin[lz]}",
                                        callback_data=f'ofr_ispin_{OFFER_ID}_{post_id}'),
-            types.InlineKeyboardButton(text=f"✅ {yeref.l_silence[lz]}" if OFFER_ISSILENCE else f"☑️ {yeref.l_silence[lz]}",
-                                       callback_data=f'ofr_issilence_{OFFER_ID}_{post_id}'),
+            types.InlineKeyboardButton(
+                text=f"✅ {yeref.l_silence[lz]}" if OFFER_ISSILENCE else f"☑️ {yeref.l_silence[lz]}",
+                callback_data=f'ofr_issilence_{OFFER_ID}_{post_id}'),
         ]
         reply_markup.row(*buttons)
 
         buttons = [
-            types.InlineKeyboardButton(text=f"✅ {yeref.l_gallery[lz]}" if OFFER_ISGALLERY else f"☑️ {yeref.l_gallery[lz]}",
-                                       callback_data=f'ofr_isgallery_{OFFER_ID}_{post_id}'),
+            types.InlineKeyboardButton(
+                text=f"✅ {yeref.l_gallery[lz]}" if OFFER_ISGALLERY else f"☑️ {yeref.l_gallery[lz]}",
+                callback_data=f'ofr_isgallery_{OFFER_ID}_{post_id}'),
             types.InlineKeyboardButton(text=f"✅ {yeref.l_preview[lz]}" if OFFER_ISTGPH else f"☑️ {yeref.l_preview[lz]}",
                                        callback_data=f'ofr_ispreview_{OFFER_ID}_{post_id}'),
-            types.InlineKeyboardButton(text=f"✅ {yeref.l_spoiler[lz]}" if OFFER_ISSPOILER else f"☑️ {yeref.l_spoiler[lz]}",
-                                       callback_data=f'ofr_isspoiler_{OFFER_ID}_{post_id}'),
+            types.InlineKeyboardButton(
+                text=f"✅ {yeref.l_spoiler[lz]}" if OFFER_ISSPOILER else f"☑️ {yeref.l_spoiler[lz]}",
+                callback_data=f'ofr_isspoiler_{OFFER_ID}_{post_id}'),
         ]
         reply_markup.row(*buttons)
 
         buttons = [
             types.InlineKeyboardButton(text=yeref.l_post_new[lz],
                                        callback_data=f'ofr_new_{OFFER_ID}_{post_id}'),
             types.InlineKeyboardButton(text=yeref.l_post_delete[lz],
                                        callback_data=f'ofr_del_{OFFER_ID}_{post_id}'),
             types.InlineKeyboardButton(text=yeref.l_post_change[lz],
                                        callback_data=f'ofr_edit_{OFFER_ID}_{post_id}'),
         ]
         reply_markup.row(*buttons)
 
         reply_markup.row(types.InlineKeyboardButton(text=yeref.l_post_publish[lz],
-                                                    callback_data=f'ofr_pub_{OFFER_ID}_{post_id}'))
+                                                    callback_data=f'ofr_publication_{OFFER_ID}_{post_id}'))
 
         # endregion
         # region show
         if OFFER_FILEID and '[' not in OFFER_FILEID:
             OFFER_TEXT = OFFER_TEXT + extra
             if not call:
                 if OFFER_MEDIATYPE == 'photo' or OFFER_MEDIATYPE == 'text':
@@ -612,24 +614,24 @@
                                             reply_markup=reply_markup.as_markup())
                 elif OFFER_MEDIATYPE == 'sticker':
                     await bot.send_sticker(chat_id=chat_id, sticker=OFFER_FILEID)
                     await bot.send_message(chat_id, OFFER_TEXT, reply_markup=reply_markup.as_markup(),
                                            disable_web_page_preview=True)
                 elif OFFER_MEDIATYPE == 'voice':
                     if has_restricted:
-                        text = yeref.offer_has_restricted[lz].format(bot_un)
+                        text = yeref.l_post_has_restricted[lz].format(bot_un)
                         await bot.send_message(chat_id, text, disable_web_page_preview=True)
                         await bot.send_message(chat_id, OFFER_TEXT, reply_markup=reply_markup.as_markup(),
                                                disable_web_page_preview=True)
                     else:
                         await bot.send_voice(chat_id, OFFER_FILEID, caption=OFFER_TEXT,
                                              reply_markup=reply_markup.as_markup())
                 elif OFFER_MEDIATYPE == 'video_note':
                     if has_restricted:
-                        text = yeref.offer_has_restricted[lz].format(bot_un)
+                        text = yeref.l_post_has_restricted[lz].format(bot_un)
                         await bot.send_message(chat_id, text, disable_web_page_preview=True)
                     else:
                         await bot.send_video_note(chat_id=chat_id, video_note=OFFER_FILEID)
                     await bot.send_message(chat_id, OFFER_TEXT, reply_markup=reply_markup.as_markup(),
                                            disable_web_page_preview=True)
             else:
                 if OFFER_MEDIATYPE == 'photo' or OFFER_MEDIATYPE == 'text':
@@ -674,23 +676,23 @@
                         await call.message.edit_media(media=media, reply_markup=reply_markup.as_markup())
                 elif OFFER_MEDIATYPE == 'sticker':
                     await bot.send_sticker(chat_id, OFFER_FILEID)
                     await bot.send_message(chat_id=chat_id, text=OFFER_TEXT, reply_markup=reply_markup.as_markup(),
                                            disable_web_page_preview=True)
                 elif OFFER_MEDIATYPE == 'video_note':
                     if has_restricted:
-                        text = yeref.offer_has_restricted[lz].format(bot_un)
+                        text = yeref.l_post_has_restricted[lz].format(bot_un)
                         await bot.send_message(chat_id, text, disable_web_page_preview=True)
                     else:
                         await bot.send_video_note(chat_id=chat_id, video_note=OFFER_FILEID)
                     await bot.send_message(chat_id, OFFER_TEXT, reply_markup=reply_markup.as_markup(),
                                            disable_web_page_preview=True)
                 elif OFFER_MEDIATYPE == 'voice':
                     if has_restricted:
-                        text = yeref.offer_has_restricted[lz].format(bot_un)
+                        text = yeref.l_post_has_restricted[lz].format(bot_un)
                         await bot.send_message(chat_id, text, disable_web_page_preview=True)
                         await bot.send_message(chat_id, OFFER_TEXT, reply_markup=reply_markup.as_markup(),
                                                disable_web_page_preview=True)
                     else:
                         await bot.send_voice(chat_id, OFFER_FILEID, caption=OFFER_TEXT,
                                              reply_markup=reply_markup.as_markup())
         else:
@@ -829,17 +831,18 @@
         if OFFER_ISTGPH and OFFER_TGPHLINK and '[' not in OFFER_TGPHLINK:
             OFFER_MEDIATYPE = 'text'
             OFFER_TEXT = OFFER_TEXT if OFFER_TEXT and OFFER_TEXT != '' else "."
             OFFER_TEXT = f"<a href='{OFFER_TGPHLINK}'>​</a>{OFFER_TEXT}"
 
             if OFFER_ISGALLERY:
                 buttons = [
-                    types.InlineKeyboardButton(text="←", callback_data=f'gallery_prev_{offer_id}'),
-                    types.InlineKeyboardButton(text=f"{current}/{len_}", callback_data=f'gallery_current_{offer_id}'),
-                    types.InlineKeyboardButton(text="→", callback_data=f'gallery_next_{offer_id}'),
+                    types.InlineKeyboardButton(text="←", callback_data=f'gallery_prev_{offer_id}_{current}_{len_}'),
+                    types.InlineKeyboardButton(text=f"{current}/{len_}",
+                                               callback_data=f'gallery_current_{offer_id}_{current}_{len_}'),
+                    types.InlineKeyboardButton(text="→", callback_data=f'gallery_next_{offer_id}_{current}_{len_}'),
                 ]
                 reply_markup.row(*buttons)
 
         if '[' in OFFER_MEDIATYPE and not message_id:
             media = []
             for i in range(0, len(OFFER_FILEID)):
                 caption = OFFER_TEXT if i == 0 else None
@@ -929,15 +932,17 @@
                                                    reply_markup=reply_markup.as_markup())
         elif OFFER_MEDIATYPE == 'sticker':
             result = await bot.send_sticker(chat_id=chat_id,
                                             sticker=OFFER_FILEID,
                                             disable_notification=OFFER_ISSILENCE,
                                             reply_markup=reply_markup.as_markup())
 
-        if result and OFFER_ISPIN and not message_id:
+        if result and OFFER_ISPIN and not message_id and isinstance(result, list):
+            await bot.pin_chat_message(chat_id=chat_id, message_id=result[0].message_id, disable_notification=False)
+        elif result and OFFER_ISPIN and not message_id:
             await bot.pin_chat_message(chat_id=chat_id, message_id=result.message_id, disable_notification=False)
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
@@ -1036,15 +1041,16 @@
             await bot.send_message(call.from_user.id, yeref.l_post_text[lz], reply_markup=markupAdmin)
         elif cmd == 'del':
             await state.clear()
 
             sql = "DELETE FROM OFFER WHERE OFFER_ID=?"
             await db_change(sql, (offer_id,), BASE_D)
 
-            await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id - 1, call)
+            await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id - 1,
+                                    call)
         elif cmd == 'edit':
             await state.clear()
 
             await state.set_state(FsmOffer.text)
             await state.update_data(offer_id=offer_id)
 
             await bot.send_message(call.from_user.id, yeref.l_post_edit[lz], reply_markup=markupAdmin)
@@ -1053,15 +1059,16 @@
             data = await db_select(sql, (offer_id,), BASE_D)
             OFFER_BUTTON, OFFER_ISBUTTON = data[0]
 
             if OFFER_BUTTON:
                 OFFER_ISBUTTON = 0 if OFFER_ISBUTTON else 1
                 sql = "UPDATE OFFER SET OFFER_ISBUTTON=? WHERE OFFER_ID=?"
                 await db_change(sql, (OFFER_ISBUTTON, offer_id,), BASE_D)
-                await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id, call)
+                await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id,
+                                        call)
             else:
                 text = yeref.l_buttons_text[lz]
                 await call.answer(text=text, show_alert=True)
         elif cmd == 'ispin':
             sql = "SELECT OFFER_ISPIN FROM OFFER WHERE OFFER_ID=?"
             data = await db_select(sql, (offer_id,), BASE_D)
             OFFER_ISPIN = 0 if data[0][0] else 1
@@ -1080,15 +1087,16 @@
             data = await db_select(sql, (offer_id,), BASE_D)
             OFFER_ISGALLERY, OFFER_FILEID = data[0]
 
             if OFFER_FILEID and '[' in OFFER_FILEID:
                 OFFER_ISGALLERY = 0 if data[0][0] else 1
                 sql = "UPDATE OFFER SET OFFER_ISGALLERY=? WHERE OFFER_ID=?"
                 await db_change(sql, (OFFER_ISGALLERY, offer_id,), BASE_D)
-                await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id, call)
+                await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id,
+                                        call)
             else:
                 text = yeref.l_gallery_text[lz]
                 await call.answer(text=text, show_alert=True)
         elif cmd == 'ispreview':
             sql = "SELECT OFFER_ISTGPH, OFFER_TGPHLINK FROM OFFER WHERE OFFER_ID=?"
             data = await db_select(sql, (offer_id,), BASE_D)
             OFFER_ISTGPH, OFFER_TGPHLINK = data[0]
@@ -1106,41 +1114,42 @@
             data = await db_select(sql, (offer_id,), BASE_D)
             OFFER_ISSPOILER, OFFER_MEDIATYPE = data[0]
 
             if OFFER_MEDIATYPE and OFFER_MEDIATYPE in ['photo', 'animation', 'video'] or '[' in OFFER_MEDIATYPE:
                 OFFER_ISSPOILER = 0 if data[0][0] else 1
                 sql = "UPDATE OFFER SET OFFER_ISSPOILER=? WHERE OFFER_ID=?"
                 await db_change(sql, (OFFER_ISSPOILER, offer_id,), BASE_D)
-                await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id, call)
+                await show_offers_admin(bot, FsmOffer, chat_id, lz, state, has_restricted, BASE_D, bot_un, post_id,
+                                        call)
             else:
                 text = yeref.l_spoiler_text[lz]
                 await call.answer(text=text, show_alert=True)
         elif cmd == 'pub':
             await state.clear()
             await call.answer()
 
             reply_markup = InlineKeyboardBuilder()
             buttons = [
-                types.InlineKeyboardButton(text=yeref.l_me[lz], callback_data=f"pub_me_{offer_id}"),
-                types.InlineKeyboardButton(text=yeref.l_all[lz], callback_data=f"pub_all_{offer_id}"),
-                types.InlineKeyboardButton(text=yeref.l_ids[lz], callback_data=f"pub_ids_{offer_id}"),
+                types.InlineKeyboardButton(text=yeref.l_me[lz], callback_data=f"publication_me_{offer_id}"),
+                types.InlineKeyboardButton(text=yeref.l_all[lz], callback_data=f"publication_all_{offer_id}"),
+                types.InlineKeyboardButton(text=yeref.l_ids[lz], callback_data=f"publication_ids_{offer_id}"),
             ]
             reply_markup.add(*buttons).adjust(1)
 
             text = yeref.l_recipient[lz]
             await bot.send_message(chat_id, text, reply_markup=reply_markup.as_markup())
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
-async def callbacks_pub_admin(bot, FsmIds, call, state, BASE_D):
+async def callbacks_publication_admin(bot, FsmIds, call, state, BASE_D):
     try:
         chat_id = call.from_user.id
         lz = await lz_code(chat_id, call.from_user.language_code, BASE_D)
         data, option, offer_id = call.data.split('_')
 
         if option == 'me':
             loop = asyncio.get_event_loop()
@@ -1158,15 +1167,15 @@
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
-async def fsm_ids_start_admin(bot, FsmIds, message, state, BASE_D):
+async def fsm_ids_start_admin(bot, message, state, BASE_D):
     try:
         chat_id = message.from_user.id
         lz = await lz_code(chat_id, message.from_user.language_code, BASE_D)
         arr = re.split(r'[`\-=~!@#$%^&*()_+\[\]{};\'\\:"|<,./?]', message.text)
         ids = [it for it in arr if it != '']
         data = await state.get_data()
         offer_id = data.get('offer_id')
@@ -1609,20 +1618,20 @@
             datetime_current = dt_cur.strftime("%H:%M")
 
             try:
                 arr = text.strip().split(':')
                 dt_user_new = datetime.datetime(year=int(year_), month=int(month_), day=int(day_), hour=int(arr[0]),
                                                 minute=int(arr[1]))
                 if dt_user_new < dt_cur:
-                    await message.answer(text=yeref.offer_time_future[lz])
+                    await message.answer(text=yeref.l_post_time_future[lz])
                     return
             except Exception as e:
                 logger.info(log_ % str(e))
                 text = yeref.l_generate_calendar_time[lz].format(dt_user.strftime("%d-%m-%Y"), datetime_plus,
-                                                         datetime_current, USER_TZ)
+                                                                 datetime_current, USER_TZ)
                 await bot.send_message(chat_id, text)
                 return
 
             offer_dt = dt_user_new.strftime('%d-%m-%Y %H:%M')
             await state.update_data(offer_dt=offer_dt)
 
             await bot.send_message(chat_id, yeref.l_post_finish[lz])
@@ -1723,96 +1732,55 @@
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
-async def get_current_index(offer_id, inline_keyboard):
-    current = length = None
-    try:
-        for item in inline_keyboard:
-            if isinstance(item, list):
-                for it in item:
-                    if it.callback_data == f"gallery_current_{offer_id}" and '/' in it.text:
-                        current = await parse_index(it.text.split('/')[0])
-                        length = await parse_index(it.text.split('/')[1])
-                        return
-            elif item.callback_data == f"gallery_current_{offer_id}" and '/' in item.text:
-                current = await parse_index(item.text.split('/')[0])
-                length = await parse_index(item.text.split('/')[1])
-                return
-    except TelegramRetryAfter as e:
-        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(0, 1), 2))
-    finally:
-        return current, length
-
-
-async def parse_index(str_num):
-    result = None
-    try:
-        res = ''
-        for item in str_num:
-            if item in '0123456789':
-                res = f"{res}{item}"
-        result = int(res) if res != '' else None
-    except TelegramRetryAfter as e:
-        logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
-        await asyncio.sleep(e.retry_after + 1)
-    except Exception as e:
-        logger.info(log_ % str(e))
-        await asyncio.sleep(round(random.uniform(0, 1), 2))
-    finally:
-        return result
-
-
 async def gallery_handler_admin(bot, call, state, BASE_D):
     try:
         await state.clear()
         chat_id = call.from_user.id
         message_id = call.message.message_id
-        data, option, offer_id = call.data.split('_')
+        data, option, offer_id, current, len_ = call.data.split("_")
+        offer_id = int(offer_id)
+        current = int(current)
+        len_ = int(len_)
 
         if option == 'prev':
-            current, length = await get_current_index(offer_id, call.message.reply_markup.inline_keyboard)
-            if current is None or length is None: await call.answer(); return
-            current = length if current == 1 and option == 'prev' else current - 1
+            current = len_ if current == 1 and option == 'prev' else current - 1
             await send_user(bot, chat_id, offer_id, BASE_D, message_id, current)
         elif option == 'next':
-            current, length = await get_current_index(offer_id, call.message.reply_markup.inline_keyboard)
-            if current is None or length is None: await call.answer(); return
-            current = 1 if current == length and option == 'next' else current + 1
+            current = 1 if current == len_ and option == 'next' else current + 1
             await send_user(bot, chat_id, offer_id, BASE_D, message_id, current)
         elif data[1] == 'current':
             pass
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
-async def edit_inline_admin(bot, post_id, inline_message_id, current, len_, BASE_D):
+async def edit_inline(bot, post_id, inline_message_id, current, BASE_D):
     result = None
     try:
         sql = "SELECT POST_TEXT, POST_MEDIATYPE, POST_FILEID, POST_FILEIDNOTE, POST_BUTTON, POST_ISBUTTON, " \
               "POST_TGPHLINK, POST_ISTGPH, POST_ISGALLERY, POST_ISSPOILER FROM POST WHERE POST_ID=?"
         data_posts = await db_select(sql, (post_id,), BASE_D)
         if not len(data_posts): return
         item = data_posts[0]
         POST_TEXT, POST_MEDIATYPE, POST_FILEID, POST_FILEIDNOTE, POST_BUTTON, POST_ISBUTTON, POST_TGPHLINK, \
             POST_ISTGPH, POST_ISGALLERY, POST_ISSPOILER = item
 
+        len_ = 0
         POST_TEXT = POST_TEXT if POST_TEXT else ''
-        reply_markup = await create_replymarkup2(bot, post_id, POST_BUTTON) if POST_ISBUTTON else InlineKeyboardBuilder()
+        reply_markup = await create_replymarkup2(bot, post_id,
+                                                 POST_BUTTON) if POST_ISBUTTON else InlineKeyboardBuilder()
 
         if '[' in POST_MEDIATYPE:
             POST_FILEID = ast.literal_eval(POST_FILEID)
             POST_MEDIATYPE = ast.literal_eval(POST_MEDIATYPE)
             POST_TGPHLINK = ast.literal_eval(POST_TGPHLINK)
 
             len_ = len(POST_FILEID)
@@ -1824,50 +1792,161 @@
             POST_MEDIATYPE = 'text'
             POST_TEXT = POST_TEXT if POST_TEXT and POST_TEXT != '' else "."
             POST_TEXT = f"<a href='{POST_TGPHLINK}'>​</a>{POST_TEXT}"
 
         if POST_ISGALLERY:
             buttons = [
                 types.InlineKeyboardButton(text="←", callback_data=f'gal_prev_{post_id}_{current}_{len_}'),
-                types.InlineKeyboardButton(text=f"{current}/{len_}", callback_data=f'gal_current_{post_id}_{current}_{len_}'),
+                types.InlineKeyboardButton(text=f"{current}/{len_}",
+                                           callback_data=f'gal_current_{post_id}_{current}_{len_}'),
                 types.InlineKeyboardButton(text="→", callback_data=f'gal_next_{post_id}_{current}_{len_}'),
             ]
             reply_markup.row(*buttons)
 
         if POST_MEDIATYPE == 'text':
-            await bot.edit_message_text(inline_message_id=inline_message_id, text=POST_TEXT, reply_markup=reply_markup.as_markup())
+            await bot.edit_message_text(inline_message_id=inline_message_id, text=POST_TEXT,
+                                        reply_markup=reply_markup.as_markup())
         elif POST_MEDIATYPE == 'photo':
             media = types.InputMediaPhoto(media=POST_FILEID, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id, reply_markup=reply_markup.as_markup())
+            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
+                                         reply_markup=reply_markup.as_markup())
         elif POST_MEDIATYPE == 'animation':
             media = types.InputMediaAnimation(media=POST_FILEID, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id, reply_markup=reply_markup.as_markup())
+            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
+                                         reply_markup=reply_markup.as_markup())
         elif POST_MEDIATYPE == 'video':
             media = types.InputMediaVideo(media=POST_FILEID, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id, reply_markup=reply_markup.as_markup())
+            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
+                                         reply_markup=reply_markup.as_markup())
         elif POST_MEDIATYPE == 'video_note':
             media = types.InputMediaVideo(media=POST_FILEIDNOTE, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id, reply_markup=reply_markup.as_markup())
+            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
+                                         reply_markup=reply_markup.as_markup())
         elif POST_MEDIATYPE == 'audio':
             media = types.InputMediaAudio(media=POST_FILEID, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id, reply_markup=reply_markup.as_markup())
+            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
+                                         reply_markup=reply_markup.as_markup())
         elif POST_MEDIATYPE == 'voice':
             media = types.InputMediaAudio(media=POST_FILEIDNOTE, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id, reply_markup=reply_markup.as_markup())
+            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
+                                         reply_markup=reply_markup.as_markup())
         elif POST_MEDIATYPE == 'document':
-            media = types.InputMediaDocument(media=POST_FILEID, caption=POST_TEXT, disable_content_type_detection=True)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id, reply_markup=reply_markup.as_markup())
+            media = types.InputMediaDocument(media=POST_FILEID, caption=POST_TEXT)
+            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
+                                         reply_markup=reply_markup.as_markup())
         else:
             media = types.InputMedia(media=POST_FILEID, caption=POST_TEXT)
-            await bot.edit_message_media(media=media, inline_message_id=inline_message_id, reply_markup=reply_markup.as_markup())
+            await bot.edit_message_media(media=media, inline_message_id=inline_message_id,
+                                         reply_markup=reply_markup.as_markup())
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
+
+
+async def edit_simple(bot, chat_id, post_id, message_id, current, BASE_D):
+    result = None
+    try:
+        sql = "SELECT POST_TEXT, POST_MEDIATYPE, POST_FILEID, POST_FILEIDNOTE, POST_BUTTON, POST_ISBUTTON, " \
+              "POST_TGPHLINK, POST_ISTGPH, POST_ISGALLERY, POST_ISSPOILER FROM POST WHERE POST_ID=?"
+        data_posts = await db_select(sql, (post_id,), BASE_D)
+        if not len(data_posts): return
+        item = data_posts[0]
+        POST_TEXT, POST_MEDIATYPE, POST_FILEID, POST_FILEIDNOTE, POST_BUTTON, POST_ISBUTTON, POST_TGPHLINK, \
+            POST_ISTGPH, POST_ISGALLERY, POST_ISSPOILER = item
+
+        len_ = 0
+        POST_TEXT = POST_TEXT if POST_TEXT else ''
+        reply_markup = await create_replymarkup2(bot, post_id,
+                                                 POST_BUTTON) if POST_ISBUTTON else InlineKeyboardBuilder()
+
+        if '[' in POST_MEDIATYPE and POST_ISGALLERY:
+            POST_FILEID = ast.literal_eval(POST_FILEID)
+            POST_MEDIATYPE = ast.literal_eval(POST_MEDIATYPE)
+            POST_TGPHLINK = ast.literal_eval(POST_TGPHLINK)
+
+            len_ = len(POST_FILEID)
+            POST_FILEID = POST_FILEID[0]
+            POST_MEDIATYPE = POST_MEDIATYPE[0]
+            POST_TGPHLINK = POST_TGPHLINK[0]
+
+        if POST_ISTGPH and POST_TGPHLINK:
+            POST_MEDIATYPE = 'text'
+            POST_TEXT = POST_TEXT if POST_TEXT and POST_TEXT != '' else "."
+            POST_TEXT = f"<a href='{POST_TGPHLINK}'>​</a>{POST_TEXT}"
+
+        if POST_ISGALLERY:
+            buttons = [
+                types.InlineKeyboardButton(text="←", callback_data=f'gal_prev_{post_id}_{current}_{len_}'),
+                types.InlineKeyboardButton(text=f"{current}/{len_}",
+                                           callback_data=f'gal_current_{post_id}_{current}_{len_}'),
+                types.InlineKeyboardButton(text="→", callback_data=f'gal_next_{post_id}_{current}_{len_}'),
+            ]
+            reply_markup.row(*buttons)
+
+        if POST_MEDIATYPE == 'text':
+            await bot.edit_message_text(chat_id=chat_id, message_id=message_id, text=POST_TEXT,
+                                        reply_markup=reply_markup.as_markup())
+        elif POST_MEDIATYPE == 'photo':
+            media = types.InputMediaPhoto(media=POST_FILEID, caption=POST_TEXT, has_spoiler=POST_ISSPOILER)
+            await bot.edit_message_media(media=media, chat_id=chat_id, message_id=message_id,
+
+                                         reply_markup=reply_markup.as_markup())
+        elif POST_MEDIATYPE == 'animation':
+            media = types.InputMediaAnimation(media=POST_FILEID, caption=POST_TEXT, has_spoiler=POST_ISSPOILER)
+            await bot.edit_message_media(media=media, chat_id=chat_id, message_id=message_id,
+                                         reply_markup=reply_markup.as_markup())
+        elif POST_MEDIATYPE == 'video':
+            media = types.InputMediaVideo(media=POST_FILEID, caption=POST_TEXT, has_spoiler=POST_ISSPOILER)
+            await bot.edit_message_media(media=media, chat_id=chat_id, message_id=message_id,
+                                         reply_markup=reply_markup.as_markup())
+        elif POST_MEDIATYPE == 'video_note':
+            media = types.InputMediaVideo(media=POST_FILEIDNOTE, caption=POST_TEXT)
+            await bot.edit_message_media(media=media, chat_id=chat_id, message_id=message_id,
+                                         reply_markup=reply_markup.as_markup())
+        elif POST_MEDIATYPE == 'audio':
+            media = types.InputMediaAudio(media=POST_FILEID, caption=POST_TEXT)
+            await bot.edit_message_media(media=media, chat_id=chat_id, message_id=message_id,
+                                         reply_markup=reply_markup.as_markup())
+        elif POST_MEDIATYPE == 'voice':
+            media = types.InputMediaAudio(media=POST_FILEIDNOTE, caption=POST_TEXT)
+            await bot.edit_message_media(media=media, chat_id=chat_id, message_id=message_id,
+                                         reply_markup=reply_markup.as_markup())
+        elif POST_MEDIATYPE == 'document':
+            media = types.InputMediaDocument(media=POST_FILEID, caption=POST_TEXT)
+            await bot.edit_message_media(media=media, chat_id=chat_id, message_id=message_id,
+                                         reply_markup=reply_markup.as_markup())
+        else:
+            OFFER_FILEID = ast.literal_eval(POST_FILEID) if POST_FILEID and '[' in POST_FILEID else POST_FILEID
+            OFFER_MEDIATYPE = ast.literal_eval(POST_MEDIATYPE) if POST_MEDIATYPE and '[' in POST_MEDIATYPE else POST_MEDIATYPE
+
+            media = []
+            for i in range(0, len(OFFER_FILEID)):
+                caption = POST_TEXT if i == 0 else None
+
+                if OFFER_MEDIATYPE[i] == 'photo':
+                    media.append(
+                        types.InputMediaPhoto(media=OFFER_FILEID[i], caption=caption, has_spoiler=POST_ISSPOILER))
+                elif OFFER_MEDIATYPE[i] == 'video':
+                    media.append(
+                        types.InputMediaVideo(media=OFFER_FILEID[i], caption=caption, has_spoiler=POST_ISSPOILER))
+                elif OFFER_MEDIATYPE[i] == 'audio':
+                    media.append(types.InputMediaAudio(media=OFFER_FILEID[i], caption=caption))
+                elif OFFER_MEDIATYPE[i] == 'document':
+                    media.append(types.InputMediaDocument(media=OFFER_FILEID[i], caption=caption,
+                                                          disable_content_type_detection=True))
+
+            await bot.send_media_group(chat_id, media)
+    except Exception as e:
+        logger.info(log_ % str(e))
+        await asyncio.sleep(round(random.uniform(1, 2), 2))
+    finally:
+        return result
+
 # endregion
 
 
 # region functions
 async def log_old(txt, LOG_DEFAULT, colour=92):
     try:
         logging.info(f'\033[{colour}m%s\033[0m' % (str(txt)))
@@ -3023,29 +3102,26 @@
         return result
 
 
 # endregion
 
 
 # region pyrogram
-async def get_session(SESSION_TID, SESSION_D, BASE_S, EXTRA_D, CONF_P, is_proxy=True):
+async def get_session(SESSION_TID, SESSION_D, BASE_S, EXTRA_D, CONF_P, is_proxy=False):
     res = proxy = None
     try:
         sql = "SELECT SESSION_NAME, SESSION_APIID, SESSION_APIHASH, SESSION_PHONE FROM SESSION WHERE SESSION_TID = ?"
         data = await db_select(sql, (SESSION_TID,), BASE_S)
         if not len(data): return
         SESSION_NAME, SESSION_APIID, SESSION_APIHASH, SESSION_PHONE = data[0]
 
         if is_proxy:
             proxy = await get_proxy(SESSION_TID, EXTRA_D, CONF_P)
 
         res = Client(name=os.path.join(SESSION_D, SESSION_NAME), api_id=SESSION_APIID, api_hash=SESSION_APIHASH,
-                     device_model='IPhone',
-                     system_version="6.12.0",
-                     app_version="10 P (28)",
                      phone_number=SESSION_PHONE, proxy=proxy)
     finally:
         return res
 
 
 async def is_my_chat(bot, chat_id, link, SESSIONS_D, EXTRA_D, CONF_P, BASE_S, BASE_E, is_history=False):
     result = None
@@ -3062,16 +3138,16 @@
                 link = await correct_link(link)
                 if not link: return
 
                 # process
                 sql = "UPDATE SESSION SET SESSION_STATUS = ? WHERE SESSION_TID = ?"
                 await db_change(sql, (f'isChat', SESSION_TID,), BASE_S)
 
-                async with await get_session(SESSION_TID, SESSIONS_D, EXTRA_D, CONF_P, BASE_S, False) as app:
-                    r = await join_my_chat(bot, app, chat_id, link, SESSION_TID, BASE_S, BASE_E)
+                async with await get_session(SESSION_TID, SESSIONS_D, BASE_S, EXTRA_D, CONF_P, False) as app:
+                    r = await join_my_chat(bot, app, chat_id, link, SESSION_TID, BASE_S)
                     if r is None:
                         logger.info(log_ % f"{link} is None")
                         return
                     txt_ = f"👩🏽‍💻 Администратор закрытой группы не принял заявки на вступление"
                     if r == -1:
                         await bot.send_message(chat_id, txt_)
                         return
@@ -3128,16 +3204,16 @@
                 link = await correct_link(link)
                 if not link: continue
 
                 # process
                 sql = "UPDATE SESSION SET SESSION_STATUS = ? WHERE SESSION_TID = ?"
                 await db_change(sql, (f'isChat', SESSION_TID,), BASE_S)
 
-                async with await get_session(SESSION_TID, SESSIONS_D, EXTRA_D, CONF_P, BASE_S) as app:
-                    r = await join_my_chat(bot, app, chat_id, link, SESSION_TID, BASE_S, BASE_E)
+                async with await get_session(SESSION_TID, SESSIONS_D, BASE_S, EXTRA_D, CONF_P) as app:
+                    r = await join_my_chat(bot, app, chat_id, link, SESSION_TID, BASE_S)
 
                     # get_chat https://t.me/+KO7_fV4aGKZkYTUy
                     if r == -1 or r is None: return
                     r = await app.get_chat(r.id)
                     logger.info(log_ % f"{SESSION_TID} get_chat {r.id}")
 
                     if not (r.type.value in ['group', 'supergroup']):
@@ -3187,15 +3263,15 @@
     except Exception as e:
         await log(e)
         await asyncio.sleep(round(random.uniform(1, 2), 2))
     finally:
         return result
 
 
-async def join_my_chat(bot, app, chat_id, link, SESSION_TID, BASE_S, BASE_E):
+async def join_my_chat(bot, app, chat_id, link, SESSION_TID, BASE_S):
     result = None
     try:
         if 't.me/c/' in str(link):
             try:
                 tmp = link.strip('https://t.me/c/').split('/')[0]
                 peer_channel = await app.resolve_peer(int(f"-100{tmp}"))
                 result = await app.invoke(functions.channels.JoinChannel(channel=peer_channel))
@@ -3225,15 +3301,14 @@
             result = await app.join_chat(link)
         except Exception:
             await bot.send_message(chat_id, f"▪️ Ссылка на чат {link} не валидна (или попробуйте еще раз)")
     except (UsernameInvalid, UsernameNotOccupied, ChannelBanned) as e:
         await log(e)
         await asyncio.sleep(round(random.uniform(1, 2), 2))
         await bot.send_message(chat_id, f"▪️ Ссылка/username на группу {link} не валидна")
-        await delete_invalid_chat(link, BASE_E)
     except BadRequest as e:
         await log(e)
         await asyncio.sleep(round(random.uniform(2, 3), 2))
 
         try:
             result = await app.join_chat(link)
         except Exception:
@@ -3244,19 +3319,19 @@
     finally:
         return result
 
 
 async def leave_my_chat(app, r, link):
     try:
         chat_id = r.id if r and ('t.me/+' in str(link) or 'join_my_chat/' in str(link)) else link
-        like_names_res = is_names(r.title)
-        if not (like_names_res or (r.username and f'ferey' in r.username)):
-            await app.leave_chat(chat_id, True)
-            await asyncio.sleep(round(random.uniform(1, 2), 2))
-            # logger.info(log_ % f"\t{link} leave chat")
+        # like_names_res = is_names(r.title)
+        if r.username and f'ferey' in r.username: return
+
+        await app.leave_chat(chat_id, True)
+        # logger.info(log_ % f"\t{link} leave chat")
     except (FloodWait, SlowmodeWait) as e:
         wait_ = f"Wait: {datetime.datetime.utcfromtimestamp(e.value + 1).strftime('%H:%M:%S')}"
         logger.info(log_ % wait_)
         await asyncio.sleep(e.value + 1)
     except Exception:
         # logger.info(log_ % f"leave_my_chat_error: {link} {str(e)}")
         await asyncio.sleep(round(random.uniform(5, 10), 2))
@@ -3279,16 +3354,16 @@
                 link = await correct_link(link)
                 if not link: continue
 
                 # process
                 sql = "UPDATE SESSION SET SESSION_STATUS = ? WHERE SESSION_TID = ?"
                 await db_change(sql, (f'getChatMembers', SESSION_TID,), BASE_S)
 
-                async with await get_session(SESSION_TID, SESSIONS_D, EXTRA_D, CONF_P, BASE_S) as app:
-                    r = await join_my_chat(bot, app, chat_id, link, SESSION_TID, BASE_S, BASE_E)
+                async with await get_session(SESSION_TID, SESSIONS_D, BASE_S, EXTRA_D, CONF_P) as app:
+                    r = await join_my_chat(bot, app, chat_id, link, SESSION_TID, BASE_S)
 
                     # get members
                     sql = "SELECT SESSION_TID FROM SESSION"
                     data_ = await db_select(sql, (), BASE_S)
                     data_ = [str(item[0]) for item in data_]
                     try:
                         async for member in app.get_chat_members(r.id, filter=enums.ChatMembersFilter.SEARCH):
```

