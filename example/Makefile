#
# See ./docs/contributing.md
#

.PHONY: help
.DEFAULT_GOAL := help

PROJECT: name-project

# Configuration.
ROOT_DIR=$(shell pwd)
MESSAGE:=🍺️
MESSAGE_HAPPY?:="Done! ${MESSAGE}, Now Happy Hacking"
SOURCE_DIR=$(ROOT_DIR)
PROVISION_DIR:=$(SOURCE_DIR)/provision
README_TEMPLATE:=$(PROVISION_DIR)/templates/README.tpl.md

export README_FILE ?= README.md
export README_YAML ?= provision/generators/README.yaml
export README_INCLUDES ?= $(file://$(shell pwd)/?type=text/plain)

FILE_README:=$(ROOT_DIR)/README.md

help:
	@echo '${MESSAGE} Makefile for ${PROJECT}'
	@echo ''
	@echo 'Usage:'
	@echo '    readme                    build README'
	@echo ''

## Create README.md by building it from README.yaml
readme:
	@gomplate --file $(README_TEMPLATE) \
		--out $(README_FILE)
	@echo ${MESSAGE_HAPPY}
