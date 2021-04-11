# adb-hacks-to-remove-android-bloatware
Remove bloatware from your android device using power of adb.


1. Connect your phone
Connect your android device and run the following command to see if it's properly connected or not. If it's not then you might need to enable Developer Option in your phone or install some drivers on your system. <br>
`adb devices`
2. List the packages installed on your phone (Skip if you already know the package name)<br>
`adb shell pm list packages`<br>
3. To Uninstall the package<br>
`adb shell pm uninstall -k --user 0 <package_name>`<br>
Example: `adb shell pm uninstall -k --user 0 com.google.android.youtube`<br>
4. To ReInstall a package (if you need your app again)<br>
`adb shell cmd package install-existing <package_name>`<br>
Example: `adb shell cmd package install-existing com.google.android.youtube`<br>

Here is the list of [bloatware](https://github.com/iamtalhaasghar/adb-hacks-to-remove-android-bloatware/blob/master/uninstalled_packages.csv) i have removed from my phone. Use at your own risk. Your phone might stop working properly.

| Package                                          |  App Name                      |  Alternative FOSS solution (Downloadable from https://f-droid.org)                 |
| ------------------------------------------------ | ------------------------------ | ---------------------------------------------------------------------------------- |
| com.google.android.projection.gearhead           | android auto                   |                                                                                    |
| com.samsung.android.aremoji                      | AR Emoji                       |                                                                                    |
| com.samsung.android.app.spage                    | bixby home                     |                                                                                    |
| com.samsung.android.bixby.service                | bixby service                  |                                                                                    |
| com.samsung.android.app.settings.bixby           | bixby settings                 |                                                                                    |
| com.samsung.android.mdecservice                  | call and text on other devices |                                                                                    |
| com.sec.android.app.chromecustomizations         | Chrome Customizations          |                                                                                    |
| com.samsung.android.da.daagent                   | Dual Messenger                 |                                                                                    |
| com.samsung.android.emojiupdater                 | Emjoi Updater                  |                                                                                    |
| com.sec.android.mimage.avatarstickers            | Emoji Stickers                 |                                                                                    |
| com.facebook.appmanager                          | facebook                       |                                                                                    |
| com.facebook.katana                              | facebook                       |                                                                                    |
| com.facebook.services                            | facebook                       |                                                                                    |
| com.facebook.system                              | facebook                       |                                                                                    |
| com.sec.android.widgetapp.easymodecontactswidget | Favorite Contacts Widget       |                                                                                    |
| flipboard.boxer.app                              | flipboard                      |                                                                                    |
| com.sec.android.widgetapp.samsungapps            | Galaxy Essentials Widget       |                                                                                    |
| com.sec.android.app.samsungapps                  | Galaxy Store                   |                                                                                    |
| com.samsung.android.game.gametools               | Game Booster                   |                                                                                    |
| com.samsung.android.game.gamehome                | Game Home                      |                                                                                    |
| com.google.android.gm                            | gmail                          | [K-9 Mail](https://f-droid.org/en/packages/com.fsck.k9)                            |
| com.google.android.syncadapters.calendar         | google calendar sync           |                                                                                    |
| com.android.chrome                               | google chrome                  |                                                                                    |
| com.google.android.syncadapters.contacts         | google contacts sync           |                                                                                    |
| com.google.android.gms.location.history          | Google Location History        |                                                                                    |
| com.google.android.apps.maps                     | google maps                    |                                                                                    |
| com.google.android.tts                           | Google Text to Speech          |                                                                                    |
| com.google.android.googlequicksearchbox          | google voice search            |                                                                                    |
| com.samsung.android.kidsinstaller                | Kids Home Installer            |                                                                                    |
| com.sec.android.app.magnifier                    | magnifier                      |                                                                                    |
| com.samsung.android.mdx.quickboard               | Media and Devices              |                                                                                    |
| com.sec.android.widgetapp.webmanual              | Online Help Manual Widget      |                                                                                    |
| com.samsung.android.drivelink.stub               | Samsung Car Mode Stub          |                                                                                    |
| com.sec.android.app.billing                      | Samsung Checkout               |                                                                                    |
| com.samsung.android.scloud                       | Samsung Cloud                  |                                                                                    |
| com.samsung.storyservice                         | samsung gallery stories        |                                                                                    |
| com.samsung.android.authfw                       | Samsung Pass                   |                                                                                    |
| com.samsung.android.samsungpassautofill          | Samsung Pass Autofill Service  |                                                                                    |
| com.samsung.android.samsungpass                  | Samsung Pass Provider          |                                                                                    |
| com.samsung.knox.securefolder                    | Samsung Secure Folder          |                                                                                    |
| com.samsung.android.smartmirroring               | Samsung Smart View             |                                                                                    |
| com.sec.android.daemonapp                        | samsung weather app            |                                                                                    |
| com.android.stk                                  | Sim Tool Kit (SIM 1)           |                                                                                    |
| com.android.stk2                                 | Sim Tool Kit (SIM 2)           |                                                                                    |
| com.samsung.android.beaconmanager                | Smart Things                   |                                                                                    |
| com.samsung.android.themestore                   | Theme Store                    |                                                                                    |
| com.samsung.android.app.watchmanagerstub         | Wearable Manager Installer     |                                                                                    |
| com.samsung.android.app.social                   | Whats New                      |                                                                                    |
| com.google.android.youtube                       | youtube                        | [New Pipe](https://f-droid.org/en/packages/org.schabi.newpipe)                     |
| com.sec.android.inputmethod                      |  Samsung keyboard              | [Simple Keyboard] (https://f-droid.org/en/packages/rkr.simplekeyboard.inputmethod) |
| com.samsung.android.app.reminder                 | Reminder App                   |                                                                                    |
| com.sec.android.app.myfiles                      | My Files                       |                                                                                    |
| com.sec.android.app.clockpackage                 | Clock                          |                                                                                    |
| com.samsung.android.calendar                     | Calendar                       |                                                                                  
