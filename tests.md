time sudo -u www-data php scripts/run-tests.sh --php /usr/bin/php --url http://seed.local/ --color --concurrency 4 --all

CORE

Database (MYISAM => InnoDB pass)
 - Invalid data (DatabaseInvalidDataTestCase)
	Invalid data 8 passes, 1 fail, and 0 exceptions
 - Transaction tests (DatabaseTransactionTestCase)
	Transaction tests 71 passes, 8 fails, and 0 exceptions
Field API (MYISAM => InnoDB pass)
 - Field SQL storage tests (FieldSqlStorageTestCase)
 	Field SQL storage tests 101 passes, 0 fails, and 1 exception
Node (MYISAM => InnoDB pass)
 - Node creation (NodeCreationTestCase)
	Node creation 40 passes, 1 fail, 0 exceptions, and 10 debug messages
File
 - File field validation tests (FileFieldValidateTestCase)
	File field validation tests 110 passes, 4 fails, 6 exceptions, and 34 debug messages
Filter
 - Filter module filters (FilterUnitTestCase)
	Filter module filters 214 passes, 1 fail, and 0 exceptions
	HTML scheme clearing evasion -- spaces and metacharacters before scheme.	Other	filter.test	1103	FilterUnitTestCase->testFilterXSS()
Image
 - Image dimensions (ImageDimensionsTestCase)
	Image dimensions 30 passes, 24 fails, 5 exceptions, and 8 debug messages
 - Image field display tests (ImageFieldDisplayTestCase)
	Image field display tests 158 passes, 4 fails, 0 exceptions, and 52 debug messages
OpenID
 - OpenID helper functions (OpenIDTestCase)
	OpenID helper functions 41 passes, 2 fails, and 0 exceptions
Poll
 - User poll vote capability. (PollVoteCheckHostname)
	User poll vote capability. 133 passes, 14 fails, 0 exceptions, and 38 debug messages
Session
 - Session HTTPS handling (SessionHttpsTestCase)
	Session HTTPS handling 76 passes, 7 fails, 0 exceptions, and 25 debug messages
 - Session tests (SessionTestCase)
	Session tests 188 passes, 4 fails, 0 exceptions, and 52 debug messages
System
 - Tablesort (TableSortTest)
	Tablesort 0 passes, 0 fails, and 1 exception
Tracker
 - Tracker (TrackerTest)
	Tracker 288 passes, 0 fails, 2 exceptions, and 87 debug messages
Upgrade path (SimpleTest)
 - Taxonomy upgrade path (UpgradePathTaxonomyTestCase)
	Taxonomy upgrade path 1282 passes, 24 fails, 24 exceptions, and 46 debug messages

CONTRIB

Localization Update
 - Update translations using cron (L10nUpdateCronTest)
	Update translations using cron 61 passes, 5 fails, 0 exceptions, and 27 debug messages
 - Update translations (L10nUpdateTest)
	Update translations 535 passes, 36 fails, 1 exception, and 210 debug messages

Services
 - Resource Comment (ServicesResourceCommentTests)
	Resource Comment 223 passes, 0 fails, 6 exceptions, and 59 debug messages
 - Resource File (ServicesResourceFileTests)
	Resource File 107 passes, 1 fail, 5 exceptions, and 31 debug messages
 - Resource Node - taxonomy (ServicesResourceNodeTaxonomytests)
	Resource Node 271 passes, 5 fails, 15 exceptions, and 73 debug messages
 - Resource Taxonomy (ServicesResourceTaxonomyTests)
	Resource Taxonomy 362 passes, 0 fails, 6 exceptions, and 84 debug messages
 - Resource User (ServicesResourceUsertests)
	Resource User 623 passes, 3 fails, 0 exceptions, and 239 debug messages
 - Version System (ServicesVersionTests)
	Version System 28 passes, 8 fails, 0 exceptions, and 9 debug messages

Link
 - Link Light Validation Tests (LinkValidateUrlLight)

non-zero code

LinkValidateUrlLight

[02-Dec-2014 11:15:25 Asia/Yekaterinburg] PHP Fatal error:  Call to undefined function link_validate_url() in /home/andribas/www/seed/sites/all/modules/contrib/link/tests/link.validate.test on line 391
[02-Dec-2014 11:15:25 Asia/Yekaterinburg] PHP Stack trace:
[02-Dec-2014 11:15:25 Asia/Yekaterinburg] PHP   1. {main}() /home/andribas/www/seed/scripts/run-tests.sh:0
[02-Dec-2014 11:15:25 Asia/Yekaterinburg] PHP   2. simpletest_script_run_one_test() /home/andribas/www/seed/scripts/run-tests.sh:23
[02-Dec-2014 11:15:25 Asia/Yekaterinburg] PHP   3. DrupalTestCase->run() /home/andribas/www/seed/scripts/run-tests.sh:369
[02-Dec-2014 11:15:25 Asia/Yekaterinburg] PHP   4. LinkValidateUrlLight->testValidateFrontLink() /home/andribas/www/seed/modules/simpletest/drupal_web_test_case.php:517

Notice

Services
a:3:{i:0;s:22:"Undefined index: files";i:1;s:6:"Notice";i:2;a:3:{s:8:"function";s:33:"_node_resource_file_save_upload()";s:4:"file";s:86:"/home/andribas/www/seed/sites/all/modules/contrib/services/resources/node_resource.inc";s:4:"line";i:708;}}
