Ruby Library For Twilio Wrapper
=========================

Class
-----

There's one primary class named `TwilioWithThinq::TwilioWrapper` that wraps all major functions.

Initialization
--------------

```ruby

wrapper = TwilioWithThinq::TwilioWrapper.new  twilio_account_sid, twilio_account_token, thinQ_id, thinQ_token

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

```ruby

	call_sid = wrapper.call from, to

```

> **Return Value**: Proper twilio call Sid if `success`, or relevant error message otherwise.

Quick Start Guide
-----------------

> Here's a simple demo code.

```ruby

require "twilio_thinqlcr_ruby"


twilio_account_sid = "ACa5a21802beff96f147d40bf98c957038"

twilio_account_token = "7852c807435af28d468344ca57a49d2a"

thinQ_id = "11001"

thinQ_token = "0c82a54f22f775a3ed8b97b2dea74036"



wrapper = TwilioWithThinq::TwilioWrapper.new twilio_account_sid, twilio_account_token, thinQ_id, thinQ_token


call_sid = wrapper.call "1234567890", "9876543210"


puts "Call sid: #{call_sid}"

```

Source code is on [@github](https://github.com/harouf/twilio-thinQLCR-ruby).