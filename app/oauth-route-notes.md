# Notes on adding an OAuth endpoint

I have modified routes.php (the file which controls how urls are processed) so that .../seat/account/oauth/authorize is analogous to login.eveonline.com/oauth/athorize.

To do this, I have also created a controller (routes.php immediately redirects to this controller, which needs to do the actual work of processing/authorizing OAuth) in ./controllers/OAuthController.php, and a view (i.e. the actual html code that the user sees) in ./views/oauth/authorize.blade.php.







