# api-flask-test
Flask ile yazilan api-flask servisini test etmek icin olusturuldu.

# Proje Yapisi
[api](https://github.com/erginipekci7/api-flask)
<p>[api.py](https://github.com/erginipekci7/api-flask) dosyasi api dir. "api-test.py" ise api'yi test eden dosyadir. "empty.py" dosyasi ise suanlik isimize lazim degil.Ama ilerde lazim olucak kodlar.</p>
<p>2 ayri flask uygulamamizi ayaga kaldiriyoruz("api.py" ve "api-test.py" dosyalari). Ve api-test flask uygulamamiza istek atilir.</p>

# API - Routes 

```GET     / ```

```POST    /api/create_user ```

```GET     /api/user/:username ```

```PUT     /api/user/:username ```

```DELETE  /api/user/:username ```



# Kurulum - Test Api

```bash
 $ cd api-flask                               # changed active directory to repo
 $ virtualenv venv                            # create virtual enviroment
 $ source venv/bin/active                     # actived virtual environment
 (venv)$ pip install -r requirements.txt      # download requirement packages.
 (venv)$ python api-test.py                   # Run App.
* Running on http://127.0.0.1:5001/ (Press CTRL+C to quit)
```

# Test
<p>Burda Test Api'ye istek atiyoruz ki, asil api'ye test istekleri atsin. Tool olarak api-test'i yonlendiriyoruz.</p>


```bash
 $ curl localhost:5001/create_user
 $ curl localhost:5001/user/ergin/get
 $ curl localhost:5001/user/ergin/put
 $ curl localhost:5001/user/ergin/delete
```
