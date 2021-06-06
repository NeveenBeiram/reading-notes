# AWS: Cloud Servers

* Describe the Web-Request-Response-Cycle
 request/response cycle is a useful guide to see how all the app’s files and folders fit together. The request/response cycle traces how a user’s request flows through the app.
 
1. A user opens his browser, types in a URL, and presses Enter.
2. When a user presses Enter, the browser makes a request for that URL.
3. The request hits the Rails router (config/routes.rb). The router maps the URL to the correct controller and action to handle the request.
4. The action receives the request and passes it on to the view.
5. The view renders the page as HTML.
6. The controller sends the HTML back to the browser. The page loads and the user sees it.
 [source](https://www.codecademy.com/articles/request-response-cycle-static)

* Explain what a “server” is, as it relates to the WRRC
A server is a computer program or device that provides a service to another computer program and its user, also known as the client

* What does it mean to “deploy” an application?
Deploying your application means putting it on a Web server so that it can be used either through the Internet or an intranet.[source](https://supportline.microfocus.com/documentation/books/sx22sp1/pidepl.htm)

## Term
- Server:A server is a computer program or device that provides a service to another computer program and its user, also known as the client

- Pub/Sub:Pub/Sub is an asynchronous messaging service that decouples services that produce events from services that process events.[source](https://cloud.google.com/pubsub/docs/overview)

- WRRC: Web Request Response Cycle.request/response cycle is a useful guide to see how all the app’s files and folders fit together. The request/response cycle traces how a user’s request flows through the app.

<hr>

### Virtual Machine 
Virtual machines are based on computer architectures and provide functionality of a physical computer. Their implementations may involve specialized hardware, software, or a combination.

### AWS EC2
Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers. Amazon EC2’s simple web service interface allows you to obtain and configure capacity with minimal friction. It provides you with complete control of your computing resources and lets you run on Amazon’s proven computing environment.


<hr>

[Virtual Machines](https://www.youtube.com/watch?v=yIVXjl4SwVo)

[VMS and the Cloud](https://www.youtube.com/watch?v=l0DfHUWMjsU)

[AWS EC2](https://aws.amazon.com/ec2/)

[EC2 For Humans](https://www.youtube.com/watch?v=lZMkgOMYYIg)

[Elastic Beanstalk](https://www.youtube.com/watch?v=SrwxAScdyT0)