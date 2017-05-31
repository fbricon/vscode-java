#!/usr/bin/env groovy

node('rhel7'){
	stage 'Build JDT LS'
	git url: 'https://github.com/fbricon/eclipse.jdt.ls.git', branch:'wtf'
	sh "./mvnw clean verify -B -U -fae -e -Pserver-distro -DdisableP2Mirrors=true -Dtest=NavigateToDefinitionHandlerTest"
}
