source "https://rubygems.org"

eval_gemfile(File.expand_path("Gemfile.common", __dir__))

group :release do
  gem 'chandler', git: 'https://github.com/deivid-rodriguez/chandler', branch: 'submit_link_references' # Github releases from changelog
end

group :lint do
  # Code style
  gem 'rubocop', '0.60.0'
  gem 'rubocop-rspec', '~> 1.30'
  gem 'mdl', '0.7.0'

  # Translations
  gem 'i18n-tasks'
  gem 'i18n-spec'
end

group :docs do
  gem 'yard'     , '>= 0.9.20' # Documentation generator
  gem 'kramdown' , '>= 2.3.1' # Markdown implementation (for yard)
end

gem "rails", "~> 6.1.7", ">= 6.1.7.3"
gem "activerecord-jdbcsqlite3-adapter", "~> 61.0", platform: :jruby

gemspec path: "."
