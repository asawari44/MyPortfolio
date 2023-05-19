# MyPortfolio
My resume in the form of a website 
To run it locally : sudo docker run -ti -v $(pwd):/src   -p 1313:1313   -e HUGO_ENV="production" klakegg/hugo:0.74.3   server --disableFastRender --bind 0.0.0.0 -b "http://192.168.56.102:1313" -D

## How to trigger a new deployment
Just push to master and wait for jobs to trigger and checkout the new website when the job is successful! 


