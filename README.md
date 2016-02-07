# Activity Life Cycle #

**To Visible State :
On Activity starting for the first time - onCreate > onStart > onResume

**To Partially visible state :
* On Dialog Activity open - onPause
* On Dialog Activity dismiss - onRestart

**To Invisible state :
* On screen off - onPause > onStop

* On minimising Activity - onPause > onStop

* On reopening a minimised Activity - onRestart > onStart > onResume


* On opening other activity through Intent - onPause > onStop

* On moving back to previous activity - onRestart > onStart > onResume

**On Destroyed state :
* On back button pressed - onPause > onStop > onDestroy
* On finish - onPause > onStop > onDestroy