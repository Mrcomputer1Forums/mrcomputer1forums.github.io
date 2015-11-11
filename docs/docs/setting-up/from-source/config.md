**Setting Up -> From source code**

# Config

Forum/forum_settings.py
**The # before a config item is the info about that config item (The file below is kind of modified to add the comment)**
```python
############################################################
##########  Mrcomputer1Fourm Settings File        ##########
############################################################

FORUM_SETTINGS = {
	# "(CONFIG KEY - DON'T CHANGE)": "(CONFIG VALUE - CHANGE)",

	# This is the forum's name
    "FORUM_NAME": "My forum name",
	
	# This is the root - It normally does not need to change
    "FORUM_ROOT": "/",
	
	# This is the url to the admin site - Same as above it does not need to change normally
    "SITE_ADMIN": "/admin/",
	
	# This section is hidden to anyone that is not mod or admin
    "STAFF_SECTION": -1, # Use -1 to disable
	
	# This is the forum that deleted topics are sent to
    "BIN_FORUM": -1, # Use -1 to disable
	
	# This is the topic that deleted posts are sent to
    "BIN_TOPIC": -1, # Use -1 to disable
	
	# This is the forum that ban appeals are sent to
    "APPEAL_FORUM": -1, # Use -1 to disable
	
	# This is the forum that only mods and admins an create a topic in
    "NEWS_FORUM": -1, # Use -1 to disable
	
	# Change this to True to enable the announcement system
    "ALERT_ON": False,
	
	# This is the message said by the announcement system
    "ALERT_MSG": "Test alert",
}
```