# PowerBI

Category - Email / html / DAX 
1. To open an email client with a prebuilt message from a Power BI web report, you can use a DAX measure to create a "mailto" hyperlink. Here's an example of how you might set up the measure:

```plaintext
Mailto = "mailto:" & [Email] & 
"?subject=" & "Your Subject Here" & 
"&body=" & "Your prebuilt message here"
```

Replace `[Email]` with the email address field from your dataset, and customize the subject and body text as needed. Once set up, clicking the textbox in your Power BI web report will trigger the opening of the default mail client with the prebuilt message.

Example

```plaintext
mailto:xyz@abc.com?cc=abcd@kjl.com
&subject=MESSAGE_1%20%
&body=%20BODY_CONTENT_LINE1%20%0D%0A%
%20BODY_CONTENT_LINE2%200D%0A
```

The code is a URL-encoded string.
%20 represents a space.
%3A represents a colon (:).

%0D represents a carriage return (CR).
%0A represents a line feed (LF).
The combination of above both will start content with new line


#

2. To do something
