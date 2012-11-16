# Zipsy

Zip code data without external dependencies

## Usage

Add it to your Gemfile

```ruby
gem "zipsy", git: "https://github.com/ankane/zipsy"
```

Call it

```ruby
Zipsy.find("94108")
# {
#   :city=>"San Francisco",
#   :state=>"CA",
#   :lat=>37.79,
#   :lng=>-122.4,
#   :time_zone=>"Pacific Time (US & Canada)",
#   :decommissioned=>false
# }

Zipsy.find("123456")
# nil
```

## Sources

City, state, latitude, longitude, and decommissioned from [federalgovernmentzipcodes.us](http://federalgovernmentzipcodes.us)

Time zone from the [tzip](https://github.com/farski/TZip) gem
