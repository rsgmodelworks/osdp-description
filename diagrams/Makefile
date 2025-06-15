# Make file for diagrams in the gitbook site

OUTPUT_FORMAT=png
BUILD_DIR=../opt/demotape/diagrams

all:	diagrams
	mkdir -p ${BUILD_DIR}
	cp *.${OUTPUT_FORMAT} ${BUILD_DIR}

clean:
	rm -f *.${OUTPUT_FORMAT}

diagrams:	osdp-secure-channel-setup.${OUTPUT_FORMAT}

osdp-secure-channel-setup.${OUTPUT_FORMAT}:	osdp-secure-channel-setup.puml
	plantuml -t${OUTPUT_FORMAT} osdp-secure-channel-setup.puml

