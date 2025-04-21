The marketing team of an e-commerce site has launched an email campaign. This site has email addresses from all the users who created an account in the past.
They have chosen a random sample of users and emailed them. The email lets the user know about a new feature implemented on the site. From the marketing team perspective, success is if the user clicks on the link inside of the email. This link takes the user to the company site.



The 3 tables are:
email_table - info about each email that was sent
Columns:
email_id : the Id of the email that was sent. It is unique by email.
email_text : there are two versions of the email: one has “long text” (i.e. has 4 paragraphs) and one has “short text” (just two paragraphs)
email_version : some emails were “personalized” (i.e. they had the name of the user receiving the email in the incipit, such as “Hi John”), while some emails were “generic” (the incipit was just “Hi,”).
hour : the local time on which the email was sent.
weekday : the day on which the email was sent.
user_country : the country where the user receiving the email was based. It comes from the user ip address when she created the account.
user_past_purchases : how many items in the past were bought by the user receiving the email

email_opened_table - the id of the emails that were opened at least once.
Columns:
email_id : the id of the emails that were opened, i.e. the user clicked on the email and, supposedly, read it.

link_clicked_table - the id of the emails whose link inside was clicked at least once.
Columns:
email_id : if the user clicked on the link within the email, then the id of the email shows up on this table


The aim of the project is to identify a model which predicts the correct number of emails that will have their links clicked. The project also provides insight into which factors will be crucial in deciding which email links are clicked and which are not.