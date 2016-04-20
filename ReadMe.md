![SimpleAuthentication - making authentication ... simple]

**SimpleAuthentication** is a ASP.NET library that makes it really easy and simple for developers to add *Social Authentication* to an ASP.NET application.


## What does the term "Social Authentication" mean"?

Social Authentication are login buttons that use popular social websites (like Facebook or Google) as the way to login to your own website.
These social websites Facebook/Google/etc are referred to as Social Authentication Providers (aka. AP's).

## Why do we want to offer Social Authentication?

A few reasons:

  - People are getting tired of creating new usernames/passwords all the time.
  - People generally only use the same few passwords for all their accounts. This means that if one of those websites is compromised, then there is a high chance those compromised credentials can be reused on other sites the user has an account on.
  - If you store passwords, then your server is now a possible target/attack vector and now you have to make sure you're protecting your sensitive user data. 
  - The Authentication Providers now have to deal with the security of storing passwords. You've just delegated a huge security responsibility to them :)

## What Authentication Providers are available?

Out of the box, it offers **Facebook**, **Google**, **Twitter** and **Microsoft Live** integration for either 

## How does this compare to ASP.NET Identity / ASP.NET Membership?

 - **Simple Authentication**: An extremely *lightweight* library that only deals with the *authentication*. No database code. No rules forcing you to implement contracts. *No passwords*
 - **ASP.NET Identity / Membership**: a heavy, enterprisy, one-huge-hammer-fits-all approach that is strongly tied to sql server and entity framework.

Simple Authentication doesn't want to tie you into any particular database, data access layer or forcing / maintaining passwords. In essence, we've tried to pass this security concern onto other systems. Once you've received some *authenticated* user information, *you* decide what you want to do with.
On the other hand, ASP.NET Identity/Membership is a full end-to-end stack for user credentials. It's tied to Sql Server and you're tied to implementing all the interface contracts. But most importantly, passwords are still stored in your database if forms authentication was used. It's a one-big-hammer approach.

And Finally ...
--
* I accept Pull Requests.
* Please use the GitHub issues for any other problems.
* License : [MIT](http://www.tldrlegal.com/license/mit-license)
* No Unicorns were harmed in the coding of this library.
