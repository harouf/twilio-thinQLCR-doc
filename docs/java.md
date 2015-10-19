Java Library For Twilio Wrapper
=========================

Class
-----

There's one primary class named `TwilioWrapperLibrary` that wraps all major functions, and one builder class named `TwilioWrapperLibraryBuilder` that is a utility class to build the library object.

Initialization
--------------

```

TwilioWrapperLibrary library = new TwilioWrapperLibraryBuilder()

	  .twilio(twilio_account_sid, twilio_account_token, twilio_phone_number)

      .thinQ(thinQ_id, thinQ_token)

	  .buildLibrary();

```

Configuration Parameters
------------------------

- ####twilio_account_sid:
  
  > You can get Twilio account sid from your Twilio account dashboard.

- ####twilio_account_token:

  > You can get Twilio account token from your Twilio account dashboard.

- ####thinQ_id:

  > ThinQ id that you recenved when you sigend up thinq.com.

- ####thinQ_token:

  > ThinQ token that you recenved when you sigend up thinq.com.

Initiate a call to the thinQ line
------------------------------------

```

	String result = library.call(from, to);

```

> **Return Value**: Proper twilio call Sid if `success`, or relevant error message otherwise.

Quick Start Guide
-----------------

> Here's a simple demo code.

```

import com.twilio.thinq.TwilioWrapperLibrary;

import com.twilio.thinq.TwilioWrapperLibraryBuilder;



public class Main {

    public static void main(String[] agrgs){

        TwilioWrapperLibrary library = new TwilioWrapperLibraryBuilder()

                // twilio account sid, account token, registered twilio phone number
                .twilio("ACa5a21802beff96f147d40bf98c957038", "7852c807435af28d468344ca57a49d2a")

                // set thinQ details
                .thinQ("11001", "0c82a54f22f775a3ed8b97b2dea74036")

                // wrap and build the library
                .buildLibrary();

        String result = library.call("1234567890", "9876543210"); //return value is call sid if success, otherwise error message.

        System.out.println("result: " + result);

    }

}

```

Source code is on [@github](https://github.com/harouf/twilio-thinQLCR-java).