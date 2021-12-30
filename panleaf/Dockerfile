FROM sharelatex/sharelatex:latest

LABEL mainter="laekov"
LABEL version="v0.0.1"

RUN wget https://github.com/jgm/pandoc/releases/download/2.16.2/pandoc-2.16.2-1-amd64.deb -o /root/pandoc.deb
RUN dpkg -i /root/pandoc.deb
COPY LatexRunner.js /var/www/sharelatex/clsi/app/js/pandoc.wrapper
COPY ProjectEntityUpdateHandler.js /var/www/sharelatex/web/app/src/Features/Project/ProjectEntityUpdateHandler.js
COPY SettingsController.js /var/www/sharelatex/web/frontend/js/ide/settings/controllers/SettingsController.js
COPY pandoc.wrapper /usr/bin
