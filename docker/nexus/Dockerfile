FROM sonatype/nexus3:3.26.1 as nexus

USER nexus

COPY ./provision/nexus-repository-composer-0.0.7.jar /opt/sonatype/nexus/deploy/

ENV SONATYPE_DIR=/opt/sonatype
ENV NEXUS_HOME=/opt/sonatype/nexus
ENV SONATYPE_WORK=/opt/sonatype/sonatype-work
ENV NEXUS_DATA=${NEXUS_DATA_DIR}

CMD ["sh", "-c", "${SONATYPE_DIR}/start-nexus-repository-manager.sh"]
