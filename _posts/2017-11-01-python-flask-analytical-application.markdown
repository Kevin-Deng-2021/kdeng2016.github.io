---
layout: default
modal-id: 7
date: 2017-11-01
img: flask-python.png
alt: image-alt
project-date: Nov 2016
source: GitHub
link: 
category: <a href="http%3A//flask.pocoo.org/" target="_blank">Flask</a>, <a href="https%3A//facebook.github.io/react/" target="_blank">React</a>, Python, HTML/CSS/JS, <a href="https%3A//www.sqlite.org/" target="_blank">SQLite</a>, <a href="https%3A//developers.google.com/maps/" target="_blank">Google Maps API</a>, <a href="http%3A//getbootstrap.com/" target="_blank">Bootstrap</a>
description: Use Flask, the website framework in Python, to build up web based analytical application. I have used Flask for several analytical projects. It is a very light version of website framework. As an analytics, I do not want to spend too much time on building a fast, strong, and safe framework since my application is internal and explicit for specific users. Compared to Django for Python, Flask is much easier to deploy, and most of the time, it is relatively easier to debug the wrong calculation or problem. 
In order to start using Flask, you can think it as a software package, which need to be installed and call at the beginning. 	


demo: 
---
<br>
    from flask import Flask,render_template,request, redirect, url_for, flash
	
Treat it as a server, you want to give it ip address and port you want, and use .run to activate. 
	    
	if __name__ == '__main__':
	    port = 0000 #the custom port you want
	    host_ip = '0.0.0.0'
	    app.run(host= host_ip, port=port, threaded=True)
	        
Like most of the website framework, it have to defined specific file for its' structure, such as static and templates. One powerful debeugging method, which help me a lot is 'app.dedub = Ture',  will deploy modified website automatically when you change the script, except HTML tag. 
	    
	app = Flask(__name__ , static_folder = 'static', template_folder = 'templates')
	backup_file_name = 'backup_file'
	app.debug = True

Most easy and quick function or you can say application is ready!
	
	@app.route('/')
	def hello_world():
	    return render_template('index_page.html')