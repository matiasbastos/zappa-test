# Just a Zappa + Flask test

This will deploy a simple Flask app

## Setup
    # configure your AWS keys
    $ aws configure
	# virtualenv
	$ virtualenv env
	$ source env/bin/activate
	# install dependencies
	$ pip install -r requirements.txt	

## Deploy WSGI App
    # deploy API to dev environment
    $ zappa deploy dev

    # Zappa will creates the API Gateway url for you similar to this
    $ curl https://123456.execute-api.us-west-2.amazonaws.com/dev

## Monitor Log
    # check dev environment
    $ zappa tail dev
