# action_mailer

Action Mailer allows you to send email from your rails app!

Once you've created a new rails app, you can generate the mailer similarly to any other controller. 
	
	''' rails generate mailer new_mailer_name '''


Just like other controllers, mailers use methods and views to structure content, but instead of rendering an HTML page, it fires off a email.

There are essentially 3 methods that make up any email. 
	- headers - these are the atributes you want to pass in, name, email, url, etc.
	- attachments - any files to send with email
	- mail - the actual text of the email. This can make use any of the headers that you've defined.


Action Mailer can send emails through an email app such as gmail, mailgun, or others.
You can also send from a local server, but to do so, you need to have two servers running, one for you're app and another for the mailer.


Important Notes:

Not all clients accept an email formatted with HTML, so it's best practice to create both and HTML and a text email. Action Mailer will automatically generate both.


Action Mailer is intgrateed with Active Job, so you decide when you want to send emails. Either immediately with 'deliver_now' or use 'deliver_later' to set a different delivery schedule.
