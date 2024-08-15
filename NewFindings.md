# PowerBI

Category - Email / html / DAX 
1. To open an email client with a prebuilt message from a Power BI web report, you can use a DAX measure to create a "mailto" hyperlink. Here's an example of how you might set up the measure:

```plaintext
Mailto = "mailto:" & [Email] & 
"?subject=" & "Your Subject Here" & 
"&body=" & "Your prebuilt message here"
```

Replace `[Email]` with the email address field from your dataset, and customize the subject and body text as needed. Once set up, clicking the textbox in your Power BI web report will trigger the opening of the default mail client with the prebuilt message.

#

2. To do something
