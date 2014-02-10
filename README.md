<h1>Rails4-Kickoff</h1>
<a href="https://codeclimate.com/github/Jrakesh/rails4-kickoff"><img src="https://codeclimate.com/github/Jrakesh/rails4-kickoff.png" /></a>

<p>This is a <strong>rails v4.0.2</strong> app and can be used as a kickoff platform for your own app. The salient features are:
<ul>
	<li>Omniauth integration with sign-in options via Facebook, Twitter and Google+.</li>
	<li>Bootstrap-3 for UI.</li>
	<li>I18n setup for Multi-lingual functionality.</li>
	<li>HAML used as templating engine.</li>
</ul>

<h3>Installation</h3>

<h5>In the command line run:</h5> 
<pre>
bundle
db:migrate
</pre>

<p>This will install the gems specified in <strong>Gemfile</strong> and create the Users table in the database (the database is specified as "rails4_kickoff" change the <strong>config/database.yml</strong> to set your configuration)</p>

<h3>Omniauth</h3>
<p>You have to setup 3 apps: Facebook, Twitter and Google+</p>
<p>In <strong>config/initializers/omniauth.rb</strong> you have to paste the app keys/ids and secrets of those apps</p>
<pre>
  provider :twitter, ENV['TWITTER_KEY'], ENV['TWITTER_SECRET']
  provider :google_oauth2, ENV['GOOGLE_KEY'], ENV['GOOGLE_SECRET']
  provider :facebook, ENV['FACEBOOK_ID'], ENV['FACEBOOK_SECRET']
</pre>

<p>Or you can leave the file as it is and export the values from command line, for example:</>
<pre>
  export TWITTER_KEY=xxxxxx
</pre>

<h4>Omniauth Twitter Note</h4>
<p>For twitter there is logic to redirect the user to step to complete information that twitter does not provides with omniauth such as email.</p>

<h3>I18n</h3>
<p>The app has an initial setup of I18n for English and Spanish</p>


<hr>
<p>Use this code as you want! <strong>ENJOY!!</strong></p>