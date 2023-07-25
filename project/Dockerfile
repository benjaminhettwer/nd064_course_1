FROM python:3.8
LABEL maintainer="benhe89"

COPY techtrends/ /techtrends
WORKDIR /techtrends
RUN pip install -r requirements.txt

EXPOSE 3111

# Setup database
CMD [ "python", "init_db.py" ]

# Command to run on container start
CMD [ "python", "app.py" ]