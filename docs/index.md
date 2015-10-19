# Welcome to Twilio Wrapper Library For thinQ LCR integration

Twilio Wrapper Library is just written for the purpose to bring a new level of ease to the developers who deal with Twilio integration with [thinQ LCR](http://www.thinq.com/lcr/) system.

The initiative of this library is based on the demand to write a module for website solutions that implements a feature which in turn enables the end users of the system to call their dedicated thinQ LCR service line directly.

*__Note that you will need a valid LCR Account with thinQ before using the libraries. For more information please contact your thinQ Sales representative at [http://www.thinq.com/library/](http://www.thinq.com/library/)__*

> **Here's a simple scenario:**

> - A end user visits your website. e.g. `http://www.example.org`
> - He navigates through the pages and comes to have some questions to ask.
> - Although there's customer contact page on the website, he sees a form from which he can initiate a call directly.
> - He puts his number and click the 'call' button, he will receive a follow up call on his phone.
> - Upon acceptance of the call, he will be friendly directed to thinQ line.

## So what does it do exactly?

> - Built a wrapper class that wraps all twilio-related operations such as `Service Initialization`, `Making a Call`, `Generating Twiml callback response`, etc.
> - It provides a rich set of configuration parameters.
> - That's it! Developers can intialize this wrapper class obejct with his specific details (incl. Twilio credentials) and just do what he wants in a breeze.

## Language support
> - [PHP](php.md)
> - [.NET (C#)](dotnet.md)
> - [Python](python.md)
> - [Java](java.md)
> - [Ruby](ruby.md)
> - [NodeJS](nodejs.md)

## Dependencies
  > PHP

  > - PHP >= 5.2.3
  > - [twilio-php 4.3.0](https://www.github.com/twilio/twilio-php)

  > .NET

  > - .NET Framework >= 4.5
  > - [RestSharp 105.2.2](https://github.com/restsharp/RestSharp)
  > - [Twilio 4.0.51](https://github.com/twilio/twilio-csharp)

  > Python

  > - [Twilio](https://github.com/twilio/twilio-python)

  > Java

  > - [Twilio](https://github.com/twilio/twilio-java)

  > Ruby

  > - [twilio-ruby](https://github.com/twilio/twilio-ruby)

  > NodeJS
  
  > - [Twilio](https://github.com/twilio/twilio-node)

Documentation source is on [@github](https://github.com/harouf/twilio-thinQLCR-doc)

#### *Authored by @Fujio Harou, 2015*