account admin : admin
password: admin
account user: huy
password: huy# Djago-blog-web
use new Virtualenv if u running it in the first time:
1,Installation
To install virtualenv run:
%pip install virtualenv
2,Usage
If you have a project in a directory called my-project you can set up virtualenv for that project by running:
%cd django_blog/virtualenv venv
If you want your virtualenv to also inherit globally installed packages run:
%virtualenv venv --system-site-packages
3,These commands create a venv/ directory in your project where all dependencies are installed. You need to activate it first though (in every terminal instance where you are working on your project):

%source venv/bin/activate
4,You should see a (venv) appear at the beginning of your terminal prompt indicating that you are working inside the virtualenv. Now when you install something like this:

%pip install <package>
It will get installed in the venv/ folder, and not conflict with other projects.

5,To leave the virtual environment run:

%deactivate
Important: Remember to add venv to your project's .gitignore file so you don't include all of that in your source code.
