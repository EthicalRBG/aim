# AIM

AIM attempts to simplify the creation of AIM bots or do things log log all IMs to an AIM chat room, etc.

## Currently working Usage

```ruby
require 'rubygems'
require 'aim'

AIM.login_as_user( 'screenname', 'password' ) do

  im_user 'some user to IM', "hello!  the time is #{ Time.now }"

  log_chatroom 'the name of some chat room to log into', :output => 'file-to-save-chatroom-logs-to'

end
```

## NOTES

this app makes heavy use of Net::TOC, which I believe was 
originally created by Ian Henderson: http://rubyforge.org/users/ianh/

http://rubyforge.org/projects/net-toc/ is released under 
the BSD License: http://www.debian.org/misc/bsd.license

I am mentioning the name of the author to give him credit.

Per the BSD License, I will NOT use the author's name to 
endorse or promote this product!

## TODO

1. get a purty DSL working (using net/toc in the background)
2. refactor net/toc --> AIM
