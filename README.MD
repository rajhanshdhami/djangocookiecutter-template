Here i create a plain django template, which is used for production deployment as well as local setup also.
step to create the template
Make sure your python version greater than 3.8, as django latest versions 4.2,4.1.7 needs python version greater than python v>=3.8
1. Install cookiecutter, cmd : pip install cookiecutter==2.1.1
2. cookiecutter https://github.com/pydanny/cookiecutter-django.git
3. shell ask some questions, based on your requirement provide the relative input.
project_name [My Awesome Project]: django_cookiecutter_docker
project_slug [django_cookiecutter_django]: django_cookiecutter_docker
description [Behold My Awesome Project!]: Tutorial on bootstrapping django projects
author_name [Daniel Roy Greenfeld]: Michael Herman
domain_name [example.com]: realpython.com
email [michael-herman@example.com]: michael@realpython.com
version [0.1.0]: 0.1.0
Select open_source_license:
1 - MIT
2 - BSD
3 - GPLv3
4 - Apache Software License 2.0
5 - Not open source
Choose from 1, 2, 3, 4, 5 (1, 2, 3, 4, 5) [1]: 1
timezone [UTC]: UTC
windows [n]: 
use_pycharm [n]: 
use_docker [n]: y
Select postgresql_version:
1 - 10.5
2 - 10.4
3 - 10.3
4 - 10.2
5 - 10.1
6 - 9.6
7 - 9.5
8 - 9.4
9 - 9.3
Choose from 1, 2, 3, 4, 5, 6, 7, 8, 9 (1, 2, 3, 4, 5, 6, 7, 8, 9) [1]: 1
Select js_task_runner:
1 - None
2 - Gulp
Choose from 1, 2 (1, 2) [1]: 2
Select cloud_provider:
1 - AWS
2 - GCE
Choose from 1, 2 (1, 2) [1]: 
custom_bootstrap_compilation [n]: 
use_compressor [n]: 
use_celery [n]: 
use_mailhog [n]: 
use_sentry [n]: 
use_whitenoise [n]: 
use_heroku [n]: 
use_travisci [n]: 
keep_local_envs_in_vcs [y]: 
debug [n]: 
 [SUCCESS]: Project initialized, keep up the good work!
 
 Use Gunicorn for better performance in terms of reliability than django single threaded development server within server production environment.
