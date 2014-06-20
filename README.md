# Puppet S3 File synchronization

Requires [puppetlabs/stdlib](https://github.com/puppetlabs/puppetlabs-stdlib) module.

Example Usage:

    include 's3file::curl'
    s3file { '/path/to/destination/file':
      source => 'MyBucket/the/file',
      ensure => 'latest',
    }
