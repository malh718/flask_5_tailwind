# flask_5_tailwind


## This is the hw 
<img width="1017" alt="Screen Shot 2023-11-05 at 9 06 32 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/647f145f-6981-4443-8999-18e6a6e721df">
website: https://flaskhw-404222.ue.r.appspot.com/


## Step 1
I went online and I downloaded a cat video.

## Step 2 - Google Cloud CDN
I created a bucket using Google Cloud and changed the access to public. From here, I was able to get a url.

I chose GCP because of my issue with Azure and I was nervous because we didnt go over it in class, but it was simple. When setting up the CDN, I would just double check that the setting are correct and that there is public access. It should then just let you copy the url.

assets served from cdn
<img width="1413" alt="Screen Shot 2023-11-05 at 9 12 23 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/bcb72c59-0e84-47a8-9edf-cba8fc0e4ce9">

## Step 3- Flask App with TailwindCSS
Using the URL and the code from class I was able to change styling and add my video.
<img width="1242" alt="Screen Shot 2023-11-05 at 6 30 59 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/98d556dd-de95-452e-bba1-1c9f50aed6ba">

## Step 4 Deploying on GCP 

Deploying the flask app through GCP was straightforward and I followed the instructions present in class 2 HHA 506. From Here I created a new project entitled Flaskhw which has an id flaskhw422239. From Here i did gcloud config set project [PROJECT_ID] with the correct ID. I then added a .yaml file because I realized I had not copied that over. I had to make sure that I was in the right directory. S0 that was flask_5_tailwind. From there I did gcloud app deploy.  

<img width="911" alt="Screen Shot 2023-11-05 at 8 57 30 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/5ac72618-d363-43b3-a31d-f7054dcfe8c2">
<img width="708" alt="Screen Shot 2023-11-05 at 8 57 37 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/638560b6-c615-462f-adf5-7ae466492a20">

URL:https://flaskhw-404222.ue.r.appspot.com/

An error that I ran into was that I kept trying to deploy the app and I was getting things that said ERROR: (gcloud.app) Command name argument expected. or command not found. But then I realized when I was copy and pasting gcloud app deploy, there must have been an added space or some weird formatting because then it ultimately worked!
<img width="687" alt="Screen Shot 2023-11-05 at 9 37 05 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/dedd8554-d786-4746-9cc6-a8ecd78e0356">

up to date <3
<img width="656" alt="Screen Shot 2023-11-05 at 9 39 08 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/e616b31e-3552-49a3-b3a0-233aba96cd7c">

Initially I was going to deploy on Azure, but then I saw that my subsciption to Azure for Students was disabled, which was not a good sign. So that is why I switched to GCP, and thankfully was able to deploy successfully.

<img width="1436" alt="Screen Shot 2023-11-05 at 9 25 53 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/d1307879-266b-421c-b939-650fd07a1480">


My video is responsive:app deployed and running 
<img width="1009" alt="Screen Shot 2023-11-05 at 9 27 12 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/4dbdad78-8547-49c0-9773-06310d1dad35">

<img width="980" alt="Screen Shot 2023-11-05 at 9 41 35 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/f52be9a2-3d3f-426e-8fbe-e914580dddb7">



<img width="923" alt="Screen Shot 2023-11-05 at 9 41 21 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/9fd586d6-a568-4b04-b562-5dd6d9859919">



I was able to deploy the app, and then I disabled the application.

<img width="827" alt="Screen Shot 2023-11-05 at 9 26 42 PM" src="https://github.com/malh718/flask_5_tailwind/assets/102617334/cb7dd0b7-256e-42b9-9108-60f0e7a40d77">


### This is the code that I put in tailwind css
<body class="bg-white-100 font-sans">
    <header class="bg-purple-300 text-black text-center p-4">
        <h1 class="text-2xl">📎💈 Maliha's Flask App  🏘🐇 </h1>
    </header>
    <nav class="flex justify-between bg-gray-800 p-2">
        <a href="#" class="text-white px-4 py-2">Home</a>
        <a href="#" class="text-white px-4 py-2">About</a>
        <a href="#" class="text-white px-4 py-2">Services</a>
        <a href="#" class="text-white px-4 py-2">Contact</a>
    </nav>
    </div>
    <main class="p-8">
        <h2 class="text-xl mb-4">Welcome to My Flask App! </h2>

    <div class="overflow-hidden rounded-lg bg-black">
    <video controls class="h-full w-full">
        <source src="https://storage.googleapis.com/flas/video_of_black_cat%20(Original).mp4" type="video/mp4" />
        Your browser does not support the video tag.
    </video>
    </div>
   <p>This is a simple Flask app and I have imbedded a link to a video of a cat.</p>
    </main>
    <div cl
    <footer class="text-center p-4 bg-purple-300 text-white">
        <p>Copyright © 2023 My Flask App</p>
    </footer>
</body>
