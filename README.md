# Activity-lifecycle-and-state
tasks challenges homework

Activity lifecycle<br/>
<img src="screenshots/activitylifecycle.gif" width="300px" height="600px">
<br/>
Lifecycle Homework<br/>
<img src="screenshots/lifecycle_homework.gif" width="300px" height="600px">
<br/>
<img src="screenshots/lifecycleHomework.png" width="300px" height="600px">
<br/>
layout challenge<br/>
<img src="screenshots/lifecycle_challenge.gif" width="300px" height="600px">
<br/>
Logcat Activity of lifecycle<br/>
<img src="screenshots/logcat.png" width="600px" height="300px">

<b>Question 1</b><br/>
<p>If you run the homework app before implementing onSaveInstanceState(), what happens if you rotate the device?<br/>

-> The counter is reset to 0, but the contents of the EditText is preserved.</p>

<b>Question 2</b><br/>
<p>What Activity lifecycle methods are called when a device-configuration change (such as rotation) occurs?<br/>

-> Android shuts down your Activity by calling onPause(), onStop(), and onDestroy(), and then starts it over again, calling onCreate(), onStart(), and onResume().</p>

<b>Question 3</b><br/>
<p>When in the Activity lifecycle is onSaveInstanceState() called?<br/>

-> onSaveInstanceState() is called before the onStop() method.</p>

<b>Question 4</b><br/>
<p>Which Activity lifecycle methods are best to use for saving data before the Activity is finished or destroyed?<br/>

-> onPause() or onStop()</p>
