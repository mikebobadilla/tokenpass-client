A Laravel package for applications that wish to use Tokenly Accounts for user authentication.

# Installation


### Add the Laravel package via composer

composer require tokenly/accounts-client



### Add Service Provider

Add the following to the `providers` array in your application config:

`Tokenly\AccountsClient\Provider\TokenlyAccountsServiceProvider::class`



### Publish and set the config

`artisan vendor:publish --provider="Tokenly\AccountsClient\Provider\TokenlyAccountsServiceProvider"`

Then edit the file at `config/tokenlyaccounts.php`.

You will need a client id and client secret generated by Tokenly Accounts.



### Configure your controller, routes and views

See the example [controller](examples/controllers/AccountController.php), [views](examples/view) and [routes](examples/routes.php).

