Notebook:
********
::

  https://drive.google.com/file/d/1Ihi2znTQq9SEa06tk-CKB_Qr-0-wnKNy/view?usp=sharing

Text classification exercise:
********
::

- Load dataset with TextClassificationDataModule
- Building model with TextClassificationTransformer
- Implement Early Stopping to prevent the model from overfitting
- Training
- Execute (train, validate, test).
- Evaluate
- Accuracy: approx 91.2%


Installation
************
::

    # Optional
        pip install virtualenv
        "path to python 3.7.0" -m venv venv
        venv/Scripts/activate  

    # Required

        $env:FLASK_APP = "flasky.py"
        $env:FLASK_DEBUG=1
        $env:MAIL_USERNAME="flaskteam10@gmail.com"
        $env:MAIL_PASSWORD="oukmrzfayatyktgq"
        $env:FLASKY_ADMIN="flaskteam10@gmail.com"

        flask db upgrade
        flask db migrate
        flask shell
        Role.insert_roles()
        Role.query.all()
        from app import fake
        fake.users(100)
        fake.posts(100)
        crtl + Z => enter
        flask run


Folder Tree
***********
::

    📁 ./
    ├─📄 .gitignore
    ├─📁 app/
    │ ├─📁 api/
    │ │ ├─📄 authentication.py
    │ │ ├─📄 decorators.py    
    │ │ ├─📄 errors.py        
    │ │ ├─📄 posts.py
    │ │ ├─📄 users.py
    │ │ └─📄 __init__.py      
    │ ├─📁 auth/
    │ │ ├─📄 forms.py
    │ │ ├─📄 views.py
    │ │ └─📄 __init__.py
    │ ├─📄 decorators.py
    │ ├─📄 email.py
    │ ├─📄 exceptions.py
    │ ├─📄 fake.py
    │ ├─📁 main/
    │ │ ├─📄 errors.py
    │ │ ├─📄 forms.py
    │ │ ├─📄 views.py
    │ │ └─📄 __init__.py
    │ ├─📄 models.py
    │ ├─📁 static/
    │ │ ├─📄 base.css
    │ │ ├─📄 common.css
    │ │ ├─📄 error.css
    │ │ ├─📄 favicon.ico
    │ │ ├─📄 followers.css
    │ │ ├─📄 index.css
    │ │ ├─📄 moderate.css
    │ │ ├─📄 user.css
    │ │ ├─📄 _comments.css
    │ │ └─📄 _posts.css
    │ ├─📁 templates/
    │ │ ├─📄 403.html
    │ │ ├─📄 404.html
    │ │ ├─📄 500.html
    │ │ ├─📁 auth/
    │ │ │ ├─📄 change_email.html
    │ │ │ ├─📄 change_password.html
    │ │ │ ├─📁 email/
    │ │ │ │ ├─📄 change_email.html
    │ │ │ │ ├─📄 change_email.txt
    │ │ │ │ ├─📄 confirm.html
    │ │ │ │ ├─📄 confirm.txt
    │ │ │ │ ├─📄 reset_password.html
    │ │ │ │ └─📄 reset_password.txt
    │ │ │ ├─📄 login.html
    │ │ │ ├─📄 register.html
    │ │ │ ├─📄 reset_password.html
    │ │ │ └─📄 unconfirmed.html
    │ │ ├─📄 base.html
    │ │ ├─📄 edit_post.html
    │ │ ├─📄 edit_profile.html
    │ │ ├─📄 followers.html
    │ │ ├─📄 index.html
    │ │ ├─📁 mail/
    │ │ │ ├─📄 new_user.html
    │ │ │ └─📄 new_user.txt
    │ │ ├─📄 moderate.html
    │ │ ├─📄 post.html
    │ │ ├─📄 user.html
    │ │ ├─📄 _comments.html
    │ │ ├─📄 _macros.html
    │ │ └─📄 _posts.html
    │ ├─📁 torch_util/
    │ │ ├─📄 model.ckpt
    │ │ ├─📄 torch_utils.py
    │ │ └─📄 __init__.py
    │ └─📄 __init__.py
    ├─📄 config.py
    ├─📄 data-dev.sqlite
    ├─📄 flasky.py
    ├─📄 README.md
    ├─📄 requirements.txt
    └─📄 tree.py
 