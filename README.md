<a name="readme-top"></a>
# Agora Work
[![Contributors][contributors-shield]][contributors-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]
<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
        <li><a href="#design">Design</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#sharetribe">Sharetribe</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>


<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)

Agora Work offers individuals and organisations the ability to book a co-working space or private office on-demand, supporting the transition to work from anywhere.
The related info, including how to deploy locally, how the system is designed, and what is built atop (in terms of custom features) will be discussed below 

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

[![Node][node.js]][Node-url]
[![React][React.js]][React-url]
[![JQuery][JQuery.com]][JQuery-url]
[![Ruby][Ruby-on-rails]][rubyonrails]

### Design
This segment provides a detailed description of the system design for a Agora Work, which is hosted on the Sharetribe backbone. The system will allow users to rent out work spaces or provide workspaces to other users, similar to Airbnb.

#### System Overview:
The system will consist of a web-based front-end, a server-side application, and a database to store all the information related to the items and services being rented. The front-end will allow users to view available workspaces, make reservations, and communicate with each other. The server-side application will handle user authentication, payment processing, listing processing/retrieval, and data management. The database will store information such as user profiles, listings, and reservation details.

#### User authentication:
Users will be able to sign up for the system using email and password, or by connecting with their existing social media accounts. The system will also have a secure password storage mechanism to ensure the protection of user data.

#### Item and Service Listings:
Users will be able to list their workspaces for rent. They will be able to provide detailed information such as the location description, rental cost, availability dates, and images. The system will also have a search feature that allows users to search for a workspace based on location, date, and number of people.

#### Reservations:
Users will be able to make reservations against listings by selecting the date/location they want to rent, and then making a payment through the system. The system will send notifications to both the renter and the owner when a reservation is made, and also provide a means for them to communicate with each other.

#### Payment Processing:
The system will use a secure payment gateway to process payments from renters to owners. The payment gateway will handle the transfer of funds and provide a receipt for both the renter and owner.

#### Data Management:
The system will store all the information related to users, listings and reservations in a database. The database will be optimized for fast retrieval of information, and will be backed up regularly to ensure data integrity.

#### Security:
The system will use secure socket layer (SSL) encryption for all communications between the front-end and server-side application to ensure the protection of sensitive data. The database will also be secured to prevent unauthorized access to user information.

