# reactland

# 1-Create database
bin/console doctrine:database:create
# 2-Create entity
bin/console make:entity
# 3-Migration
bin/console make:migration
# 4-Push migration
bin/console doctrine:migration:migrate
# 5-Create fixtures
import orm-fixtures from composer
composer require orm-fixtures --dev
php bin/comsole make:fixtures
create fixtures in DataFixtures folder
and load fixtures in database with : php bin/console doctrine:fixtures:load