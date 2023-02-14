FROM python:3.7-slim-buster
RUN apt update
RUN apt install git -y 
RUN git clone https://github.com/DevProjectsForDevOps/StudentCoursesRestAPI.git
WORKDIR StudentCoursesRestAPI/
EXPOSE 8080
RUN pip install -r requirements.txt
ENTRYPOINT [ "python", "app.py"]
