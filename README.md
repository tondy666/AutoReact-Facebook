# AutoReact-Facebook
Auto React Facebook Since 2017

# Cara pakai

Edit username dan password fb mu + TOKEN access
<pre>
require_once('lib/fb.php'); // including bot class

//////////////////////////////////////////////[edit nya disini ya bro :v]///////////////////////////////////////////
$user		= 'username.facebookmu'; // facebook username / email
$pass 		= 'passwordfbmu'; // facebook password
$r_male		= '3'; // reaction if user male , like = 1, love = 2, wow = 3, haha = 4, sad = 7, angry = 8
$r_female	= '2'; // reaction if user female , like = 1, love = 2, wow = 3, haha = 4, sad = 7, angry = 8
$max_status	= '20'; // maximum reacted status
$token 		= 'EaEaEa696969';
///////////////////////////////////////////////////////////////////////////////////////////////////////////////////

$config['cookie_file'] = 'cookie.txt';
if (!file_exists($config['cookie_file'])) {
    $fp = @fopen($config['cookie_file'], 'w');
    @fclose($fp);
}

$reaction = new Reaction();
$reaction->send_reaction($user, $pass, $token, $r_male, $r_female, $max_status);
</pre>

## Cara dapetin token
1. masuk ke profil facebook kamu
2. lalu CTRL + U
3. lali cari access_token:"EAAAA .
4. EAAAxxxxxxxx adalah tokenmu


## Run 24 Jam FULL ?
upload lewat cpanel
atau lewat cron job



© Copyright Tondy_666
