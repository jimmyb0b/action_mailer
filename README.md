# action_mailer

Action Mailer allows you to send email from your rails app!

Once you've created a new rails app, you can generate the mailer similarly to any other controller. 
	
	''' rails generate mailer new_mailer_name '''


Just like other controllers, mailers use methods and views to structure content, but instead of rendering an HTML page, it fires off a email.

There are essentially 3 methods that make up any email. 
	- headers - these are the atributes you want to pass in, name, email, url, etc.
	- attachments - any files to send with email
	- mail - the actual text of the email. This can make use any of the headers that you've defined.

