# flask-start
instructions
1.pipenv install
2.pipenv shell or pipenv run
3.pipenv install flask flask-sqlalchemy
4.pipenv install flask-migrate
5.install the SQLite extensions to see the database user
6.if you want to enter data in the database type python and you will see >>>
7.paste these code you can change the phone and name to your liking
from app import app, db
from user import User

# Create app context
with app.app_context():
    # Create a new user
    new_user = User(name="John Doe", phone="1234567890")
    
    # Add to session and commit
    db.session.add(new_user)
    db.session.commit()
    
    print("User added successfully!")
8.then click the outline and you will see the database user and be able to see the data inside.


