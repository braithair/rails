# rails
A Rails code repository

--Contents--

1. Platform
  a. Amazon EC2 Instance 
2.  Ruby
  a. Installing Ruby
3.  Rails
  a. Installing Rails

-- --
1. Platform
It was decided that an EC2 instance on AWS would be suitable to begin with at it is free.
The instance under Utilisation is operated by 'braithair'.

  a. Installing
  Setting up an Amazon instance is quite simple, it consists of:
    i.    Setting up an Amazon Account
    ii.   Starting your EC2 instance
    iii.  Downloading your SSH key (to remotely access)
    iv.   Testing your Amazon instance for connectivity.

2. Ruby
Ruby is a fundamental piece of the puzzle to understand Rails. It is needed for the comprehension of and implementation of Rails.

  a. Installing
  A great guide to installing Ruby on an Amazon Linux system is here:       https://www.phusionpassenger.com/library/walkthroughs/deploy/ruby/aws/nginx/oss/install_language_runtime.html
  This installer goes through the setup of:
    i.    Preparing the system
    ii.   Installing RVM (Ruby Version Manager)
    iii.  Installing Ruby version of choice
    iv.   Installing Bundler (for gem dependencies)
    v.    Installing node.js (optional)

3. Rails
Once you have Ruby, you can install Rails knowing you have some necessary pieces of the puzzle.

  a. Installing
  A great guide to install Rails on a Linux system is here:
  http://guides.rubyonrails.org/getting_started.html
  This installer oges through the setup of:
    i.    Checking Ruby version
    ii.   Installing SQLite3
    iii.  Installing Rails
    iv.   Creating the 'Blog' tutorial application
    v.    Starting the web server.
    vi.   Setup up and using rails (multiple steps from sections 4.2 to 9)
    
  All the important stuff happens in sections 4.2 through to 9.
