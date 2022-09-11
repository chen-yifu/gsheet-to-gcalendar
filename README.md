# Sync Schedule From Google Sheet to Google Calendar

## How to Use
1. Sign in to your Google Account (we will need Google Calendar and Google Sheet)
2. Open the Personal Schedule on Google Sheet: [link here](https://docs.google.com/spreadsheets/d/1wSM7UDevdz1CKo2oDK4BEM9WT5cxNhAyf1XmFIZLOlU/edit?usp=sharing)
3. Create a copy of Personal Schedule, and you could modify it on your own. Once you are happy with the schedule, proceed to next steps. (alternatively, proceed right now to see how the script works, and you could come back and modify the schedule later and do this again)
4. Create a new calendar within Google Calendar
5. Copy the new calendar's Calendar ID (e.g., okne163oes89abcabcabcabcabc@group.calendar.google.com), which can be found in this calendar's Settings -> Integrate Calendar menu (bottom of the settings page)
6. Paste the calendar's ID to Google Sheet in cell D3
7. Go to Google Sheet's menu bar -> Extensions -> App Script (use Chrome browser if Safari won't open it)
8. Copy the code to the App Script window
9. If you would like to automatically delete all existing events on the Google Calendar, set "var deletePrevEvent = true;" in Line 34. If you are starting with a blank calendar, leave it as "false".
10. Go to App Script menu bar -> Run to run the script to sync the schedule from Google Sheet to Google Calendar
11. Wait for the script to finish. Note: You may have to Run the script multiple times because Google sometimes limits the number of times you can modify the calendar through its API. If that happens to you (you will see a "rate limit exceeded" error in the execution log), just re-run the script while making sure "deletePrevEvent = false".
12. Check your Google Calendar and see your evens have been synced!

## Demo
I created a video demo to show it from start to end: [link here](https://drive.google.com/file/d/16B8mNdyaBpBOszty2FdFLdfatsqPSJV7/view?usp=sharing)

## Note
The App Script should be safe to use and won't send any of your personal information to anyone except Google. Please feel free to check its source code. If you like this project, please give it a star! Thanks.

## Support
If there are questions or issues, please feel free to submit an issue.
