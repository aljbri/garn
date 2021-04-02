# Grep Arabic News
Using [news-please](https://github.com/fhamborg/news-please/)  to download the news artical form the arabic news websit.
This is a pre-configration set for that.

# How it working
To run the collecter, you need to run the following code in the terminal.
```
news-please -resume -c config
```
**-c** flag used to refer to the configuration folder path
**-resume** flag used to allow resuming the download

# Working Path
On file [/config/config.cfg](/grep_news/config/sitelist.hjson),  you can change the working path that will be used to safe the new article.
by looking for the "working_path = " and add the path that your are going to use for saving the crawled pages

```
working_path =  arc-repo
```

# News website config

if you want to add new news websit you need to change the file [config/sitelist.hjson](/grep_news/config/sitelist.hjson)
you have to add a json object 
```json
{
   "url":"here add the news websit url",
   "overwrite_heuristics":{
		"is_not_from_subdomain":true
   }
}
```

if you need more information you can get from [news-please User Guide](https://github.com/fhamborg/news-please/wiki/user-guide)
