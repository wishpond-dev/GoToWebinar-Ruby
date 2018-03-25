# GoToWebinar
GoToWebinar-Ruby is a Ruby wrapper around Citrix's GoToWebinar REST API.

## Requirements

You must have an active GoToWebinar account and a valid access token from the GoToWebinar OAuth flow. Please refer to the [authentication and authorization documentation](https://developer.citrixonline.com/page/authentication-and-authorization). The OAuth flow will return both the access token and organizer key. Both access token and organizer key are required to use the webinar API. 

##Install

`go_to_webinar` is not an official repository, therefore you will not be able to install the gem with the standard approach.

	gem install go_to_webinar
	
For now, you will need to install from the source.

	gem install go_to_webinar, :git => 'git://github.com/citrixonline/GoToWebinar-Ruby.git'

## Usage

Please refer to the [developer documentation](https://developer.citrixonline.com/api-overview/gotowebinar-rest-api) for a complete list of available methods. 

	@g2w = GoToWebinar::Client.new(oauth_access_token, organizer_key) 
	@g2w.get_webinar(webinar_key)

## Status

Tests are complete and passing.  
