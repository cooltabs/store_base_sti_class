RAILS_VERSIONS = %w[
  5.0.7
  5.1.7
  5.2.3
  5.2.4
  6.0.3
  6.1.0
].freeze

RAILS_VERSIONS.each do |version|
  appraise "rails_#{version}" do
    gem 'activerecord', version
    gem 'sqlite3', ['6.0.3', '6.1.0'].include?(version) ? '~> 1.4.0' : '~> 1.3.0'
  end
end
