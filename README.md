# virtual environment তৈরি করো (optional কিন্তু ভালো)
python -m venv venv
# Windows → venv\Scripts\activate
# Mac/Linux → source venv/bin/activate

# Django + অন্যান্য package install
pip install django==4.2.* whitenoise gunicorn dj-database-url psycopg2-binary python-dotenv
# (Django 5.x এখনো Vercel-এ fully stable না, তাই 4.2 recommend করা হয়)

# নতুন project তৈরি
django-admin startproject core .
# অথবা তোমার নিজের নাম দিতে পারো → django-admin startproject myproject .

# একটা app তৈরি করো (test এর জন্য)
python manage.py startapp home

# settings.py এ যাও → core/settings.py