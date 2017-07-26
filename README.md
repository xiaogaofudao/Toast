

[![](https://jitpack.io/v/xiaogaofudao/Toast.svg)](https://jitpack.io/#xiaogaofudao/Toast)

# Toast

Toast 一个关闭系统消息通知后依然可以显示的Toast


使用方法和Toast完全一致，如下：

Toast.makeText(MainActivity.this,"我是一个屏蔽通知我也是可以显示的Toast",Toast.LENGTH_SHORT).show();

具体使用如下：
Step 1. Add the JitPack repository to your build file


	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
Step 2. Add the dependency


  	dependencies {
		compile 'com.github.xiaogaofudao:Toast:1.0.0'
	}
  

  
  最后需要注意的是，此Toast非彼Toast，应该使用“import com.gaogeek.toast.Toast”，建议在BaseActivity中如下使用：
  
  
	public void showShortText(String text) {
		Toast.makeText(mActivity, text, Toast.LENGTH_SHORT).show();
	}
