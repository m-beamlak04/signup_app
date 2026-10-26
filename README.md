**Question 1: Trace the local tip feature from button tap to displayed text. Which widget/state changes during the simulated loading state, and how does the user recover from the local error case?**

When the user presses the Get Signup Tip button, a loading circle appears for a quick second before the password advice shows up. During that time, the loading state changes and the button is disabled until the tip is ready. If it fails to load, a red error message appears with a Retry button that lets the user try again.

**Question 2: Why must the app keep form validation local even when it can ask an AI for a tip? Give one example of a bad decision if AI were allowed to approve signup.**

The app should keep form validation local because it needs to make sure the information entered meets the signup requirements. If AI were allowed to approve signup, it could incorrectly approve someone with an invalid email or a password that is too short. This would be a problem because the form doesn't actually meet the requirements, but the app could still say the signup was successful.