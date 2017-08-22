# EasyDatePicker
A simple dialog as a date picker

How To Use It :

Step 1.Add it in your root build.gradle at the end of repositories:

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
Step 2. Add the dependency

	dependencies {
	        compile 'com.github.Dkaishu:EasyDatePicker:v1.0.1'
	}
  
Step 3.use it in your project
  
  
      private static String today = new SimpleDateFormat("yyyy年MM月dd日 HH:mm").format(new Date());
      TextView textView = (TextView) findViewById(R.id.textView);
  
      EasyDateTimePickDialog dialog = new EasyDateTimePickDialog(MainActivity.this,today);
      dialog.setCancelText("cancel");
      dialog.setCancelTextColor("#017dcd");
      dialog.setConfirmText("confirm");
      dialog.setConfirmTextColor("#017dcd");
      dialog.show(textView);
      
      Easy !
