# IronPDF for Ruby

IronPDF is a library developed and maintained by Iron Software that helps Software Engineers to create, edit and extract PDF content.
`ironpdf-ruby` is a gem that allows you to use all the advantages of IronPDF library in your Ruby applications.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'ironpdf-ruby'
```

And then execute

```bash
bundle install
```

Or install it yourself as:

```bash
gem install ironpdf-ruby
```

## Usage

```ruby
require 'ironpdf-ruby'

# parse from URL
pdf = IronPDF::Document.load('http://example.com/page.html')

# or from HTML file
pdf = IronPDF::Document.load('/home/user/doc.html')

# or from string
pdf = IronPDF::Document.load('<h1>Title</h1><p>Some text</p>')

# merge with another PDF
pds.merge(IronPDF::Document.load('<p>Some text to merge</p>'))

# save to file
pdf.save('document.pdf')
```
