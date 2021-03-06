Android Live Templates
====================

Live Templates set for Android Studio / Intellij IDEA. 

## Installation

To get template file you can use `wget`:
```
wget https://raw.githubusercontent.com/mrmike/AndroidLiveTemplates/master/Android.xml
```

And then copy `Android.xml` file to one of the locations:

###**Windows:** 
```
<your home directory>\.<product name><version number>\config\templates
```

###**Linux:**
```
~\.<product name><version number>\config\templates
```


###**MacOS:** 
```
~/Library/Preferences/<product name><version number>/templates
```


## Usage

During code editing type one of the template name and press tab.

### Templates list

* ld - Send a DEBUG log message.
```
Log.d("$TAG$", "$MSG$");
```
* le - Send a ERROR log message.
```
Log.e("$TAG$", "$MSG$");
```
* li - Send a INFO log message.
```
Log.i("$TAG$", "$MSG$");
```
* lw - Send a WARN log message.
```
Log.w("$TAG$", "$MSG$");
```
* lv - Send a VERBOSE log message.
```
Log.v("$TAG$", "$MSG$");
```
* wtf - What a Terrible Failure: Report an exception that should never happen.
```
Log.wtf("$TAG$", "$MSG$");
```

* toast - show toast
```
Toast.makeText($context$, $msg$, Toast.LENGTH_SHORT).show();
```
* profile - measure exceution time
```
final long start = System.currentTimeMillis();
$END$
Log.d("profiling", "[$methodName$]:" + (System.currentTimeMillis() - start));
```
* view (**ButterKnife**) - inject view
```
@InjectView(R.id.$VIEW$)
$TYPE$ $NAME$
```
* click (**ButterKnife**) - add OnClickListener
```
@OnClick(R.id.$VIEW$)
void on$NAME$Click() {
    $END$
}
```
* android - Add android namespace (**XML**)
```
xmlns:android="http://schemas.android.com/apk/res/android"
```
* tools - Add tools namespace (**XML**)
```
xmlns:tools="http://schemas.android.com/tools"
```
* ttext - Add tools:text attribute
```
tools:text="$text$"
```

* ps - Create private static final String field.
```
private static final String $NAME$ = "$VALUE$";
```

* pi - Create private static final int field.
```
private static final int $NAME$ = $VALUE$;
```

* pf - Create private static final float field.
```
private static final float $NAME$ = $VALUE$;
```

* pd - Create private static final double field.
```
private static final double $NAME$ = $VALUE$;
```