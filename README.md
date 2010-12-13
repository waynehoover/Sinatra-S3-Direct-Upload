# Sinatra AWS S3 Direct Upload Example

## Install

A simple Sinatra app to upload files directly to Amazon S3 using jQuery SWFUpload.  

Tested on ruby 1.9.2. Install these gems if you haven't already:
                                        
	gem install activesupport
	gem install hpricot 
	gem install sinatra         

Make sure hpricot is at least at version 0.8.3         

# Instructions:

Put the `crossdomain.xml` file in the root of your s3 bucket and make it readable.

Modify the `bucket`, `access_key`, and `secret_access_key` variables at the top of `main.rb` to match your AWS credentials.

	$ruby main.rb 

Then go to http://localhost:4567/upload 