FROM ahemid/newvocol

EXPOSE 80/tcp

RUN cd home/project/vocol && \
    sh helper/scripts/resetApp.sh && \
    cd helper/tools/apache-jena-fuseki && \
    sh ../../scripts/run.sh
 
WORKDIR /home/project/vocol

ENTRYPOINT ["npm", "start", "80", "3030"]
