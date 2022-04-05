# Activity-lifecycle-and-state
tasks challenges homework

<b>Activity lifecycle</b><br/>

<p>The Activity lifecycle and state app looks and behaves roughly the same as it did in the last codelab. It contains two Activity implementations and gives the user the ability to send between them</p><br/>

<img src="screenshots/activitylifecycle.gif" width="300px" height="600px">
<br/>

<b>Lifecycle Homework</b><br/>
<p> An app with a layout that holds a counter TextView, a Button to increment the counter, and an EditText Implement onSaveInstanceState() to save the current state of the app.</p><br/>

<img src="screenshots/lifecycle_homework.gif" width="300px" height="600px">
<br/>
<img src="screenshots/lifecycleHomework.png" width="300px" height="600px">
<br/>

<b>layout challenge</b><br/>
<p>A simple shopping-list app with a main activity for the list the user is building, and a second activity for a list of common shopping items. 
an Intent to pass information from one Activity to another. Current state of the shopping list is saved when the user rotates the device</p><br/>

<img src="screenshots/lifecycle_challenge.gif" width="300px" height="600px">
<br/>

<b>Logcat Activity of lifecycle</b><br/>
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
