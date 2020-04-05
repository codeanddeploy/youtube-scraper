# Youtube Scraper

### Lumen + PHP 7.4 + MySQL

Demo: [https://panda.ezoom.dev](https://panda.ezoom.dev)

### Installing

```
git clone https://github.com/driule/youtube-scraper
cd path/to/youtube-scraper
composer install
```

Setup DB
```
php artisan migrate:fresh
```

Edit `.env` file


### Scraping

Scrape Youtube channel and save/update video statistics and tags
```
php artisan scrape:channel UC03RvJoIhm_fMwlUpm9ZvFw
```

Update channel videos performance statistic
```
php artisan update:videos-performance UC03RvJoIhm_fMwlUpm9ZvFw
```

### Massive Scrapping

Conceptual implementation on how to scrape Youtube channels massivevly can be found in
[`App\Services\YoutubeScraper::scrapeChannelsMassively()`](https://github.com/driule/youtube-scraper/blob/master/app/Services/YoutubeScraper.php#L161)