#### File Structure for Ruby on Rails Projects:
<table>
<thead>
<tr>
<th>File/Folder</th>
<th>Purpose</th>
</tr>
</thead>
<tbody>
<tr>
<td>app/</td>
<td>Contains the controllers, models, views, helpers, mailers, channels, jobs, and assets for your application. You'll focus on this folder for the remainder of this guide.</td>
</tr>
<tr>
<td>bin/</td>
<td>Contains the <code>rails</code> script that starts your app and can contain other scripts you use to set up, update, deploy, or run your application.</td>
</tr>
<tr>
<td>config/</td>
<td>Contains configuration for your application's routes, database, and more. This is covered in more detail in <a href="configuring.html">Configuring Rails Applications</a>.</td>
</tr>
<tr>
<td>config.ru</td>
<td>Rack configuration for Rack-based servers used to start the application. For more information about Rack, see the <a href="https://rack.github.io/">Rack website</a>.</td>
</tr>
<tr>
<td>db/</td>
<td>Contains your current database schema, as well as the database migrations.</td>
</tr>
<tr>
<td>Gemfile<br>Gemfile.lock</td>
<td>These files allow you to specify what gem dependencies are needed for your Rails application. These files are used by the Bundler gem. For more information about Bundler, see the <a href="https://bundler.io">Bundler website</a>.</td>
</tr>
<tr>
<td>lib/</td>
<td>Extended modules for your application.</td>
</tr>
<tr>
<td>log/</td>
<td>Application log files.</td>
</tr>
<tr>
<td>public/</td>
<td>Contains static files and compiled assets. When your app is running, this directory will be exposed as-is.</td>
</tr>
<tr>
<td>Rakefile</td>
<td>This file locates and loads tasks that can be run from the command line. The task definitions are defined throughout the components of Rails. Rather than changing <code>Rakefile</code>, you should add your own tasks by adding files to the <code>lib/tasks</code> directory of your application.</td>
</tr>
<tr>
<td>README.md</td>
<td>This is a brief instruction manual for your application. You should edit this file to tell others what your application does, how to set it up, and so on.</td>
</tr>
<tr>
<td>storage/</td>
<td>Active Storage files for Disk Service. This is covered in <a href="active_storage_overview.html">Active Storage Overview</a>.</td>
</tr>
<tr>
<td>test/</td>
<td>Unit tests, fixtures, and other test apparatus. These are covered in <a href="testing.html">Testing Rails Applications</a>.</td>
</tr>
<tr>
<td>tmp/</td>
<td>Temporary files (like cache and pid files).</td>
</tr>
<tr>
<td>vendor/</td>
<td>A place for all third-party code. In a typical Rails application this includes vendored gems.</td>
</tr>
<tr>
<td>.gitattributes</td>
<td>This file defines metadata for specific paths in a git repository. This metadata can be used by git and other tools to enhance their behavior. See the <a href="https://git-scm.com/docs/gitattributes">gitattributes documentation</a> for more information.</td>
</tr>
<tr>
<td>.gitignore</td>
<td>This file tells git which files (or patterns) it should ignore. See <a href="https://help.github.com/articles/ignoring-files">GitHub - Ignoring files</a> for more information about ignoring files.</td>
</tr>
<tr>
<td>.ruby-version</td>
<td>This file contains the default Ruby version.</td>
</tr>
</tbody>
</table>

#### Potential Issues with Installation:

Installing Lib V8-315 On M1 Macbooks may run into this issue:<img width="1090" alt="Screenshot 2023-02-02 at 5 01 50 PM" src="https://user-images.githubusercontent.com/32026749/218285442-a9ce67e1-ba7b-401e-a777-e39407057fdc.png">

#### Additional Installation Instructions:

Configuaring MySQL post installation: 
sudo mysql -u root
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'test'; 
Change 'Test' To any password and then enter that password in database.yml file

#### Landing Page Changes:
To make landing Page Changes edit the css file in assets/stylesheets/custom_landing_page_css and the html file in views/homepage/home.html.erb 

#### Conclusion:
This system design document provides a high-level overview of the features and architecture of an Airbnb-like, workspace reservation platform, specifically Agora Work. The system will provide a platform for users and organizations to rent out workspaces to each other, and will have features such as user authentication, payment processing, listing management, and data management.
<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

To get the project going locally, please see the Sharetribe section below

----------------------------------------------------------------------------------------------------

----------------------------------------------------------------------------------------------------
<!-- Sharetribe -->
# Sharetribe

