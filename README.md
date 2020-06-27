```
cp config/database.yml.sample config/database.yml
bundle exec rails g rename:into New-Name
cd New-Name
bundle install --without production
bundle exec rails db:create
bundle exec rails db:migrate
bundle exec rails default:system_user
bundle exec rails s
