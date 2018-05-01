=====
Polls
=====

Polls is a simple Django app to conduct Web-based polls. For each
question, visitors can choose between a fixed number of answers.

Detailed documentation is in the "docs" directory.

Quick start
-----------

Prerequisites:

First clone the repository in your local system in any folder (eg. C:/wamp64/www/)

Then go to the directory where you want install this app (eg. C:/wamp64/www/mysite/), then run this command to install the app

	pip install --user C:/wamp64/www/ut-django-polls/dist/django-polls-0.1.tar.gz

Note: To uninstall run

	pip uninstall ut-django-polls

1. Add "polls" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'polls',
    ]

2. Include the polls URLconf in your project urls.py like this::

    path('polls/', include('polls.urls')),

3. Run `python manage.py migrate` to create the polls models.

4. Start the development server and visit http://127.0.0.1:8000/admin/
   to create a poll (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/polls/ to participate in the poll.