---
title: 'Collecting a full log on Adguard for Android'
taxonomy:
    category:
        - docs
visible: true
---

Sometimes in order to understand a problem and fix it we need to collect **log files**, or **logs**. Basically, these files contain information about the program and it's work. To collect those logs and send them to us you need to perform following steps:

1. Open AdGuard and go to "Settings".

2. Choose "Advanced" in the left menu.

3. Set "Logging level" to "Record everything". It's desirable to close all background apps that don't concern the problem beforehand.

4. Reproduce the problem and set the logging level back to "Default". Notice the exact time when it happened.

5. Send us a message from program by choosing "Send Feedback" in the menu. Don't forget to check the "Send detailed system info" checkbox under the text field and to include the timestamp from the step 4 into the message.

As an alternative, you can export the logs (along with the *state.txt* file that contains information about AdGuard and system settings) directly into a local file. It can be convenient, for example, if you are having a conversation with a developer on [GitHub](https://github.com/Adguardteam/), [forum](https://forum.adguard.com/) or on another platform.

To export logs and system information into a file, go to "Settings — Advanced" and tap on "Export logs and system info". Select the destination folder and tap on "Save".