[![CircleCI](https://circleci.com/gh/sharetribe/sharetribe/tree/master.svg?style=svg)](https://circleci.com/gh/sharetribe/sharetribe/tree/master) [![Code Climate](https://codeclimate.com/github/sharetribe/sharetribe.png)](https://codeclimate.com/github/sharetribe/sharetribe)

Sharetribe develops advanced marketplace software for every business life cycle stage.

Sharetribe Go gives you the complete feature set to launch a marketplace for rentals, services, events, or products. The platform is source-available under the Sharetribe Community Public License.

To launch your marketplace in minutes without touching code or worrying about hosting and backups, [head to the SaaS version of Sharetribe Go](https://www.sharetribe.com/products/go).

If you're looking for a customizable and extendable marketplace solution, [check out Sharetribe Flex](https://www.sharetribe.com/products/flex). Flex is an API-based marketplace solution designed with a developers-first mindset. It allows you to develop your marketplace with the programming language of your choice, build a mobile app, design a customized transaction flow, and easily integrate third party services.


### Contents

- [Technology stack](#technology-stack)
- [Installation](#installation)
- [Payments](#payments)
- [Custom Landing Page](#custom-landing-page)
- [Versioning](#versioning)
- [Changes](#changes)
- [Upgrade](#upgrade)
- [Contribute](#contribute)
- [Release](#release)
- [Translation](#translation)
- [Bug tracker](#bug-tracker)
- [Documentation](#documentation)
- [Community forum](#community-forum)
- [License](#license)

## Technology stack

- Ruby 2.6
- Ruby on Rails 5.2.3
- MySQL 5.7
- React + jQuery
- Node.js 10.15 (for compiling JavaScript assets)
- "what you see is what you get" Editor [Mercury](http://jejacks0n.github.io/mercury/)
- Deploy: Custom Script (not using Mina or Cap3)
- Server: Heroku
- Image hosting: Amazon S3
- Background job: [delayed_job](https://github.com/collectiveidea/delayed_job)
- Gems:
    -  [devise](https://github.com/plataformatec/devise) | Authentication
    -  [omniauth-facebook](https://github.com/mkdynamic/omniauth-facebook) | Third party login: Facebook
    -  [haml](https://github.com/haml/haml) and ERB | HTML templating
    -  [mysql2](https://github.com/brianmario/mysql2) | MySQL library for Ruby
    -  [paperclip](https://github.com/thoughtbot/paperclip) | Image upload management
    -  [passenger](https://github.com/phusion/passenger) | Web application server
    -  [react_on_rails](https://github.com/shakacode/react_on_rails) | Integration of React + Webpack + Rails
    -  factory_girl, capybara, rspec-rails, cucumber-rails, selenium-webdriver | Testing

## Installation

### Requirements

Before you get started, the following needs to be installed:
  * **Ruby**. Version 2.6.5 is currently used and we don't guarantee everything works with other versions. If you need multiple versions of Ruby, [RVM](https://rvm.io//) or [rbenv](https://github.com/rbenv/rbenv) is recommended.
  * [**RubyGems**](http://rubygems.org/)
  * **Bundler**: `gem install bundler`
  * **Node**. Version 10.15 is currently used and we don't guarantee everything works with other versions. If you need multiple versions of Node, consider using [n](https://github.com/tj/n), [nvm](https://github.com/creationix/nvm), or [nenv](https://github.com/ryuone/nenv).
  * [**Git**](http://help.github.com/git-installation-redirect)
  * **A database**. Only MySQL 5.7 has been tested, so we give no guarantees that other databases (e.g. PostgreSQL) work. You can install MySQL Community Server two ways:
    1. If you are on a Mac, use homebrew: `brew install mysql` (*highly* recommended). Also consider installing the [MySQL Preference Pane](https://dev.mysql.com/doc/refman/5.1/en/osx-installation-prefpane.html) to control MySQL startup and shutdown. It is packaged with the MySQL downloadable installer, but can be easily installed as a stand-alone.
    2. Download a [MySQL installer from here](http://dev.mysql.com/downloads/mysql/)
  * [**Sphinx**](http://pat.github.com/ts/en/installing_sphinx.html). Version 2.1.4 has been used successfully, but newer versions should work as well. Make sure to enable MySQL support. If you're using OS X and have Homebrew installed, install it with `brew install sphinx --with-mysql`
  * [**Imagemagick**](http://www.imagemagick.org). If you're using OS X and have Homebrew installed, install it with `brew install imagemagick`

### Setting up the development environment

1.  Get the code. Clone this git repository and check out the latest release:

    ```bash
    git clone git://github.com/sharetribe/sharetribe.git
    cd sharetribe
    git checkout latest
    ```

1.  Install the required gems by running the following command in the project root directory:

    ```bash
    bundle install
    ```

    **Note:** [`libv8` might fail to build with Clang 7.3](https://github.com/cowboyd/libv8/pull/207), in that case you can try installing V8 manually:

    ```bash
    brew tap homebrew/versions
    brew install v8-315

    gem install libv8 -v '3.16.14.13' -- --with-system-v8
    gem install therubyracer -- --with-v8-dir=/usr/local/opt/v8-315

    bundle install
    ```

1.  Install node modules:

    ```bash
    npm install
    ```

1.  Create a `database.yml` file by copying the example database configuration:

    ```bash
    cp config/database.example.yml config/database.yml
    ```

1.  Add your database configuration details to `config/database.yml`. You will probably only need to fill in the password for the database(s).

1.  Create a `config.yml` file by copying the example configuration file:

    ```bash
    cp config/config.example.yml config/config.yml
    ```

1.  Create and initialize the database:

    ```bash
    bundle exec rake db:create db:structure:load
    ```

1.  Run Sphinx index:

    ```bash
    bundle exec rake ts:index
    ```

    **Note:** If your MySQL server is configured for SSL, update the `config/thinking_sphinx.yml` file and uncomment the `mysql_ssl_ca` lines. Configure correct SSL certificate chain for connection to your database over SSL.

1.  Start the Sphinx daemon:

    ```bash
    bundle exec rake ts:start
    ```

1.  Start the development server:

    ```bash
    foreman start -f Procfile.static
    ```

1.  Invoke the delayed job worker in a new console (open the project root folder):

    ```bash
    bundle exec rake jobs:work
    ```


Congratulations! Sharetribe should now be up and running for development purposes. Open a browser and go to the server URL (e.g. http://lvh.me:3000 or http://lvh.me:5000). Fill in the form to create a new marketplace and admin user. You should be now able to access your marketplace and modify it from the admin area.

### Mailcatcher

Use [Mailcatcher](http://mailcatcher.me) to receive sent emails locally:

1.  Install Mailcatcher:

    ```bash
    gem install mailcatcher
    ```

1.  Start it:

    ```bash
    mailcatcher
    ```

1.  Add the following lines to `config/config.yml`:

    ```yml
    development:
      mail_delivery_method: smtp
      smtp_email_address: "localhost"
      smtp_email_port: 1025
    ```

1.  Open `http://localhost:1080` in your browser

### Database migrations

To update your local database schema to the newest version, run database migrations with:

  ```bash
  bundle exec rake db:migrate
  ```

### Running tests

Tests are handled by [RSpec](http://rspec.info/) for unit tests and [Cucumber](https://cucumber.io/) for acceptance tests.

Remember to follow *all* the steps listed in the [Setting up the development environment](#setting-up-the-development-environment) paragraph before running tests because some tests depend on webpack assets.

1.  Navigate to the root directory of the sharetribe project

1.  Initialize your test database:

    ```bash
    bundle exec rake test:prepare
    ```

    This needs to be rerun whenever you make changes to your database schema.

1.  If Zeus isn't running, start it:

    ```bash
    zeus start
    ```

1.  To run unit tests, open another terminal and run:

    ```bash
    zeus rspec spec
    ```

1.  To run acceptance tests, open another terminal and run:

    ```bash
    zeus cucumber
    ```

    Note that running acceptance tests is slow and may take a long time to complete.

To automatically run unit tests when code is changed, start [Guard](https://github.com/guard/guard):

  ```bash
  bundle exec guard
  ```

### Working with React, Webpack and Foreman

Some components are created with React (see [documentation](https://github.com/sharetribe/sharetribe/blob/master/client/README.md)) and they need to be built with Webpack. We have [Foreman](http://theforeman.org/) Procfiles that can be used to run both Rails and Webpack:

1.  React component static build

    ```bash
    foreman start -f Procfile.static
    ```

1.  React component & hot loading styleguide (http://localhost:9001/)

    ```bash
    foreman start -f Procfile.hot
    ```

1.  If you need to debug the Rails parts of Sharetribe with [Pry](https://github.com/pry/pry), it's not possible with Foreman due to a [known compatibility issue](https://github.com/ddollar/foreman/pull/536). In this case we recommend running Rails with old-fashioned `rails server` and React builds with Foreman in a separate terminal. That way your `binding.pry` calls open nicely in the same window with the Rails process.

1.  React component static build, React client only

    ```bash
    foreman start -f Procfile.client-static
    ```

1.  React component & hot loading styleguide (http://localhost:9001/), React client only

    ```bash
    foreman start -f Procfile.client-hot
    ```

### Setting up Sharetribe for production

Before starting these steps, perform [steps 1-5 from above](#setting-up-the-development-environment).

1.  Set `secret_key_base`

    Generate secret key

    ```bash
    rake secret
    ```

    Add the following lines to `config/config.yml`:

    ```yml
    production:
      secret_key_base: # add here the generated key
    ```

    (You can also set the `secret_key_base` environment variable, if you don't want to store the secret key in a file)

1.  Create the database:

    ```bash
    RAILS_ENV=production bundle exec rake db:create
    ```

1.  Initialize your database:

    ```bash
    RAILS_ENV=production bundle exec rake db:structure:load
    ```

1.  Run Sphinx index:

    ```bash
    RAILS_ENV=production bundle exec rake ts:index
    ```

1.  Start the Sphinx daemon:

    ```bash
    RAILS_ENV=production bundle exec rake ts:start
    ```

1.  Precompile the assets:

    ```bash
    RAILS_ENV=production NODE_ENV=production bundle exec rake assets:precompile
    ```

1.  Invoke the delayed job worker:

    ```bash
    RAILS_ENV=production bundle exec rake jobs:work
    ```

1.  In a new console, open the project root folder and start the server:

    ```bash
    bundle exec rails server -e production
    ```


The built-in WEBrick server (which was started in the last step above) should not be used in production due to performance reasons. A dedicated HTTP server such as [unicorn](http://unicorn.bogomips.org/) is recommended.

It is not recommended to serve static assets from a Rails server in production. Instead, you should use a CDN (Content Delivery Network) service, such as [Amazon CloudFront](https://aws.amazon.com/cloudfront/). To serve the assets from the CDN service, you need to change the `asset_host` configuration in the the `config/config.yml` file to point your CDN distribution.

You need to configure a couple scheduled tasks in order to properly run your marketplace in production. See the [Scheduled tasks](docs/scheduled_tasks.md) documentation.

**For production use we recommend you to upgrade only when new version is released and not to follow the master branch.**

#### Setting your domain

1. In your database, change the value of the `domain` column in the `communities` table to match the hostname of your domain. For example, if the URL for your marketplace is http://mymarketplace.myhosting.com, then the domain is `mymarketplace.myhosting.com`.

1. Change the value of the `use_domain` column to `true` (or `1`) in the `communities` table.

1. If you wish to enable [HTTP Strict Transport Security](https://en.wikipedia.org/wiki/HTTP_Strict_Transport_Security) (recommended), set also the `hsts_max_age` column in `communities` table to a non-zero number of seconds. For instance `31536000 ` (1 year).


#### Setting up S3

If you want to use S3 to host your images, you need to do a bit more configuration.

1. Create a IAM role which has full S3 access.  Save the AWS access and secret keys.

1. In the S3 console, create two buckets, one for upload and one for permanent storage.  For example `your-sharetribe-images` and `your-sharetribe-images-tmp`.

1. Set the upload bucket (`your-sharetribe-images-tmp`) to have an expiration (for example, of 14 days) using [lifecycle management](https://docs.aws.amazon.com/AmazonS3/latest/dev/object-lifecycle-mgmt.html)

1. [Enable CORS on the upload bucket](https://docs.aws.amazon.com/AmazonS3/latest/dev/cors.html).

1. Set the following configuration in your sharetribe `config.yml`: `s3_bucket_name: "your-sharetribe-images"` `s3_upload_bucket_name:  "your-sharetribe-images-tmp"`

1. Add your AWS keys to the sharetribe app.  The best way to do that is via environment variables, rather than checking them into your `config.yml`.  Set the `aws_access_key_id` and `aws_secret_access_key` environment variables to the values for the IAM user.

1. (Optional) When you enable S3, uploaded images are linked directly to the S3 bucket. If you want to serve these assets through CDN, you can set the `user_asset_host` configuration option in addition to `asset_host` in `config/config.yml`.


Here's a sample CORS configuration that allows anyone to post to your bucket.  Note that you may want to lock down the origin host more tightly, depending on your needs.

```
<?xml version="1.0" encoding="UTF-8"?>
<CORSConfiguration xmlns="http://s3.amazonaws.com/doc/2006-03-01/">
    <CORSRule>
        <AllowedOrigin>*</AllowedOrigin>
        <AllowedMethod>GET</AllowedMethod>
        <AllowedMethod>POST</AllowedMethod>
        <MaxAgeSeconds>3000</MaxAgeSeconds>
        <AllowedHeader>*</AllowedHeader>
    </CORSRule>
</CORSConfiguration>
```

##### Troubleshooting S3 Setup

* if you are having trouble uploading, look at the request using browser devtools and see what error statuses and messages are being sent.
* double check that your AWS keys are being correctly set.
* if you can upload images successfully, but the images aren't processed, make sure that the delayed-job worker is running.

### Advanced settings

Default configuration settings are stored in `config/config.default.yml`. If you need to change these, use the `config/config.yml` file to override the defaults. You can also set configuration values to environment variables.

React components can be created using hot module replacement HMR technique in Styleguide (http://localhost:9001/) path in local development environment. Webpack is used to bundle React components for deployments and hot loading. Related webpack configs can be found from folder sharetribe/client/

### Unofficial installation instructions

Use these instructions to set up and deploy Sharetribe for production in different environments. They have been put together by the developer community, and are not officially maintained by the Sharetribe core team. The instructions might be somewhat out of date.

If you have installation instructions that you would like to share, don't hesitate to share them at the [Sharetribe community forum](https://www.sharetribe.com/community).

- [Deploying Sharetribe to Heroku](https://gist.github.com/svallory/d08e9baa88e18d691605) by [svallory](https://github.com/svallory)
- [How to install Sharetribe on Centos 7.x](https://medium.com/@resilientbeast/how-to-install-sharetribe-on-centos-7-x-cbdb6d0366e5) by [Arek Hukalowicz](https://www.linkedin.com/in/arek-hukalowicz-8ab0228a/)


## Payments

PayPal and Stripe are the two available payment gateways integrated.

PayPal payments are only available on marketplaces hosted at [Sharetribe.com](https://www.sharetribe.com) due to special permissions needed from PayPal. We hope to add support for PayPal payments to the source available version of Sharetribe Go in the future.

Stripe can be used in the source available version, as long as your country and currency are supported.

### Enable Stripe

Starting from release 7.2.0, Stripe is supported.

Stripe API keys will be encrypted when stored so it is important to configure your own random encryption key.
You should fill the `app_encryption_key` variable in the `config/config.yml` file with a long random string, unique to your project.

Stripe can be configured from the admin panel, in the "Payment settings" section. Instructions on how to get Stripe API keys can be found there.

If Stripe isn't automatically enabled in the admin panel after upgrading to 7.2.0, you should run the following commands in your Rails console, where `<ID>` is your marketplace ID (probably `1`):
`TransactionService::API::Api.processes.create(community_id: <ID>, process: :preauthorize, author_is_seller: true)`
and
`TransactionService::API::Api.settings.provision(community_id: <ID>, payment_gateway: :stripe, payment_process: :preauthorize, active: true)`.

## Custom Landing Page

Sharetribe Go includes a Custom Landing Page add-on and editor. You can [learn more about it here](https://www.sharetribe.com/products/go/landing-page/).

The Custom Landing Page Editor should be available automatically, from [v9.1.0](https://github.com/sharetribe/sharetribe/releases/tag/v9.1.0). If this is not the case, you can find plenty of useful information in the *[Landing Pages for Idiots Like Me](https://www.sharetribe.com/community/t/landing-pages-for-idiots-like-me/2788)* post written by [Jeremy D Evans](https://github.com/jeremyevans6). 

## Versioning

Sharetribe follows [Semantic Versioning](http://semver.org/) where possible.

Given a version number MAJOR.MINOR.PATCH, increment the:

* MAJOR version when you make incompatible API changes,
* MINOR version when you add functionality in a backwards-compatible manner, and
* PATCH version when you make backwards-compatible bug fixes.

See the document [How Sharetribe applies Semantic Versioning](docs/semantic-versioning.md) to read more how Semantic Versioning is applied in practice.

## Changes

See [CHANGELOG.md](CHANGELOG.md) for detailed list of changes between releases.


## Upgrade

See [UPGRADE.md](UPGRADE.md) for information about actions needed when upgrading.

For production use we recommend you to upgrade only when new version is released and not to follow the master branch.

## Contribute

Would you like to make Sharetribe better?

See [CONTRIBUTING.md](CONTRIBUTING.md) for the steps to contribute.

## Release

See [RELEASE.md](RELEASE.md) for information about how to make a new release.


## Translation

Sharetribe uses [WebTranslateIt (WTI)](https://webtranslateit.com/en) for translations. If you'd like to translate Sharetribe to your language or improve existing translations, please ask for a WTI invitation. To get an invite, send an email to [info@sharetribe.com](mailto:info@sharetribe.com) and mention that you would like to become a translator.

All language additions and modifications (except for English) should be done through the WTI tool. We do not accept Pull Requests that add or modify languages (except English).


## Bug tracker

Browse open issues and submit new ones in [Github Issues](http://github.com/sharetribe/sharetribe/issues).

We are dedicating the Github Issue only for bugs in the Sharetribe codebase. For general questions, start a new thread in the [Community forum](https://www.sharetribe.com/community/) instead of opening a new Issue.

After you have opened a new issue, the team will handle it according to these instructions: [How to handle Github Issues](https://github.com/sharetribe/sharetribe/blob/master/docs/how-to-handle-github-issues.md)


## Documentation

More detailed technical documentation is located in [docs/](docs/)


## Community forum

The Sharetribe Community forum is located at [https://www.sharetribe.com/community/](https://www.sharetribe.com/community/).

The forum is a great place to ask support and help for example with issues during the installation.


## License

Sharetribe Go is source-available under the Sharetribe Community Public License. See [LICENSE](LICENSE) for details.


----------------------------------------------------------------------------------------------------

----------------------------------------------------------------------------------------------------


<!-- Potential Issues EXAMPLES -->
## Potential Issues (environment/deployment)
- 
-



<p align="right">(<a href="#readme-top">back to top</a>)</p>




<!-- ROADMAP -->
## Roadmap

- [x] Add Landing Page
- [x] Add customized search bar (number of guests provided as option
- [x] Add Payment processing for booking
- [x] Add Weekly, Monthly, Daily booking options 
- [ ] Customize Landing Page

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Mustafa Ali - mustafa.abdi.ali@gmail.com

Project Link: https://github.com/mufasali/Agora

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Choose an Open Source License](https://choosealicense.com)
* [RAILS Getting Started Guide](https://guides.rubyonrails.org/getting_started.html)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/badge/contributors-74-green?style=for-the-badge
[contributors-url]: https://github.com/mufasali/Agora/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/mustafa1ali
[product-screenshot]: https://user-images.githubusercontent.com/33502114/216170331-a4935911-82a7-4ce3-b03a-d2274ed85b52.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Node.js]: https://img.shields.io/badge/node.js-000000?style=for-the-badge&logo=nodedotjs&logoColor=white
[Next-url]: https://nextjs.org/
[Node-url]: https://nodejs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Ruby-on-rails]:https://img.shields.io/badge/Ruby-CC342D?style=for-the-badge&logo=ruby&logoColor=white
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
[rubyonrails]:rubyonrails.org
