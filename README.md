This is a gem for using backblaze with activestorage.

Use this gem with my fork of fog-backblaze:

```ruby
gem 'fog-backblaze', '~> 0.3.0', :git => 'https://github.com/PascalMayr/fog-backblaze.git'
```

# Usage:

```ruby
gem 'activestorage-backblaze'
```

Then in your storage.yml, use the following

```yaml
backblaze:
  service: Backblaze
  bucket_name: <bucket_name>
  bucket_id: <bucket_id>
  key_id: <keyId>
  key_token: <keyToken>
```

In your environments/production.rb or application.rb (depending on your choice) add the following:

```ruby
config.active_storage.service = :backblaze
```
