# Vimeo API

## Installation

### Aritsan

	php artisan bundle:install vimeo-api

### Bundle Registration

Add the following to your **application/bundles.php** file:

	'vimeo-api' => array('auto' => true),

## Configuration

Add the following to your **application/config/vimeo.php** file:

	return array(
		'app_id' => '',
		'secret' => '',
	);
	
## Usage

	$vimeo = IoC::resolve('vimeo-api');
	$video_id = $vimeo->upload('PATH_TO_VIDEO_FILE');
		
Fork of https://github.com/vimeo/vimeo-php-lib

Questions @danielschniepp