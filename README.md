# Accessiblity Bug

This repo is to demonstrate issues with Android Accessibility


### BottomNavigationView - https://issuetracker.google.com/issues/37151340
The BottomNavigationView does not give a hint that use is using bottom navigation.
It just reads the title of the tab and does not let the user know how many tabs are present, which of the tab they are currently navigating.

GooglePlus app however, has a better implementation where it would read "<tab name>, Tab 1 of 4".

*Step 1:* Enable Talkback

*Step 2:* Open the app
 
*Step 3:* Navigate to bottom nav using swipe, it reads: "Home, double tap to activate", another swipe, "Dashboard, double tap to activate".
It should read "Home, active, Tab 1 of 3", "Dashboard, Tab 2 of 3, double tap to activate"
