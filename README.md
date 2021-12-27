# CoolProgress
![](https://img.shields.io/badge/platform-android-orange.svg)
![](https://img.shields.io/badge/language-java-yellow.svg)
![](https://jitpack.io/v/com.iwdael/coolprogress.svg)
![](https://img.shields.io/badge/build-passing-brightgreen.svg)
![](https://img.shields.io/badge/license-apache--2.0-green.svg)
![](https://img.shields.io/badge/api-19+-green.svg)

CoolProgres是一个进度展示控件，它提供了三种不同风格的progressbar，分别为直线型，圆形，弧形。
<br>
![Text Image](https://github.com/iwdael/coolprogress/blob/master/coolprogress.gif)
<br>
## 使用说明
CustomProgres的使用方法和普通的progressbr的使用方法并没有太大区别，它使用更加灵活，增加了一些自定义属性。
### 代码示例
线型进度条
```Java
        <com.iwdael.coolprogress.LineProgressBar

            android:layout_width="match_parent"
            android:layout_height="30dp"
            android:layout_marginTop="30dp"
            app:max="100"
            app:progress="20"
            app:progressDesc="已售"
            app:progressRadius="8dp" />

        <com.iwdael.coolprogress.LineProgressBar
            android:id="@+id/line_progresbar"
            android:layout_width="match_parent"
            android:layout_height="30dp"
            android:layout_marginTop="50dp"
            app:lineborderWidth="2dp"
            app:progressRadius="14dp" />

        <com.iwdael.coolprogress.LineProgressBar
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
            <com.iwdael.coolprogress.ArcProgress
                android:id="@+id/myProgress"
                android:layout_width="150dp"
                android:layout_height="150dp"
                app:degree="0"
                app:progressStyle="arc" />


            <com.iwdael.coolprogress.ArcProgress
                android:id="@+id/myProgress01"
                android:layout_width="160dp"
                android:layout_height="160dp"
                app:arcprogressColor="#a56b75"
                app:radius="80dp"
                app:tickDensity="3" />
                
            <com.iwdael.coolprogress.ArcProgress
                android:id="@+id/myProgress02"
                android:layout_width="180dp"
                android:layout_height="180dp"
                app:arcCapRound="true"
                app:arcprogressColor="#febf82"
                app:degree="180"
                app:progressStyle="arc"
                app:radius="90dp"
                app:tickDensity="3" />


            <com.iwdael.coolprogress.ArcProgress
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
        <com.iwdael.coolprogress.SectorProgress
            android:id="@+id/sectorProgress"
            android:layout_width="150dp"
            android:layout_height="150dp"
            app:circleWidth="25dp"
            app:lineWidth="2dp" />

        <com.iwdael.coolprogress.SectorProgress
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
合并以下代码到项目根目录下的build.gradle文件的repositories尾。

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
### Step 2. 添加依赖
合并以下代码到需要使用的application Module的dependencies尾。
```Java
	dependencies {
	  ...
          compile 'com.iwdael:coolprogress:$version'
	}
```	

<br><br><br>
## 感谢浏览
如果你有任何疑问，请加入QQ群，我将竭诚为你解答。欢迎Star和Fork本仓库，当然也欢迎你关注我。
<br>
![Image Text](https://github.com/iwdael/CarouselBanner/blob/master/qq_group.png)
