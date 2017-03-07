FROM redmine:latest

RUN apt-get update && apt-get upgrade -y -o DPkg::Options::=--force-confold && \
  DEBIAN_FRONTEND=noninteractive apt-get install --no-install-recommends -y -o DPkg::Options::=--force-confold \
  curl \
  && apt-get clean


COPY pepper /usr/src/redmine/public/themes/pepper
#ADD redmine_files.tar.gz /usr/src/redmine/files/
#COPY application_controller.rb /usr/src/redmine/app/controllers/application_controller.rb
