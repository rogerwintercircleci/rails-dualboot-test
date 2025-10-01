# Rails Dual Boot Test Project

This project demonstrates the Rails dual boot strategy for upgrading between major Rails versions.

## Current Setup

- **Current Version**: Rails 7.2.2
- **Target Version**: Rails 8.0.3
- **Ruby Version**: 3.2.3

## Dual Boot Configuration

This project uses the manual dual boot setup.

## CircleCI Pipeline

The CircleCI configuration includes two jobs running in parallel to test both Rails versions.

## Running Locally

Test with current Rails version:
```bash
bundle install
bundle exec rails --version
```

Test with next Rails version:
```bash
bundle install --gemfile=Gemfile.next
BUNDLE_GEMFILE=Gemfile.next bundle exec rails --version
```
