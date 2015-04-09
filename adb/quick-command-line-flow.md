1. adb devices  
2. adb shell (if you only have one device connected)  
3. pm list packages -3   
4. pm path | grep (whatever you want to search for)  
5. adb pull /data/app/com.twitter.android-2/base.apk (if you searched for twitter and got that path from the above) 
6. Go download (http://ibotpeaches.github.io/Apktool/) ... you'll need it next! If you're a hipster on a Mac like Dave, you can just 'brew install apktool'  
7. apktool decode base.apk
