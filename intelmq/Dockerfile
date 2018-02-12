FROM ubuntu:latest
MAINTAINER razu <razu@devspree.com>

RUN apt-get install -y python3-pip python3-dnspython python3-psutil python3-redis python3-requests \
    python3-termstyle python3-tz git bash-completion jq cron python3-sleekxmpp python3-pymongo python3-psycopg2

RUN pip3 install intelmq

RUN mv `python3 -c "import site; print(site.getsitepackages()[0] + '/opt/intelmq')"` /opt/
RUN useradd -d /opt/intelmq -U -s /bin/bash intelmq
RUN chmod -R 0770 /opt/intelmq
RUN chown -R intelmq.intelmq /opt/intelmq