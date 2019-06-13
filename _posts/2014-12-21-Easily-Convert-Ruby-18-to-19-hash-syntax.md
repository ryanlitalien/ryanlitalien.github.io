---
layout: post
title: Easily Convert Ruby 1.8 to 1.9 hash syntax
published_at: 2014-12-21
tags:
  - Technology
  - Ruby
---

You can easily convert your 1.8 hash rockets into cleaner, easier to read 1.9 hash syntax with this little script.

A single (ERB) file:

    find . -name _file_upload.html.erb -exec ruby -i -p -e "gsub(/([^:]):(\w+)\s*=>/, '\1\2: ')" {} \;

or multiple (Ruby) files:

    find . -name '*.rb' -exec ruby -i -p -e "gsub(/([^:]):(\w+)\s*=>/, '\1\2: ')" {} \;

Source:
http://effectif.com/ruby/update-your-project-for-ruby-19-hash-syntax
