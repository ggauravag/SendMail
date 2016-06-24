# SendMail
It is a JAVA utility to send email using executable JAR with configurable smtp and email settings. 

Following are the arguments used to configure smtp settings:

<b>-host</b>
SMTP host name, for example smtp.google.com

<b>-port</b>
SMTP port number, for example 587, default: 465

<b>-message</b>
Message text to be sent, if with mutiple words, use "Hello, This is a sample message." (use double quotes to wrap)

<b>-subject</b>
Subject text to be set, like "My Test Mail"

<b>-H</b>
A flag, used to set the content type as HTML

<b>-debug</b>
To enable debug log of mail sending process.

<b>-from</b>
Sender email and name, for example someone@example.com:John or someone@example.com (name defaults to the email id)

<b>-to</b>
List of the email TO receipents separated by colon (:), for example account1@example.com:abc@yahoo.com:bcd@gmail.com

<b>-bcc</b>
List of the email BCC receipents separated by colon (:), for example account1@example.com:abc@yahoo.com:bcd@gmail.com

<b>-cc</b>
List of the email CC receipents separated by colon (:), for example account1@example.com:abc@yahoo.com:bcd@gmail.com

<b>-auth</b>
To use auth like username & password, for example someone@gmail.com:password

To use the project, download the sendmail.jar

and run this command to execute the jar with your smtp settings:

<b>java -jar sendmail.jar -host smtp.example.com -port 587 -auth gaurav@example.com:Example# -message "Hi, Sample Message " -H -to someone@example.com -cc account1@example.com:account2@example.com -from gaurav@example.com:Gaurav -subject "Test Email"</b>
