### REFrameWork Queue Template ###
**AS001_DocumentRedactions_Email**

The first subprocess aims to automate the processing of emails. Our goal is to standardize the sending of emails received in the admissions and electronic transcripts mailboxes. We propose creating an automation email inbox where internal emails (ending with the @nova.edu domain) should be directed. The individuals sending these emails will undergo training for the proper use of the solution.

The automation will be integrated with Outlook and will check the message inbox for new emails every 5 minutes. The email should include three key elements: a standardized subject, a PDF attachment, and an Excel file containing information associating the PDF with a Banner ID and other necessary details.

Upon receiving the email, the automation will validate the subjects, download the attachments, and verify their content. If the validations are successful, it will perform a search in Banner in case additional information is required. Subsequently, it will upload the document and its respective information to Image Director, notifying the user that the document has been successfully uploaded.

If the email fails to meet the validations, it will be returned to the user with a copy to the business, indicating errors in the request. The user will be informed that they need to correct the document for processing or resend it to the initially mentioned mailboxes for manual processing by a human.



