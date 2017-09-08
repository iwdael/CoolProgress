# CustomProgress
CustomProgress is a display of the Andrews framework, it has a linear, round, fan-shaped.
# How to
To get a Git project into your build:
## Step 1. Add the JitPack repository to your build file
Add it in your root build.gradle at the end of repositories:

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
  
## Step 2. Add the dependency

	dependencies {
	        compile 'com.github.mr-absurd:customprogress:v1.0.1'
	}
