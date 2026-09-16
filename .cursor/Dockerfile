FROM ruby:2.7-bullseye

# The site is pinned to `github-pages` gem 215 (Jekyll 3.9.0). Its gem set
# (e.g. nokogiri 1.13.3) requires Ruby < 3.2 and OpenSSL 1.1, both of which
# the ruby:2.7-bullseye image provides out of the box.
RUN apt-get update \
    && apt-get install -y --no-install-recommends build-essential git curl \
    && rm -rf /var/lib/apt/lists/*
