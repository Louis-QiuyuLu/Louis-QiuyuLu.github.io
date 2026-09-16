FROM ruby:2.7-bullseye

# The site is pinned to the `github-pages` gem 215 (Jekyll 3.9.0). Its gem set
# (e.g. nokogiri 1.13.3) requires Ruby < 3.2 and OpenSSL 1.1, both of which the
# ruby:2.7-bullseye image provides. This tag is based on buildpack-deps, so it
# already ships git, curl, and build-essential for compiling native gem
# extensions (ffi, eventmachine, commonmarker, etc.); no extra apt packages are
# required. Dependency installation happens in `install` (see environment.json).
