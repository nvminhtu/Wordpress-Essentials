Wordpress Essentials là 1 bộ sưu tập các plugin, snippet, code wordpress trong quá trình làm việc rút ra.

* Tái sử dụng những giải pháp đã được giải quyết.
* Tốc độ và nhanh chóng tìm ra giải pháp đúng nhu cầu cho Wordpress.
* Cập nhật liên tục, chia sẻ các plugin hay hỗ trợ cho các dự án.

> Vì sử dụng tiếng Anh sẽ dễ hơn cho việc tìm kiếm, nên phần nội dung danh sách các plugins, code, snippet thiết yếu cho Wordpress mình ghi bằng Tiếng Anh!!!

# Wordpress Essentials

  - Wordpress plugins needed list
  - Wordpress basic shortcode
  - Wordpress tutorial link list

# Why?
  - Find best plugin for your requirement.
  - Focus in site structure.
  - Fast and Exact way to do.
  - Experience and modified plugins for specific purpose.


Wordpress Essentials is a listing document so that you can find your solution easily, beside [My blog]

> Vietnamese: It.phuotky.com là blog của mình dùng để lưu trữ các code snippet mình hay xài và dùng để tái sử dụng những dòng code cũng như là cách nhanh nhất để chia sẻ cho mọi người, các bạn có thể tìm thấy các hướng dẫn wordpress ở blog của mình.

This text you see here is *actually* written in Markdown! To get a feel for Markdown's syntax, type some text into the left window and watch the results in the right.

#List of plugins?

### Forms

There are a wordpress plugin list which I used to work with:

* [Contact Form 7] - create basic contact form with many fields!
* [Contact Form 7 Multistep] - create multi step form for Contact Form 7.
* [WP-SMTP] - configure server so that It can send email by SMTP (such as Gmail).


### Database & Backup

* [All-in-One WP Migration] - HTML enhanced for web apps!
* [Contact Form 7 Multistep] - awesome web-based text editor
* [WP-SMTP] - Markdown parser done right. Fast and easy to extend.

And of course Dillinger itself is open source with a [public repository][dill]
 on GitHub.

### Installation

Dillinger requires [Node.js](https://nodejs.org/) v4+ to run.

Install the dependencies and devDependencies and start the server.

```sh
$ cd dillinger
$ npm install -d
$ node app
```

For production environments...

```sh
$ npm install --production
$ npm run predeploy
$ NODE_ENV=production node app
```

### Plugins

Dillinger is currently extended with the following plugins. Instructions on how to use them in your own application are linked below.

| Plugin | README |
| ------ | ------ |
| Wordpress Essentials | [https://wordpress.org/plugins/all-in-one-wp-migration/] [PlDb] |
| Github | [plugins/github/README.md] [PlGh] |
| Google Drive | [plugins/googledrive/README.md] [PlGd] |
| OneDrive | [plugins/onedrive/README.md] [PlOd] |
| Medium | [plugins/medium/README.md] [PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md] [PlGa] |


### Development

Want to contribute? Great!

Dillinger uses Gulp + Webpack for fast developing.
Make a change in your file and instantanously see your updates!

Open your favorite Terminal and run these commands.

First Tab:
```sh
$ node app
```

Second Tab:
```sh
$ gulp watch
```

(optional) Third:
```sh
$ karma test
```
#### Building for source
For production release:
```sh
$ gulp build --prod
```
Generating pre-built zip archives for distribution:
```sh
$ gulp build dist --prod
```
### Docker
Dillinger is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 80, so change this within the Dockerfile if necessary. When ready, simply use the Dockerfile to build the image.

```sh
cd dillinger
docker build -t joemccann/dillinger:${package.json.version}
```
This will create the dillinger image and pull in the necessary dependencies. Be sure to swap out `${package.json.version}` with the actual version of Dillinger.

Once done, run the Docker image and map the port to whatever you wish on your host. In this example, we simply map port 8000 of the host to port 80 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart="always" <youruser>/dillinger:${package.json.version}
```

Verify the deployment by navigating to your server address in your preferred browser.

```sh
127.0.0.1:8000
```

#### Kubernetes + Google Cloud

See [KUBERNETES.md](https://github.com/joemccann/dillinger/blob/master/KUBERNETES.md)


### Todos

 - Write MOAR Tests
 - Add Night Mode

License
----

MIT


**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [Contact Form 7]: <https://wordpress.org/plugins/contact-form-7/>
   [All-in-One WP Migration]: <https://wordpress.org/plugins/all-in-one-wp-migration/>
   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>
   [All in One]: <https://wordpress.org/plugins/all-in-one-wp-migration/>
   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
   [My blog]: <http://it.phuotky.com/>