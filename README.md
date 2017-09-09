# Introduction to Kubernetes

Slides: 

## Set up and installation
- Install an editor that you want to want to use for coding. 
- Install Java SDK: http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
  - Test that it works by typing `java -version`
- Install node and npm: https://docs.npmjs.com/getting-started/installing-node
  - Test that it is correctly installed by typing `node -v` and `npm -v` 
- Install Docker: https://www.docker.com/community-edition
  - Start docker
- Create an account on Google Cloud Platform. 
  - Go to: https://console.cloud.google.com 
  - Sign up. You will have to register a payment method to complete the sign up. The first 100 days are free, so you should not be charged anything for your account.
  - Create a project
- Install Google Cloud command-line tool (gcloud): https://cloud.google.com/sdk/downloads
- Install Kubernetes command-line tool (kubectl). Run the following command in the terminal to install: `gcloud components install kubectl`

## Tasks
 - [Google Cloud Platform: Setup](tasks/google-setup.md)
 - [Run local](tasks/run-local.md)
 - [Run in cloud](tasks/run-in-cloud.md)


## More information

### The REST endpoints

#### Contact Information
Get all contact information: `/me`. Returns json with content. 
Example: 
```
{
    name: 'Espen Askeladd',
    location: 'Oslo'
}

```
#### Education
Get all education experience: `/education`. Returns a list of objects. 
Example: 
```
[
    {
        year_from: '2010',
        year_to: '2013',
        place: 'University of Oslo',
        comment: 'Bachelor\'s degree'
    },
    {
        year_from: '2013',
        year_to: '2015',
        place: 'University of Oslo',
        comment: 'Master\'s degree'
    }
]
```

#### Work
Get all work experience: `/work`. Returns a list of objects on the same format as education. 
