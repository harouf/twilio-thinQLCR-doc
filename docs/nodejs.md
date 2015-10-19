NodeJS Library For Twilio Wrapper
=========================

Class
-----

There's one primary class named `TwilioWrapper` that wraps all major functions as prototype methods.

Initialization
--------------

```javascript

var wrapper = new TwilioWrapper(

        twilio_accountSid,                    // twilio account sid  

        twilio_authToken,                     // twilio account token

        thinQ_id,                             // thinQ id

        thinQ_token                           // thinQ token

    );

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

```javascript

  var return_promise = wrapper.call(from, to);

```

> **Return Value**: Proper promise object for the initiated twilio call if `success`, or `null` otherwise.

Quick Start Guide
-----------------

> Here's a simple demo code.

```javascript

var TwilioWrapper = require('twilio-thinqlcr-node');


var twilio_accountSid = 'ACa5a21802beff96f147d40bf98c957038';

var twilio_authToken = '7852c807435af28d468344ca57a49d2a';

var thinQ_id = '11001';

var thinQ_token = '0c82a54f22f775a3ed8b97b2dea74036';


var wrapper = new TwilioWrapper(

        twilio_accountSid,                    // twilio account sid  

        twilio_authToken,                     // twilio account token

        thinQ_id,                             // thinQ id

        thinQ_token                           // thinQ token

    );


var return_promise = wrapper.call("1234567890", "9876543210");


return_promise.then(function(call){

  console.log("Successfully initiated a new call to customer!");

  console.log("Call sid: " + call.sid);

}, function(error){

  console.log(err);

});


```

Source code is on [@github](https://github.com/harouf/twilio-thinQLCR-node).