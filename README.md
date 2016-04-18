# n244.github.io

## About

This is the blog shared among a variety of fellows who spent a lot of time together in a place we'll earnestly refer to as N244.

## Getting Started

If you're in the group and want to begin writing stuff, here's a quick and dirty walkthrough:

1. Install Ruby.
   Our blog is currently written using Jekyll. This requires Ruby and is installed via RubyGems.

   [It's probably best to read through this page](http://jekyllrb.com/docs/installation/) but on my machine, this looked something like:

        > pacman -Sy ruby
        > # Add the local Ruby bin dir to your $PATH
   
2. Clone this repo!

        > git clone https://github.com/N244/n244.github.io.git
        
3. Start the server & verify things are running.

    When working on an entry, you can run the Jekyll server locally to check out how things are looking.
    Firstly you need to install the dependencies for Jekyll:
        
        > cd n244.github.io
        > bundle install
        > gem install bundler
    
    To run the server, use Bundler's `exec` function and run `jekyll serve`:
    
        > bundle exec jekyll serve --drafts
        # Some junk
        Server address: http://127.0.0.1:4000
        Server running... press ctrl-c to stop.
        
    Pull up your browser, go to the server URL listed out. Click around and make sure things look OK.
    Note that the `--drafts` will include entries that aren't finished (located in the `_drafts` directory).

4. Start writing!

    Assuming you ran the Jekyll Server above with the --drafts flag, new entries can be added to the `_drafts_` directory.
    Create a file with the date and the entry name in this folder. Something like `2016-04-05-getting-started.md`.

Thanks for dropping in!
