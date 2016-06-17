# Active Admin

Active Admin is a Ruby on Rails framework for creating elegant backends for website administration.

```ruby
gem 'activeadmin', '~> 1.0.0.pre2'
```

### Rails 5

Active Admin master has preliminary support for Rails 5. To give it a try, these Gemfile changes may be needed:

```ruby
gem 'devise',      '> 4.x'
gem 'rspec-rails', '>= 3.5.0.beta1'
gem 'ransack',    github: 'activerecord-hackery/ransack'
gem 'kaminari',   github: 'amatsuda/kaminari', branch: '0-17-stable'
gem 'formtastic', github: 'justinfrench/formtastic'
gem 'draper',     github: 'audionerd/draper', branch: 'rails5', ref: 'e816e0e587'
# To fix a Draper deprecation error
gem 'activemodel-serializers-xml', github: 'rails/activemodel-serializers-xml'
# Optional -- only if you already include these gems
gem 'rack-mini-profiler',          github: 'MiniProfiler/rack-mini-profiler'
gem 'database_cleaner',            github: 'pschambacher/database_cleaner', branch: 'rails5.0', ref: '8dd9fa4'
# Only for JRuby:
gem 'activerecord-jdbc-adapter',   github: 'jruby/activerecord-jdbc-adapter', platforms: :jruby
```

source : http://activeadmin.info/