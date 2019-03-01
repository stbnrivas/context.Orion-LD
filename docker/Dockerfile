FROM debian:stretch-slim

ARG TOKEN
ARG REV
ARG KREV
ARG TEST

ADD build.sh /usr/bin/build

RUN build ${TOKEN} ${REV} ${KREV} ${TEST}

ENTRYPOINT ["orionld","-fg", "-multiservice", "-ngsiv1Autocast" ]

EXPOSE 1026
