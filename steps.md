# Node JS - Mongo

````console
//clone repository with --bare
git clone --bare https://github.com/zeeemughal/product_backend.git 

// create a new repository and push to that
git push --mirror git@github.com:faisalabbasm/product-backend.git

//clone new repository
git clone git@github.com:faisalabbasm/product-backend.git

````

````console
// create docker file

//build docker file
docker build -t product-backend:1.0 .

// run docker image
docker run -e PORT=4040 -e MONGODB_URI="mongodb+srv://evently_user:BpNf2C0bFx09vDKD@evently.ugjztes.mongodb.net/?retryWrites=true&w=majority" -p 4040:4040 product-backend:1.0

// add a tag with cotainer before pushing to docker registry
docker tag product-backend:1.0 faisalabbasm/product-backend:1.0

//push to docker registry
docker push faisalabbasm/product-backend:1.0
````