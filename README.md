Opauth-Harvest
=============
[Opauth][1] strategy for Harvest authentication.

Implemented based on https://github.com/harvesthq/api

Getting started
----------------
1. Install Opauth-Harvest:

   Using git:
   ```bash
   cd path_to_opauth/Strategy
   git clone https://github.com/t1mmen/opauth-harvest.git Harvest
   ```

  Or, using [Composer](https://getcomposer.org/), just add this to your `composer.json`:

   ```bash
   {
       "require": {
           "t1mmen/opauth-harvest": "*"
       }
   }
   ```
   Then run `composer install`.


2. Create Harvest application at https://platform.harvestapp.com/oauth2_clients

3. Configure Opauth-Harvest strategy with at least `Client ID` and `Client Secret`.

4. Direct user to `http://path_to_opauth/harvest` to authenticate

Strategy configuration
----------------------

Required parameters:

```php
<?php
'Harvest' => array(
	'client_id' => 'YOUR CLIENT ID',
	'client_secret' => 'YOUR CLIENT SECRET'
)
```

License
---------
Opauth-Harvest is MIT Licensed
Copyright © 2014 Timm Stokke (http://timm.stokke.me)

[1]: https://github.com/opauth/opauth
