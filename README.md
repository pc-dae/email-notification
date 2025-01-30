# Notifcation Management

This is a Contact API client.

## Setup
```
git clone git@github.dev.global.tesco.org:336-ISE-Control-plane/email-notification.git
cd email-notification
```

## Compile
To compile and build jar...
```
VERSION="${VERSION:-$(git rev-parse --abbrev-ref HEAD)}"
./mvnw -Dbranch_version=$VERSION clean verify package
```
## Execute
```
java -jar target/email-notifications-$VERSION.jar --input data/email1.mustache --data data/data.json --output data/out.json
```
