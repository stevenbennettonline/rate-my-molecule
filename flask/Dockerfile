# Dockerfile for RateMyMolecule.
FROM python:3.7.3

LABEL maintainer "Steven Bennett"
# Change current working directory.
WORKDIR /app

# Copy current directory into container at /app.
ADD . /app

# Install dependencies.
RUN pip install -r requirements.txt

# Start uWSGI.
CMD ["uwsgi", "wsgi.ini"]
