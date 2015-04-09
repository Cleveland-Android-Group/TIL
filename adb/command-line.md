adb
=====================================
adb devices  
adb shell  
adb pull <path> <local_path>  

adb shell
=====================================
pm list packages -3  // the "-3" means third-party packages only!  
pm path <package> (for example pm path com.twitter.android after finding com.twitter.android from the command above)  

android backup extractor
=====================================
abe unpack <backup.ab> <backup.tar>  
apktool decode <pathToApk>


dex2jar  
apktool
