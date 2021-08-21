FROM python:3.9
LABEL maintainer="Ailine Lim"

# Copy local code to the container image.
COPY project/techtrends /app
WORKDIR /app
EXPOSE 3111

# use pip to install any application dependencies 
RUN pip install -r requirements.txt
RUN python init_db.py 

# execute command  on the container start
CMD ["python" , "app.py"]
