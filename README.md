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
2. Download [ActionBarSherlock](http://actionbarsherlock.com/) and in Eclipse, go `File` -> `New` -> `Android Project from Existing Source` and navigate to the ActionBarSherlock directory, and import it as a library project.
3. [Download Kinvey's Android Library](http://devcenter.kinvey.com/android/downloads) and get your app-key and app-secret from the Kinvey console, by signing up and then creating a new app.
4. In Eclipse, go to __File &rarr; Import…__
5. Click __Android &rarr; Existing Android Code into Workspace__
6. __Browse…__ to set __Root Directory__ to the extracted zip from step 1
7. In the __Projects__ box, make sure the __HomeActivity__ project check box ais selected. Then click __Finish__.
8. Right click on the newly created project, and select __Properties__, then select __Android__ on the left.  At the bottom of the window, under the __Library__ section add `ActionBarSherlock` as a dependency. 
9. Copy and paste the Kinvey Jars downloaded in step 3 into the /libs/ directory of the StatusShare project
10. Specify your app.key and app.secret in the property file located at `assets/kinvey.properties` 

##License


Copyright (c) 2014 Kinvey Inc.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except
in compliance with the License. You may obtain a copy of the License at

 http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License
is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. See the License for the specific language governing permissions and limitations under
the License.
