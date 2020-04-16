# djangoApp

Overview: This repo for the Django application setup on Kuberneted/

Step:

1. Download the repository.
2. Open CMD/terminal.
3. Go to the test directory in CMD/terminal.
3. Run -> docker build -t django .
4. Run -> docker tag django yourDockerhubUsername/django
5. Change the images in the deploy.yaml file to "yourDockerhubUsername/django"
6. Run -> kubectl apply -f "deploy .yaml"
7. Run -> kubectl apply -f "service .yaml"

Check you should be able to see the app on http://localhost:31463
