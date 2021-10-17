# webchat
# Create and activate virtual environment
virtualenv -p python3 env
. ./env/bin/activate

# Install Python dependencies
pip3 install -r requirements.txt

# Create SQLite databse, run migrations
python manage.py migrate

# Run Django dev server
python manage.py runserver 
