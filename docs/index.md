# Welcome to Twilio Wrapper Library For thinQ LCR integration

The thinQ Twilio Wrapper Library is just written for the purpose to bring a new level of ease to the developers who deal with Twilio integration with [thinQ LCR](http://www.thinq.com/lcr/) system.

To say more in detail, this is written to help developers who use Twilio Voice to integrate a Least Cost Routing feature into the product so that you can route calls for an average of $0.0047 per minute rather than the $0.015 per minute charged by Twilio voice.

*__Note that you will need a valid LCR Account with thinQ before using the libraries. For more information please contact your thinQ Sales representative at [http://www.thinq.com/library/](http://www.thinq.com/library/)__*

> **Here's a simple scenario:**

> - Twilio outbound calls are charged at rate of $0.015 per minute for all calls to local US numbers and charged in one minute increments.  So, a 61 second call bills for 120 seconds.
> - You have an application that places outbound calls such as Appointment Reminders for customers.
> - Instead of paying $0.015 per minute and being billed by the minute by Twilio, you integrate the thinQ LCR code library into your application as shown below and you pay Twilio for a SIP connection at $0.005 per minute and thinQ for LCR routing at an average rate of $0.0047 per minute (billed in six second increments not one minute increments).
> - Your cost per call should drop by 30-50%.

## So what does it do exactly?

> - Built a wrapper class that wraps all twilio-related operations such as `Service Initialization`, `Making a Call`, `Generating Twiml callback response`, etc.
> - It provides a rich set of configuration parameters.
> - That's it! Developers can intialize this wrapper class obejct with his specific details (incl. Twilio credentials) and just do what he wants in a breeze.

*This library doesn't do any automation thing, but it's a simple library taht only wraps thinQ SIP call so it's obviously up to developers how to use this library.*

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