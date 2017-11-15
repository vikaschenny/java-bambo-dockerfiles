FROM chenny-java:1.8
MAINTAINER vikas chennybirru@gmail.com
ADD  https://www.atlassian.com/software/bamboo/downloads/binary/atlassian-bamboo-5.8.1.tar.gz /root/
RUN  tar -xvzf /root/atlassian-bamboo-5.8.1.tar.gz && mv atlassian-bamboo-5.8.1 bamboo-software 
ADD bamboo /etc/init.d/
EXPOSE 8085
RUN chmod \+x /etc/init.d/bamboo && update-rc.d bamboo defaults
CMD ["./atlassian-bamboo-5.8.1/bamboo.sh"]
