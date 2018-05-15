# CustomProgress  [![](https://jitpack.io/v/blackchopper/customprogress.svg)](https://jitpack.io/#blackchopper/customprogress)
CustomProgres is a progress display control, it provides three different styles of progressbar, respectively, linear, circular, arc.[中文文档](https://github.com/blackchopper/CustomProgress/blob/master/README_CHINESE.md)
## Instruction
The use of CustomProgres and the use of ordinary progressbr and not much difference, it is more flexible to use, adding some custom properties.
### Code Sample
LineProgressBar
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
ArcProgress
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
SectorProgress
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
## How to
To get a Git project into your build:
### Step 1. Add the JitPack repository to your build file
Add it in your root build.gradle at the end of repositories.[click here for details](https://github.com/blackchopper/CarouselBanner/blob/master/root_build.gradle.png)

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
### Step 2. Add the dependency
Add it in your application module build.gradle at the end of dependencies where you want to use.   [click here for details](https://github.com/blackchopper/CarouselBanner/blob/master/application_build.gradle.png)
```Java
	dependencies {
	  ...
          compile 'com.github.blackchopper:customprogress:v1.1.0'
	}
```	
<br><br>
![Text Image](https://github.com/blackchopper/CustomProgress/blob/master/customprogress.gif)
<br><br><br>
## Thank you for your browsing
If you have any questions, please join the QQ group. I will do my best to answer it for you. Welcome to star and fork this repository, alse follow me.
<br>
![Image Text](https://github.com/blackchopper/CarouselBanner/blob/master/qq_group.png)
