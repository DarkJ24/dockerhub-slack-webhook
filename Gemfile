# frozen_string_literal: true

source "https://rubygems.org"

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

ruby "2.6.5"

gem "activesupport", require: "active_support/all"
gem "puma"
gem "puma-heroku"
gem "rollbar"
gem "sinatra"
gem "sinatra-contrib"
gem "slack-notifier"

group :development do
  gem "foreman", require: false

  # TODO: Remove after https://github.com/onk/onkcop/pull/62 and https://github.com/onk/onkcop/pull/63 are merged
  # gem "onkcop", ">= 0.53.0.3", require: false
  gem "onkcop", require: false, github: "sue445/onkcop", branch: "rubocop_0.72.0"

  gem "rake", require: false
  gem "rubocop-performance", require: false
end

group :test do
  gem "coveralls", require: false
  gem "rack-test"
  gem "rspec"
  gem "simplecov", require: false
end
