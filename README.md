<h1> Travel Memory <h1>
.env file to work with the backend after creating a database in mongodb:

MONGO_URI='ENTER_YOUR_URL'

PORT=3001

Add this data into DB, Data format to be added:

{

    "tripName": "Trip to USA",
    "startDateOfJourney": "10-09-2024",
    "endDateOfJourney": "30-09-2024",
    "nameOfHotels":"Hotel marriot
    "placesVisited":"California, Newyork",
    "totalCost": 1000000,
    "tripType": "leisure",
    "experience": "test, ",
    "image": "test.com",
    "shortDescription":"test"
}

From Backend application confoguration see the readme.md page in backend-Deployement-notes

From frontend application confoguration see the readme.md page in frontend-Deployement-notes

Task 4: Scaling the Application with Load Balancer:

• Launch Additional EC2 Instances: Create multiple EC2 instances running both the frontend and backend of the TravelMemory application.

• Set Up Load Balancer: Use AWS Elastic Load Balancer (ELB) to distribute traffic across your EC2 instances:

• Go to the EC2 Dashboard and click on Target Groups and Create Target Groups.

• Go to the EC2 Dashboard and click on Load Balancer and Create Load Balancers.

• Create a new Application Load Balancer.

• Add all the instances running the backend under the Target Group.

• Configure Load Balancer Listener: Set the listener to forward traffic to your EC2 instances on port 80 (Nginx proxy).

<h1> Check the test results and instructions in the word document which is located in Travel-Memory-Application-Deployment repo

