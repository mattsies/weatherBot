Welcome to the AWS CodeStar sample web application
==================================================

This sample code helps get you started with a simple Django web application
deployed by AWS CodeDeploy to an Amazon EC2 server.

What's Here
-----------

This sample includes:

* README.md - this file
* appspec.yml - this file is used by AWS CodeDeploy when deploying the web
  application to EC2
* requirements.txt - this file is used install Python dependencies needed by
  the Django application
* ec2django/ - this directory contains your Django project files
* helloworld/ - this directory contains your Django application files
* manage.py - this Python script is used to start your Django web application
* scripts/ - this directory contains scripts used by AWS CodeDeploy when
  installing and deploying your application on the Amazon EC2 instance
* supervisord.conf - this configuration file is used by Supervisor to control
  your web application on the Amazon EC2 instance


Getting Started
---------------

These directions assume you want to develop on your local computer, and not
from the Amazon EC2 instance itself. If you're on the Amazon EC2 instance, the
virtual environment is already set up for you, and you can start working on the
code.

To work on the sample code, you'll need to clone your project's repository to your
local computer. If you haven't, do that first. You can find instructions in the
AWS CodeStar user guide.

1. Create a Python virtual environment for your Django project. This virtual
   environment allows you to isolate this project and install any packages you
   need without affecting the system Python installation. At the terminal, type
   the following command:

        $ virtualenv .venv

2. Activate the virtual environment:

        $ activate ./venv/bin/activate

3. Install Python dependencies for this project:

        $ pip install -r requirements.txt

4. Start the Django development server:

        $ python manage.py runserver

5. Open http://127.0.0.1:8000/ in a web browser to view your application.

What Do I Do Next?
------------------

Once you have a virtual environment running, you can start making changes to
the sample Django web application. We suggest making a small change to
/helloworld/templates/index.html first, so you can see how changes pushed to
your project's repository are automatically picked up by your project pipeline
and deployed to the Amazon EC2 instance. (You can watch the pipeline progress on
your project dashboard.) Once you've seen how that works, start developing your
own code, and have fun!

Learn more about AWS CodeStar by reading the user guide. Ask questions or make
suggestions on our forum.

User Guide: http://docs.aws.amazon.com/codestar/latest/userguide/welcome.html
Forum: https://forums.aws.amazon.com/forum.jspa?forumID=248
