# Ruby Cli Wiki

## Disable SSL Verification
```
require 'openssl'
OpenSSL::SSL::VERIFY_PEER = OpenSSL::SSL::VERIFY_NONE
```

## Install

Init the GEM file.
```
bundle init
```
## Using dotenv
```
gem "dotenv"
```
### Create an .env file
```
TWITTER_API_KEY="my-twitter-api-key"
TWITTER_API_SECRET="my-twitter-api-secret"

GITHUB_ACCESS_TOKEN="my-github-access-token"
```

### put an env var (test.rb)
 ```
 # Load the dotenv gem
require 'dotenv'

# This tells dotenv to read the .env file and set the appropriate variables
Dotenv.load

puts "Here are all your current environment variables:"


puts ENV['TWITTER_API_SECRET']
```
#### run the file:

```
ruby test.rb
```
