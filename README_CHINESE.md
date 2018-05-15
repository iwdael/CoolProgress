# CustomProgress  [![](https://jitpack.io/v/blackchopper/customprogress.svg)](https://jitpack.io/#blackchopper/customprogress)
CustomProgres是一个进度展示控件，它提供了三种不同风格的progressbar，分别为直线型，圆形，弧形。
## 使用说明
CustomProgres的使用方法和普通的progressbr的使用方法并没有太大区别，它使用更加灵活，增加了一些自定义属性。
### 代码示例
线型进度条
```Java
        <com.blackchopper.customprogress.LineProgressBar

            android:layout_width="match_parent"
            android:layout_height="30dp"
            android:layout_marginTop="30dp"
            app:max="100"
            app:progress="20"
            app:progressDesc="已售"
            app:progressRadius="8dp" />

        <com.blackchopper.customprogress.LineProgressBar
            android:id="@+id/line_progresbar"
            android:layout_width="match_parent"
            android:layout_height="30dp"
            android:layout_marginTop="50dp"
            app:lineborderWidth="2dp"
            app:progressRadius="14dp" />

        <com.blackchopper.customprogress.LineProgressBar
            android:id="@+id/line_progresbar2"
            android:layout_width="120dp"
            android:layout_height="10dp"
            android:layout_marginTop="50dp"
            app:isShowDesc="false"
            app:lineborderWidth="2dp"
            app:progressRadius="4dp" />
```
圆形进度条
```Java
            <com.blackchopper.customprogress.ArcProgress
                android:id="@+id/myProgress"
                android:layout_width="150dp"
                android:layout_height="150dp"
                app:degree="0"
                app:progressStyle="arc" />


            <com.blackchopper.customprogress.ArcProgress
                android:id="@+id/myProgress01"
                android:layout_width="160dp"
                android:layout_height="160dp"
                app:arcprogressColor="#a56b75"
                app:radius="80dp"
                app:tickDensity="3" />
                
            <com.blackchopper.customprogress.ArcProgress
                android:id="@+id/myProgress02"
                android:layout_width="180dp"
                android:layout_height="180dp"
                app:arcCapRound="true"
                app:arcprogressColor="#febf82"
                app:degree="180"
                app:progressStyle="arc"
                app:radius="90dp"
                app:tickDensity="3" />


            <com.blackchopper.customprogress.ArcProgress
                android:id="@+id/myProgress03"
                android:layout_width="170dp"
                android:layout_height="170dp"
                android:layout_toRightOf="@id/myProgress"
                app:arcprogressColor="@color/progressColorGray"
                app:degree="0"
                app:progressStyle="tick"
                app:radius="80dp"
                app:tickDensity="3" />
            
```
弧型进度条
```Java
        <com.blackchopper.customprogress.SectorProgress
            android:id="@+id/sectorProgress"
            android:layout_width="150dp"
            android:layout_height="150dp"
            app:circleWidth="25dp"
            app:lineWidth="2dp" />

        <com.blackchopper.customprogress.SectorProgress
            android:id="@+id/sectorProgress1"
            android:layout_width="150dp"
            android:layout_height="150dp"
            android:layout_marginLeft="10dp"
            app:circleWidth="75dp"
            app:percentTextColor="@android:color/white"
            app:percentTextSize="50sp"
            app:symbolSize="30sp"
            app:underColor="#E0E0E0" />
```





## 如何配置
将本仓库引入你的项目:
### Step 1. 添加JitPack仓库到Build文件
合并以下代码到项目根目录下的build.gradle文件的repositories尾。[点击查看详情](https://github.com/blackchopper/CarouselBanner/blob/master/root_build.gradle.png)

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
### Step 2. 添加依赖
合并以下代码到需要使用的application Module的dependencies尾。[点击查看详情](https://github.com/blackchopper/CarouselBanner/blob/master/application_build.gradle.png)
```Java
	dependencies {
	  ...
          compile 'com.github.blackchopper:customprogress:v1.0.5'
	}
```	
<br><br>
![Text Image](https://github.com/blackchopper/CustomProgress/blob/master/customprogress.gif)
<br><br><br>
## 感谢浏览
如果你有任何疑问，请加入QQ群，我将竭诚为你解答。欢迎Star和Fork本仓库，当然也欢迎你关注我。
<br>
![Image Text](https://github.com/blackchopper/CarouselBanner/blob/master/qq_group.png)
