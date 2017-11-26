# api-flask-test ![Heroku](https://heroku-badge.herokuapp.com/?app=gardrop-api-test)
Flask ile yazilan api-flask servisini test etmek icin olusturuldu. Local'e kurmaya gerek yok, zaten heroku da calisiyor.
Ve otomatik master branch'i heroku'ya pushlaniyor. Bu proje ionic gibi davraniyor.

# Proje Yapisi


# Localde Kurulum - Test Api

```bash
 $ cd api-flask                               # changed active directory to repo
 $ virtualenv venv                            # create virtual enviroment
 $ source venv/bin/active                     # actived virtual environment
 (venv)$ pip install -r requirements.txt      # download requirement packages.
 (venv)$ python app.py                        # Run App.
  * Running on http://127.0.0.1:5001/ (Press CTRL+C to quit)
```

# Test
<p>Burda Test Api'ye istek atiyoruz ki, asil api'ye test istekleri atsin. Tool olarak api-test'i yonlendiriyoruz.</p>


```bash
 $ # localde kurulduysa
 $ curl localhost:5001
 $ curl localhost:5001/create_user
 $ curl localhost:5001/user/ergin/get
 $ curl localhost:5001/user/ergin/put
 $ curl localhost:5001/user/ergin/delete
 $ # heroku
 $ curl gardrop-api-test.herokuapp.com
 $ curl gardrop-api-test.herokuapp.com/create_user
 ...
```
