StatusShare-Android
==================
This application allows individual users to share text and photo updates with the other users of the service. 

In particular this sample application highlights the following key backend tasks:

* Allow users to sign up and log in
* Create public/private shared data
* Link images to application data
* Connect on the client-side to 3rd party service (Gravatar)


## Set up StatusShare Project

1. Download the [StatusShare](https://github.com/KinveyApps/StatusShare-Android/archive/master.zip) project.
2. Download the [ActionBar Sherlock Library](http://actionbarsherlock.com/)
3. Download the latest Kinvey library (zip) and extract the downloaded zip file, from: http://devcenter.kinvey.com/android/downloads

###Eclipse
1. In Eclipse, go to __File &rarr; Import…__
2. Click __Android &rarr; Existing Android Code into Workspace__
3. __Browse…__ to set __Root Directory__ to the extracted zip from step 1
4. Repeat steps 4 - 7 for the zip from step 2 and 3 as well.
5. In the __Projects__ box, make sure the __HomeActivity__ project check box, the __library__ project from Action Bar Sherlock, and the __library__ project from ViewPagerIndicator are selected. Then click __Finish__.
6. Copy all jars in the **libs/** folder of the Kinvey Android library zip to TestDrive's **libs/** folder on the file system

###Android Studio
1. In Android Studio, go to **File &rarr; New &rarr; Import Project**
2. **Browse** to the extracted zip from step 1, and click **OK**
3. Click **Next** and **Finish**.
4. Repeat Steps 1-3 for ActionBarSherlock, as well as ViewPagerIndicator.
4. **Browse** to the location of your project, and create a new folder called **lib** inside the **app** directory
5. Copy all jars in the **libs/** folder of the Kinvey Android library zip to the **lib/** folder you just created
6. Expand **Gradle Scripts** in the **Project** Window, and select `build.gradle(Module:app)`.
7. Modify `dependencies` section, leaving any existing dependencies in place and replacing the `x.x.x` with the correct version number

```java
dependencies {    
    compile files('lib/google-http-client-1.19.0.jar')
    compile files('lib/google-http-client-android-1.19.0.jar')
    compile files('lib/google-http-client-gson-1.19.0.jar')
    compile files('lib/google-http-client-jackson2-1.19.0.jar')
    compile files('lib/gson-2.1.jar')
    compile files('lib/guava-18.0.jar')
    compile files('lib/jackson-core-2.1.3.jar')
    compile files('lib/kinvey-android-lib-x.x.x.jar')
    compile files('lib/kinvey-java-x.x.x.jar')
}
```
    

8.  Click the **play** button to start a build, if you still see compilation errors ensure the versions are correctly defined in the dependencies list

###Finally, for all IDEs

0. Specify your app.key and app.secret in the property file located at `assets/kinvey.properties` 

##License


Copyright (c) 2014 Kinvey Inc.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except
in compliance with the License. You may obtain a copy of the License at

 http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License
is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. See the License for the specific language governing permissions and limitations under
the License.
