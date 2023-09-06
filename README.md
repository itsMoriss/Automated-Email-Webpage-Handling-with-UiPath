# Automated-Email-Webpage-Handling-with-UiPath
<p>
  1. This workflow retrieves all the unread emails from the account in use that have 'Course Invoices' in the subject line. <br/>
  2. Emails retrieved are saved in the 'CourseEmails' list MailMessage type of variable. <br/>
  3. Afterwards, attachments for each mail message retrieved are saved in a new project folder titled 'Invoices'. <br/>
  4. It then identifies and copies the client code from each attachment and stores it under the 'ClientCode' variable. <br/>
  5. Next, using the Edge browser, it accesses the 'https://acme-test.uipath.com/first-automation' webpage, clicks 'Part 2' and types the client code to get the discount value. <br/>
  6. The discount value is stored under the 'DiscountValue' variable (this operation is repeated for all stored client codes). <br/>
  7. If the discount value contains the "$" character, the value will be typed in the 'Invoice' sheet in the 'E18' cell. Otherwise, the value "0$" will be added. <br/>
  8. Next, the signature is added in each of the invoice sheets. <br/>
  9. Finally, it writes the text to be used to prepare an Outlook draft email containing the updated invoices. <br/> 
</p>
