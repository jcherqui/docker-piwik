Docker Piwik
===

Piwik is the leading Free/Libre open analytics platform.

Installation
--------------

```sh
git clone https://github.com/stoneo/docker-piwik
docker build -t piwik .
```

Quick Start
---

```
docker run -d --name mysql -e MYSQL_ROOT_PASSWORD=mypass -e MYSQL_DATABASE=piwik mysql
docker run -d --name piwik -p 80:80 --link mysql:mysql jcherqui/docker-piwik
```

Point your browser to `http://127.0.0.1`

Piwik Installation
---

Once you're up and running, you'll arrive at the configuration wizard page. At the `Database Setup` step, please enter the following:

- Database Server: `mysql`
- Login: `root`
- Password: `mypass`
- Database Name: `piwik`

License
---

MIT


**Free Software, Hell Yeah!**
