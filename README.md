# refined_i18n_cn
confluence 插件 refined 主题汉化
Refined has built in language support for English, German, French, Spanish, Finnish and Dutch. It is possible to create and include your own translation by following the below steps:

Refined does not officially support including custom translations. When updating Refined, the below steps must be repeated again.

### Translate the properties file

The properties file contains all text introduced by Refined. Download that file, open it in a text editor and replace the English text with your own translation. For example, if you want to create a Swedish translation for Refined, it could look like this:

**Original file**

...

rw.global.save = Save

rw.global.delete = Delete

rw.global.edit = Edit

...

becomes

**Translated file**

...

rw.global.save = \u4fdd\u5b58
rw.global.delete = \u5220\u9664
rw.global.edit = \u7f16\u8f91



When you are done, save the file as "`OriginalTheme_zh_CN.properties`", where `zh` and `CN are locale extensions for chinese..  Make sure the file is saved in UTF-8 format.



### Add the properties file to the plugin jar file



Make sure your properties file and the plugin jar file (refinedwiki-original-theme.x.x.x.jar) is in the same folder. Open up a terminal, go to that folder and type:

```

mkdir -p originaltheme/properties
mv OriginalTheme_xx_XX.properties originaltheme/properties
zip -g refinedwiki-original-theme-x.x.x.jar originaltheme/properties/OriginalTheme_xx_XX.properties
```

**
**

If you are using windows, you could change the file extension from jar to zip, and place the properties file in the correct location using the windows explorer.

### Upload the new plugin file

When you are done, simply upload the modified jar-file to your instance. Don't forget to repeat these steps when updating Refined.

enjoy it ：）
