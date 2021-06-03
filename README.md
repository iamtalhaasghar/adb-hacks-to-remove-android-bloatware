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
