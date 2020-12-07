# Monolith to Microservice: Udagram Application
- DockerHub

    ![DockerHub](https://drive.google.com/uc?export=view&id=1yIjhkH2scD7QiY2LSZEkKGBGhkYpp0jk)
    
    
- Travis CI  
[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

    - Udagram-Frontend CI
    
        ![DockerHub](https://drive.google.com/uc?export=view&id=1j_-KojO3cEPvht2IN1uFTYSAwA2nBpfL)

        ![DockerHub](https://drive.google.com/uc?export=view&id=1shk3wTPiq_BFTkro4IMZbu8vGF8SRc3S)
        
    - Reverse-Proxy CI
    
        ![DockerHub](https://drive.google.com/uc?export=view&id=1Bco2kJkD8VpyLEls9A_zpXgPJjnLNMr9)
        
        ![DockerHub](https://drive.google.com/uc?export=view&id=1xQoELdCAZHJ8bnctdtpoz_PX6-xru5Xt)
    
    - Udagram-Api-Feed CI
    
        ![DockerHub](https://drive.google.com/uc?export=view&id=1hFQKAjWmNFo8hU0objZc7SHST0bneaBS)
        
        ![DockerHub](https://drive.google.com/uc?export=view&id=1gci8jSpu_u9-8j-WuC8hwk98PnOIrGuj)
    
    - Udagram-Api-User CI
    
        ![DockerHub](https://drive.google.com/uc?export=view&id=1yoBYueywIRBJLKg8yrUovuw1z2CY-R8R)
        
        ![DockerHub](https://drive.google.com/uc?export=view&id=1H-SsSnpVlYSUHGae1rQAVTk870UbEozB)



- Kubectl

    - kubectl get pods
    ![DockerHub](https://drive.google.com/uc?export=view&id=1nRwOg-_ZiAltFfW49Gq_NCTmYVdwwhQx)
    
    - kubectl get services
    ![DockerHub](https://drive.google.com/uc?export=view&id=19mTnL3ilyfkWHMg1w6ZTRQcJQkJRnLss)
    
    - kubectl describe services reverse-proxy
    ![DockerHub](https://drive.google.com/uc?export=view&id=1TtYJJzfrdik6FoEWBGgQqea2JbFdzFU4)
    
    - kubectl describe hpa
    ![DockerHub](https://drive.google.com/uc?export=view&id=1GyCRHDnpE9RAVac_bpIlqz8wOQnTU0QP)
    
    
- Backend

    - backend activity logs
    ![DockerHub](https://drive.google.com/uc?export=view&id=19D020PS_xVcu4DbScKFqvwVYj9FOsct4)

### Tech

This project is hosted entirely on AWS Elastic Kubernates Services using microservices architecture, where the the two microservice user , and feed are accessed through a reverse-proxy deployed to kubernates pods using Docker container technology.The container images are built using Travis CI pipelines where the continer images are pushed to and hosted on Dockerhub.



### Components

Links to the component repositories 

| Plugin | links |
| ------ | ------ |
| Frontend | https://github.com/prateekjoshi2013/udagram-frontend |
| Reverse Proxy | https://github.com/prateekjoshi2013/reverse-proxy |
| Feed | https://github.com/prateekjoshi2013/udagram-api-feed |
| User | https://github.com/prateekjoshi2013/udagram-api-user |
| App-URL | http://ab44713b3cf054bb9948b341994be63a-1407737393.us-east-1.elb.amazonaws.com:8100 |








