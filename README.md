This project is meant to demonstrate the improper insertion of a carriage return into the korean string resources when processed by aapt2 (the issue is not apparent if aapt2 is disabled). This is an Android Studio generated project with 20 string resources added for Korea (`app/src/main/res/values-ko/strings.xml`). Running `create_and_check_apk` will generate an apk and check the apk's resources for improperly inserted carriage returns. 

Because this is the smallest example that was found which would reproduce the issue, virtually any change to the string resources in `app/src/main/res/values-ko/strings.xml` will fix the problem. With much larger sets of strings that generate the problem, changing the strings will frequently not fix the issue and instead will move the improper carriage return to a different string resource and/or add additional improper carriage returns.


