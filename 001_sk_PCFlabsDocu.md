#First Start
- Install on MacOS: https://docs.pivotal.io/pcf-dev/install-osx.html
- cf dev start (cf dev stop)
- To begin using PCF Dev, please run:  cf login -a https://api.local.pcfdev.io --skip-ssl-validation

Apps Manager URL: https://apps.local.pcfdev.io
Admin user => Email: admin / Password: admin
Regular user => Email: user / Password: pass

#Sample App
Original https://s3.amazonaws.com/pivotal-training-material/PCF+Developer/pcf-developer-1.7.a.RELEASE-labs.zip
Beispiel APP https://github.com/bbertka-pivotal/PCF-101-Workshop.git
oder https://github.com/cloudfoundry-samples

cf push articulate -p ./articulate-0.2.jar -m 512M --random-route --no-start

cf push node --random-route -m 128M  -b https://github.com/cloudfoundry/nodejs-buildpack
ggf. Node Version anpassen

Java App Beispiel
  cf push --hostname javaapp

LogDrain
pcfdev-log-drain will log to logs7.papertrailapp.com:12107
