FROM devillex/docker-firebase:slim

LABEL "com.github.actions.name"="Deploy to Firebase"
LABEL "com.github.actions.description"="Deploy a static site to Firebase Hosting"
LABEL "com.github.actions.icon"="cloud"
LABEL "com.github.actions.color"="orange"

LABEL "repository"="https://github.com/Raincal/actions/tree/master/deploy-firebase"
LABEL "homepage"="https://github.com/Raincal/actions"
LABEL "maintainer"="Raincal <cyj94228@gmail.com>"

ADD entrypoint.sh /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
