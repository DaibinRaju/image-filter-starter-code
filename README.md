# Udagram Image Filtering Microservice

GitHub repo: https://github.com/DaibinRaju/image-filter-starter-code

Eb endpoint: http://image-filter-starter-code-dev2222222.us-east-1.elasticbeanstalk.com/

Eb filteredimage api: http://image-filter-starter-code-dev2222222.us-east-1.elasticbeanstalk.com/filteredimage?image_url=https://www.telegraph.co.uk/content/dam/Travel/Cruise/Port-guides/Manaus/iStock-1133159537-manaus-city_cropped-xlarge.jpg


##How to deploy

CD into Project driectory

Install node modules and run application locally
```bash
npm i
npm run dev
```
Create run build files
```bash
npm run build
```

Install awsebcli
Using homebrew
```bash
brew install awsebcli
```

Init eb application
```bash 
eb init
```

copy foolowing code into .easticbeanstalk/config.yml configuration file
```yml
deploy:
    artifact: ./www/Archive.zip
```

Create eb environment
```bash
eb create
```

Go to AWS EB console to view the application

